Software installed

1. PostgreSQL 18 (via EnterpriseDB installer for Windows), full component set: PostgreSQL Server, pgAdmin 4, Stack Builder, Command Line Tools. Stack Builder itself was skipped, no extras installed through it.
2. pgAdmin 4 (bundled with the PostgreSQL installer above), used for all database and role setup.

Database setup, done in pgAdmin

1. Registered local server connection, host localhost, port 5432, maintenance database postgres, username postgres.
2. Created login role saiprice_user under Login/Group Roles, with login privilege enabled and a password set.
3. Created database saiprice_db under Databases, owner set to saiprice_user.

Python packages installed, via pip inside venv

1. psycopg2-binary
2. python-decouple

Both were installed twice in practice. First attempt landed outside the active project venv by mistake, second attempt after diagnosis landed correctly.

Files created or edited

1. .env created in project root, containing DB_NAME, DB_USER, DB_PASSWORD, DB_HOST, DB_PORT. Confirmed excluded from git via existing .gitignore.
2. saiprice/settings.py edited, added from decouple import config near the top, replaced the sqlite3 DATABASES block with a postgresql block reading all five values from config().
3. requirements.txt regenerated with pip freeze > requirements.txt, run twice, once before diagnosing the missing packages, once after, to lock in the corrected state.

Commands run to verify and debug

1. pip show python-decouple, used to confirm the package was actually present in the active environment. First run came back not found, second run after reinstalling confirmed it.
2. pip show psycopg2-binary, same pattern, confirmed missing then confirmed installed.
3. where python, returned nothing due to PowerShell aliasing where to Where-Object instead of the real path lookup.
4. Get-Command python, correct PowerShell equivalent, confirmed the active interpreter path pointed into the project's own venv, not a stray global Python.
5. python manage.py migrate, run twice. First run failed with ModuleNotFoundError for psycopg2. Second run, after the package was actually installed in the right venv, succeeded and applied Django's default migrations.

Git commands run

1. git status, checked before staging to confirm .env was not present and requirements.txt was.
2. git add .
3. git commit -m "Connect Django to PostgreSQL"
4. git push, rejected on first attempt because the remote had a commit not present locally.
5. git pull --rebase, pulled the remote commit and replayed the local commit cleanly on top, no conflicts.
6. git push, second attempt, succeeded.

Bugs hit and root cause, worth keeping in your log so you don't repeat them

1. Missing packages twice, decouple and psycopg2. Root cause was not an interpreter mismatch, it was simply not having run the install command yet inside this specific venv at the time settings.py was written. Confirmed after the fact that terminal and interpreter were correctly aligned the whole time.
2. Push rejected. Root cause was a remote commit that predated your session, likely an earlier edit made directly through GitHub's web interface. Fixed with a rebase, not a merge, keeping your commit history linear.