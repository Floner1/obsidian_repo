	revised ipq notes 2-10-26 and added some more stuff

# Plan changes

### Version 1 (09-09-2026): 2013 vs 2014 with FastF1 lap and sector data

- Plan: compare 2013 and 2014 teammates around the 2014 radio coaching ban.
- Data: FastF1 lap and sector data.
- Confound named: the V6 hybrid power unit.
- Context: the 1994 and 2008 driver-aid bans, qualitative only.
- Why it looked reasonable: the ban was a clear date, Horner and Wolff disagreed about it on record, and teammate gaps cancel most of the car.

### What was wrong with version 1 (found 02-10-2026)

- Sector data: FastF1 documents full data support only from 2018. Jolpica's laps data has driverId, position and lap time, with no sectors. 2013 and 2014 have no sector data.
- Ban date: the ban was enforced from Singapore (21-09-2014), round 14 of 19 in 2014. Only 6 races of 2014 fall after it.
- Power units: the V6 hybrid arrived in 2014 (the season started 16-03-2014), so 2013 vs 2014 mostly compares cars.
- Pairs: only 2 of 11 teammate pairs stayed together from 2013 to 2014 (Mercedes and Marussia). Marussia's pair broke up after Bianchi's crash at the Japanese GP.
- Title fight: Hamilton and Rosberg fought for the 2014 title. That is another factor I cannot adjust for.
- Link to the question: the test measures a coaching ban. The question is about data-driven strategy. I owe a defence of that link (see Question, hypothesis and prediction).

### Version 2 (01-10-2026): the within-2014 split plus a 2013 Mercedes baseline

- Test: compare teammate lap-time gaps in 2014 rounds 1 to 13 against rounds 14 to 19, around the FIA coaching ban. 2013 Mercedes is a thin baseline.
- Data: lap times, positions and driver IDs from jolpica. No sector data exists for 2013 or 2014.
- Confound: the V6 started at round 1, so both halves of 2014 run it. Car development stays an open confound.
- Limits to state: 6 post-ban races, about 9 stable pairs, and only driver coaching was banned.

Why the within-2014 split helped:

- Both halves of 2014 run the V6, so only the coaching rule changes.
- About 9 pairs kept the same two drivers all season in 2014. Marussia lost Bianchi after Japan and Caterham used substitute drivers.
- It still had one change point and only 6 post-ban races.

#### How the 2013 baseline was meant to work

- Why include 2013: it gives a baseline for the 2014 result. Without it, I cannot tell whether a change in the teammate gap after round 14 comes from the ban or from ordinary variation.
- How: apply the same split to 2013 (rounds 1 to 13 vs 14 to 19). Coaching was legal all of 2013, so this shows how much the gap normally moves between those two stretches.
- Reading it: if the 2014 shift is clearly larger than the 2013 shift, that supports a ban effect. If the two are similar, the shift is normal variation.
- Never compare raw 2013 numbers against raw 2014 numbers. The car changed, completely new chassis, engine, regs, etc.
- Why only Mercedes: it was the only pair that raced together through both full seasons.

#### Questions I asked about the baseline, and the answers

- On comparing only 2014 coaching with 2014 non-coaching: I can, and it is the core test. The 2013 data answers one extra question, which is whether the change after round 14 is bigger than the gap normally moves. The last 6 races of 2014 are different circuits, the cars develop through the season, and Hamilton and Rosberg were racing for the title. Any of those could change the gap without the ban.
- On whether 2013 gives a true value for racing with coaching: partly. Coaching was legal all year, neither Mercedes drivers were heavily involved in the title fight, so it is cleaner than 2014 on that one factor. It is not a true value. The 2013 car is different, Hamilton was new in 2013 replacing Schumacher and Pirelli (the tire supplier for f1) changed tire construction in germany (round 9 7/7/13) and in hungary (round 10 28/7/13)
- On why the baseline is thin: it rests on one pair and one season. It sizes ordinary variation. It proves nothing alone, and it is not a control.
- I had established a rule in v2 of the plan: if the gap numbers, the shift and the permutation test are not final by Sun 25-10-2026, drop the 2013 baseline first, as it would put me behind schedule.

### Version 3 (current, 05-10-2026): the ban on and off across 2014 to 2016

I found a better idea than version 2. It uses the 2014 and 2016 races with no ban against the races with a ban from 2014 to 2016.

How I got there:

- First thought: compare before the ban, during the ban and after it. The problem was that the cars differ widely across those periods.
- Before the ban, only Rosberg and Hamilton stayed together from 2013 to 2014, and they were fighting for the 2014 title.
- The ban was lifted at the German Grand Prix in 2016, so the end of the ban is a second change point.
- No ban: 2014 rounds 1 to 13 plus 2016 rounds 12 to 21 (German GP onward). That is 13 + 10 = 23 races.
- Ban: 2014 rounds 14 to 19 plus all of 2015. That is 25 races. The first 11 races of 2016 had a stricter ban and form a separate group.

Why version 3 is better:

- The ban starts and ends, so I test the change twice instead of once.
- The post-ban sample grows from 6 races to 25 (36 with the stricter 2016 races).
- Mercedes, Williams and Force India kept the same pair for 2014, 2015 and 2016, so I get 3 pairs instead of 1.
- If the gap moves when the ban starts and moves back when it ends, that is much stronger than a single shift.
- It replaces the 2013 baseline. The ban ending in 2016 does the job that 2013 was meant to do, and 2013 had one usable pair and a different car.

What stays from version 2:

- The gap measure, the cleaning rules and the permutation test (see Method).
- The V6 stays constant across 2014 to 2016, so the power unit change drops out.

What it costs:

- More data to pull and clean: 59 races across 3 seasons.
- Probably one or two extra sessions.

### Question change (05-10-2026)

- Original question (09-09-2026): whether data-driven strategy reduces the role of driver skill in F1.
- New question (03-10-2026): To what extent did the FIA's 2014 to 2016 ban on in-race driver coaching change the lap-time gap between teammates in F1?

Why I changed it:

- The old question was bigger than my test. Data-driven strategy covers pit and tyre decisions as well as radio coaching, and my test covers only coaching.
- Driver skill has no direct measure. The teammate lap-time gap measures it only indirectly.
- The syllabus (2023 to 2025) asks for a question that is specific and answerable through evidence (page 8). The new question names the ban and the measure, so my data can answer it directly.
- With the old question, my conclusion would have needed heavy qualification, because the question went further than the test.

What I keep:

- The original topic. In-race coaching is data-driven instruction from the pit wall, so I connect it to data-driven strategy and driver skill in the introduction and the evaluation, and I state the limits there.

## Question, hypothesis and prediction

- Original research question (09-09-2026): whether data-driven strategy reduces the role of driver skill in F1.
- Current research question (changed 05-10-2026, see Plan changes): To what extent did the FIA's 2014 to 2016 ban on in-race driver coaching change the lap-time gap between teammates in F1?
- Link to the original topic: in-race coaching is data-driven instruction from the pit wall, so it is one part of data-driven strategy. The test covers only that part.
- 150-word definition owed (due Fri 09-10). It must define in-race coaching and the teammate gap, then add one sentence on how coaching connects to data-driven strategy and what the test leaves out.
- Hypothesis: banning coaching removes help for the weaker driver, so the teammate gap should widen when the ban starts and narrow again after it ends.
- Write the prediction in the log before I see any data.
- I can't test that the ban makes races "less exciting and competitive". Lap gaps do not measure excitement, can be part of context in FIA's debate.
- FIA motive, reported by Motorsport.com: make drivers "heroes again". Check the original wording before quoting.
- Opposing views: Horner and Wolff disagreed on record (from my 05-09 notes, see Links).

## Background: the radio ban timeline

### 2014: announced and enforced

- 11-09-2014: FIA directive. Charlie Whiting: "No radio conversation from pit to driver may include any information that is related to the performance of the car or driver."
- Applied from Singapore, round 14 of the 2014 season, 21 9 2014
- Purpose: enforce Article 20.1 of the sporting regulations, "The driver must drive the car alone and unaided."
- Article 20.1 appears word for word in the 2014 Sporting Regulations (28-02-2014 version, see Links): "The driver must drive the car alone and unaided." A text search of all 55 pages found no article on team radio. Radio appears only in Articles 12.5, 34 and 40.1 and the podium ceremony rules, and none limits messages to drivers. RaceFans (11-09-2014) and Formula1.com (16-09-2014) both give Article 20.1 as the basis for the ban. Amendments after 28-02-2014 are not covered.
- Whiting also reminded teams that data transmission from pit to car is prohibited by Article 8.5.2 of the Technical Regulations. The article reads "Pit to car telemetry is prohibited." in the 2014 Technical Regulations (23-01-2014 version, see Links), in the 2011 issue of the 2014 regulations and in the 2015 Technical Regulations (29-06-2014 version). The 2011 and 2015 files were searched in full. The 23-01-2014 file was read at Article 8.5 only.
- Article 8.7 of the Technical Regulations, "Driver radio", covers the radio equipment and not what teams say. A voice radio system between car and pits must be stand-alone and must not transmit or receive other data. All such communications must be open and accessible to the FIA and broadcasters. The wording is the same in the 2011 issue, the 2015 version (29-06-2014) and the 2016 version (27-02-2016).

### 2014: revised to driver performance only

- Banned immediately (examples named by Formula1.com): driving lines on the circuit, contact with kerbs, braking points, throttle application in general, driving technique in general.
- Postponed to 2015 (car performance): car set-up parameters for specific corners, and comparative data between drivers' speeds and gear selections.
- Reason given: "the complexity of introducing such a ban at short notice".
- Sources disagree on gear selection. Formula1.com puts it in the postponed group. Motorsport.com's 2016 analysis puts it in the first phase. Cite Formula1.com and say the sources differ.

### 2015

- The push to widen the ban to car performance for 2015 was abandoned. Only the driver-coaching phase stayed in force through 2015.
- Sources: Autosport and Motorsport.com. Neither has been read in full and no publication dates were visible. Find the dated originals before citing.
- A text search of all 57 pages of the 2015 Sporting Regulations (03-12-2014 version, see Links) found no team radio article. Article 20.1 is unchanged. Amendments published during 2015 are not covered.

### 2016

- Full ban from the Australian Grand Prix (round 1). Engineers could not give technical guidance.
- 28-07-2016: the FIA lifted the limits from the German Grand Prix (31-07-2016, round 12).
- FIA wording, quoted by RaceFans: "With the exception of the period between the start of the formation lap and the start of the race, there will be no limitations on messages teams send to their drivers either by radio or pit board."
- The FIA framed it as better content for fans, because teams must give the commercial rights holder unrestricted access to the messages.
- A text search of all 56 pages of the 2016 Sporting Regulations (20-04-2016 version, see Links) found no team radio article. Amendments after 20-04-2016 are not covered.

### Today

- F1 Oversteer says only the formation lap is still restricted. The 2026 regulations are not checked.
- That matches what I hear on the radio now: car adjustments and corner losses.
- Discarded: a page on f1briefing.com claims strict current limits on engineer advice. It contradicts the FIA's 2016 statement.

### Article numbers

- 2014 and 2015 Sporting Regulations: Article 20.1, "The driver must drive the car alone and unaided."
- 2016 Sporting Regulations (20-04-2016 version): the same sentence is Article 27.1. The regulations were renumbered, so cite 27.1 for 2016.
- RaceFans (2016) cites 27.1, which matches. Motorsport.com cites 20.1, which matches the 2014 and 2015 numbering.
- 2014 and 2015 Technical Regulations (23-01-2014 and 29-06-2014 versions): Article 8.5.2, "Pit to car telemetry is prohibited."
- 2016 Technical Regulations (27-02-2016 version, see Links): the same sentence is Article 8.5.3. The 2016 text adds a new Article 8.5.1, so the old 8.5.1 and 8.5.2 became 8.5.2 and 8.5.3.
- Article 8.7 (Driver radio) keeps its number in the 2011, 2015 and 2016 versions.

### What the ban stops, with examples

Coaching ban (2014 and 2015), driver performance only:

- Braking points. Named in the Formula1.com revision of September 2014.
- Racing lines. The same revision names driving lines on the circuit, contact with kerbs, throttle application and driving technique.
- Gear selection. Sources disagree. Formula1.com puts it in the postponed group, and Motorsport.com's 2016 analysis puts it in the first phase. Cite Formula1.com and say the sources differ.

Full ban (2016 only), which also covered car performance:

- Car set-up adjustments. Postponed in 2014, dropped for 2015 and covered only by the stricter 2016 ban.
- Direct technical questions, such as torque map settings. No source reviewed names torque maps, so treat this as an example of car performance advice and not as a quoted rule.

The examples are grouped by ban type because braking points, racing lines, gear selection, car set-up and torque maps do not all belong to the same ban. The split matches the groups in the data. The full-ban races stay separate because the 2016 ban covered more.

### Earlier context from my 09-09 notes

- 1994 and 2008 driver-aid bans (active suspension, traction control, ABS, launch control). The FIA's reasoning was that the technology had started deciding races more than drivers.
- Traction control returned in 2001 because the FIA could not police the ban, then was banned again in 2008 once the standard ECU could catch it.
- This gives the radio ban a second, earlier example of the same argument.

## Groups, race counts and pairs

### The three groups

- No ban (coaching legal): 2014 rounds 1 to 13 (13 races) plus 2016 rounds 12 to 21 (10 races). Total 23.
- Coaching ban: 2014 rounds 14 to 19 (6) plus all of 2015 (19). Total 25.
- Full ban (stricter): 2016 rounds 1 to 11. Total 11. Kept as a separate group.
- All races: 59. Races under any ban: 36.
- Main comparison: no ban vs coaching ban. Check: add the full-ban races and see whether the result moves.

### After removing wet races

- No ban: 21. Coaching ban: 22. Full ban: 9. Total: 52.
- Wet races removed: Hungary 2014 and Brazil 2016 (no ban), Japan 2014, Britain 2015 and USA 2015 (coaching ban), Monaco 2016 and Britain 2016 (full ban).
- This rests on my wet-race list, checked against race pages, and on the whole-race rule (see Wet races).

### Fixes to my earlier notes

- 2016 has 21 rounds, not 19. The German GP is round 12. No-ban races in 2016 are rounds 12 to 21, which is 10 races. My note "last 9 rounds" excludes Germany. 13 + 9 would be 22, not 23.
- "30 no coaching races when accounted for rain" should be 21. The other 9 are the stricter 2016 full-ban races.

### Pairs (line-ups from the 2014, 2015 and 2016 season pages)

- Mercedes: Rosberg and Hamilton, 2014 to 2016.
- Williams: Massa and Bottas, 2014 to 2016.
- Force India: Pérez and Hülkenberg, 2014 to 2016.
- Ferrari: Vettel and Räikkönen, 2015 and 2016 only. In 2014 it was Räikkönen and Alonso.
- Mercedes, Williams and Force India all run Mercedes power units. Ferrari does not. The result describes those teams, not the whole grid.

## Method

### Data

- Source: jolpica laps (driverId, position, time), through FastF1's Ergast interface or the API directly.
- Pull 2014, 2015 and 2016.
- Write the gap calculation once as a function and loop it over every race. Do not run races by hand.
- Not tested live. Access is confirmed from documentation only. The smoke test (2014 round 1 laps) settles it. It was planned for Sat 03-10.

### Gap measure

- Per race and per pair: median lap time for each driver on clean laps, using matched lap numbers.
- Gap = the difference as a percent of lap time. Use the absolute value, so it does not matter who is faster.
- One number per race and pair.
- Example with made-up numbers: if one driver's median lap is 90.00 seconds and the other's is 90.18, the gap is 0.20 percent.

### Cleaning rules

- Green-flag laps only. Reason (mine): the lap should show racing pace.
- Drop lap 1. Reason: it depends on grid position and traffic.
- Drop pit in-laps and out-laps. Reason: they do not show pace.
- Drop safety-car laps. Reason: same.
- Drop wet races. Reason: wet conditions change what lap time measures, and the data has no weather for each lap, so I drop the whole race (see Wet races).

### Wet races

- Wet races: 2014 Hungary and Japan. 2015 Britain and USA. 2016 Monaco, Britain and Brazil. That is 7 of 59, so 52 are dry.
- First source: a Reddit list of wet-weather races. Reddit is user-compiled and weak as evidence.
- Check: I checked all 59 races against their race pages (Wikipedia for 57 races, f1-fansite.com for the 2014 Australian and Malaysian races, see Links). The result matches the Reddit list on all 7 wet races.
- What the race pages say about the 7: Japan 2014 and Brazil 2016 were wet throughout. Hungary 2014, USA 2015, Monaco 2016 and Britain 2016 started wet and dried out. Britain 2015 started dry and turned wet from about lap 33.
- Rule (04-10-2026): I drop every wet race. A race is wet if its race page says any part of it ran on intermediate or wet tyres.
- Reasons: the lap data gives times and positions but no weather or tyre data for each lap, so I cannot tell wet laps from dry laps inside a mixed race. Dropping the whole race also keeps the method simple.
- Cost: 7 of 59 races, which is 12 percent. That leaves 52. Britain 2015 loses about 30 dry laps, because rain began around lap 33.
- Labels come from the weather only. I do not change a label after seeing the gap numbers.
- Optional check: if the result lands close to p = 0.05, rerun it with the 5 mixed-condition races kept and see whether it moves.

### Statistics: the shift

- Shift = average gap in the banned group minus average gap in the no-ban group.
- Example with made-up numbers: no-ban gaps 0.20, 0.30 and 0.25 average 0.25. Banned gaps 0.35, 0.40 and 0.30 average 0.35. The shift is +0.10 percentage points.
- With the ban starting and ending, I get two shifts. The first should be positive (gap widens). The second should be negative (gap narrows again).

### Statistics: the permutation test

- Put all the gap numbers in one pile and throw away the labels.
- Shuffle the pile and deal it into a fake no-ban group and a fake banned group, the same sizes as the real ones.
- Calculate the shift for the fake groups. Repeat 10,000 times.
- The p-value is the share of shuffles that gave a shift as big as mine or bigger.
- Most reports use 0.05 as the cutoff. That is a convention, not a law.
- Run it per pair and pooled.
- Why a permutation test: it assumes nothing about the shape of the data. This is my reasoning, not a sourced rule.
- Practice run on the made-up numbers above: shift +0.10, p about 0.10. Three races per group is too few for a convincing result. My real groups have 21 and 22 races.

```python
import numpy as np
legal = np.array([0.20, 0.30, 0.25])
banned = np.array([0.35, 0.40, 0.30])
observed = banned.mean() - legal.mean()
pooled = np.concatenate([legal, banned])
rng = np.random.default_rng(1)
count = 0
for _ in range(10000):
    rng.shuffle(pooled)
    if pooled[:len(banned)].mean() - pooled[len(banned):].mean() >= observed - 1e-9:
        count += 1
print(observed, count / 10000)
```

### What a small p-value means

- A small p-value says the shift is unlikely to be random race-to-race noise. It does not say what caused the shift.
- Other things changed at the same time: the cars, the season and the title fight. Suppose the 2015 car suited one driver better. The gap would widen without any help from the ban, and the test would still give a small p-value.
- Three checks raise my confidence: the shift appears at the date the ban started (Singapore 2014) and not before, the gap moves back after the ban ended (German GP 2016), and all pairs move in the same direction.
- Wording in the report: "consistent with the ban having an effect". Never "the ban caused it".
- A p-value of 0.03 does not mean a 97 percent chance the ban worked. It means that if the ban did nothing, about 3 percent of shuffles would give a shift this big.

### Is the sample big enough

- Smallest shift I could detect at 80 percent power and a 5 percent level, in standard deviations (SD) of the race-to-race gap:
    - old 6-race design: about 1.4
    - one pair, 23 vs 25 races: about 0.8
    - three pairs pooled: about 0.5
    - with 15 percent of races lost (my assumption): about 0.87 and 0.51
- Dropping the 7 wet races loses 12 percent of races, which sits inside that 15 percent assumption.
- These figures come from the standard two-sample approximation. No source yet. Find a statistics text to cite before using them.
- The real SD is unknown until the data is pulled.
- Rule: if my shift is smaller than these thresholds, report the result as inconclusive. That is a valid finding and the evaluation marks reward it.

## Evaluation notes (limits to write up)

- Two rule changes only. More races reduce noise but cannot separate the ban from other things that changed at the same time. Say so.
- Cars differ across seasons. A teammate gap cancels most of the car within a race. It does not cancel how well a car suits each driver.
- Title fights: as far as I know, Hamilton and Rosberg fought for the 2014 and 2016 titles but not 2015. Check on the season pages.
- Races from the same pair and season are correlated, so the p-value looks better than it should.
- Mercedes, Williams and Force India all use Mercedes power. The result covers those teams.
- Coaching is one part of data-driven strategy, so the finding says little about the rest. The 150-word definition covers the link.
- Lap-time gap is an imperfect measure of skill.
- The stricter 2016 ban is a different treatment, so it stays a separate group.
- No sector data, so no corner-level analysis.
- Data access is confirmed from documentation only until the smoke test runs.
- Five of the 7 races dropped as wet had mixed conditions, so they also lose their dry laps (see Wet races). The findings cover dry races only. Wet races may show larger teammate gaps. No source yet.
- The 2014 ban was enforced through a race director directive reading Article 20.1, and no article in the 2014, 2015 or 2016 Sporting Regulations, or in the Technical Regulations searched, limits what teams may say by radio. Technical Regulations Article 8.7 covers the radio equipment only. I cannot say how strictly teams complied.
- Version 1 and version 2 problems (see Plan changes) can be used here as evidence that I tested my own design.

## Source evaluation

### Strong

- FIA Sporting Regulations 2014 (28-02-2014), 2015 (03-12-2014) and 2016 (20-04-2016): primary sources, searched in full for radio rules. None found. Article 20.1 in 2014 and 2015, Article 27.1 in 2016.
- FIA Technical Regulations 2015 (29-06-2014, 88 pages) and 2016 (27-02-2016, 90 pages): primary sources, searched in full. Article 8.5.2 (8.5.3 in 2016) reads "Pit to car telemetry is prohibited." Article 8.7 (Driver radio) covers the radio equipment only.
- FIA Technical Regulations 2014 (23-01-2014): primary source. Only Article 8.5 was read. It gives Article 8.5.2 as "Pit to car telemetry is prohibited."
- Formula1.com, 11-09-2014 directive article: official F1 site, dated. Gives the Whiting quote and the Singapore start.
- Formula1.com, September 2014 revision: official. Lists banned and postponed examples.
- RaceFans, 11-09-2014: dated report. Gives Article 20.1 as the basis and cites no radio article.
- Formula1.com, 16-09-2014: official, dated. Gives Article 20.1 and the list of allowed and banned messages.
- RaceFans, 28-07-2016: dated report quoting the FIA decision to lift limits.
- Cambridge 9980 syllabus (2023 to 2025): official. Check the 2027 version.
- UCAS QIP page: assessment weights, AO1 70 percent and AO2 reflection 15 percent.
- FastF1 documentation and jolpica documentation: official project docs.

### Usable with checks

- Motorsport.com, 2016 radio ban analysis: reputable outlet. 
- Autosport, FIA abandons plans to restrict radio: reputable outlet.
- FIA Technical Regulations 2014, earlier issue on argent.fia.com (cover reads 14 July 2011, 77 pages): FIA host, searched in full, but an early issue and not the 2014 version. It gives the same Article 8.5.2 and 8.7 wording as 2015. Cite the 23-01-2014 version instead.
- FIA Technical Regulations 2016, copy on zonef1.com: third-party site, not the FIA. Its cover date (27 February 2016), page count (90) and Article 8.5 text match the 2016 file searched in full. It was not compared page by page.
- Wikipedia season pages: good for line-ups and calendars. Cross-check once against Formula1.com results.
- Wikipedia race pages and f1-fansite.com results pages: used to label each race wet or dry. Wikipedia is open to anyone to edit, so each label rests on one source.
- F1 Oversteer: secondary feature, no date. Used only for the current formation-lap rule. Check the 2026 regulations.

### Weak or discarded

- Reddit wet-race list: weak. Used as the first list only. Every race was then checked against its race page.
- f1briefing.com: discarded. It contradicts the FIA's 2016 statement and what I hear on the radio.

## Links

### Regulations and rules

- FIA 2014 Sporting Regulations: https://www.fia.com/sites/default/files/regulation/file/1-2014%20SPORTING%20REGULATIONS%202014-02-28.pdf
- FIA 2015 Sporting Regulations (03-12-2014 version): https://www.fia.com/sites/default/files/regulation/file/2015%20SPORTING%20REGULATIONS%202014-12-03.pdf
- FIA 2016 Sporting Regulations (20-04-2016 version): https://www.fia.com/files/2016-f1-sporting-regulations-published-200416pdf
- FIA 2014 Technical Regulations (23-01-2014 version): https://www.fia.com/sites/default/files/regulation/file/1-2014%20TECHNICAL%20REGULATIONS%202014-01-23_0.pdf
- FIA 2014 Technical Regulations, earlier issue (cover reads 14 July 2011): https://argent.fia.com/web/fia-public.nsf/A0425C3A0A7D69C0C12578D3002EBECA/$FILE/2014_F1_TECHNICAL_REGULATIONS_-_Published_on_20.07.pdf
- FIA 2015 Technical Regulations (29-06-2014 version): https://www.fia.com/sites/default/files/regulation/file/1-2015%20TECHNICAL%20REGULATIONS%202014-06-29.pdf
- 2016 Technical Regulations (27-02-2016 version, copy on zonef1.com, not the FIA): https://www.zonef1.com/saisons/2016/reglement_technique16_eng.pdf
- Cambridge 9980 syllabus 2023 to 2025: https://www.cambridgeinternational.org/Images/608552-2023-2025-syllabus.pdf
- Cambridge samples database (submission dates): www.cambridgeinternational.org/samples
- UCAS QIP page: https://qips.ucas.com/qip/cambridge-international-project-qualification

### The radio ban

- Directive, 11-09-2014: https://www.formula1.com/en/latest/article/fia-to-limit-radio-transmissions-on-car-performance.4cbQkTbahAJbGozBsegAs4
- Revised to driver performance only: https://www.formula1.com/en/latest/headlines/2014/9/FIA-revises-radio-ban-to-driver-performance-only.html
- RaceFans, FIA to restrict team radio messages (11-09-2014): https://www.racefans.net/2014/09/11/fia-restrict-team-radio-messages-next-race/
- Formula1.com, FIA clarifies radio transmission restrictions (16-09-2014): https://www.formula1.com/en/latest/article/fia-clarifies-radio-transmission-restrictions.4uSbLsruNnnmXXDqUjh7yV
- Abu Dhabi 2014 press conference (Horner and Wolff): https://www.fia.com/news/2014-abu-dhabi-grand-prix-thursday-press-conference
- Autosport, FIA abandons plans to further restrict radio: https://www.autosport.com/f1/news/fia-abandons-plans-to-further-restrict-formula-1-radio-information-5009856/5009856/
- Motorsport.com, full scope of the 2016 radio ban: https://www.motorsport.com/f1/news/analysis-the-full-scope-of-f1-s-2016-radio-ban-677934/677934/
- RaceFans, radio ban lifted (28-07-2016): https://www.racefans.net/2016/07/28/radio-ban-lifted-races/
- F1 Oversteer, the 2016 radio rule: https://www.f1oversteer.com/features/the-bizarre-f1-rule-that-was-brought-in-for-12-races-and-then-scrapped/
- Found but not read: Autosport, radio restrictions lifted from German GP: https://www.autosport.com/f1/news/formula-1s-radio-restrictions-to-be-lifted-from-german-gp-5039652/5039652/
- Found but not read: Motorsport.com, common sense prevails as F1 abandons radio ban rules: https://www.motorsport.com/f1/news/common-sense-prevails-as-f1-abandons-complex-radio-ban-rules/3222387/

### Seasons and line-ups

- 2013 season: https://en.wikipedia.org/wiki/2013_Formula_One_World_Championship
- 2014 season: https://en.wikipedia.org/wiki/2014_Formula_One_World_Championship
- 2014 Singapore Grand Prix: https://en.wikipedia.org/wiki/2014_Singapore_Grand_Prix
- 2015 season: https://en.wikipedia.org/wiki/2015_Formula_One_World_Championship
- 2016 season: https://en.wikipedia.org/wiki/2016_Formula_One_World_Championship

### Wet and dry check, race pages

- 2014 Australian GP, dry: https://www.f1-fansite.com/f1-result/race-result-2014-australian-f1-gp/
- 2014 Malaysian GP, dry: https://www.f1-fansite.com/f1-result/race-result-2014-malaysian-f1-gp/
- 2014 Bahrain GP, dry: https://en.wikipedia.org/wiki/2014_Bahrain_Grand_Prix
- 2014 Chinese GP, dry: https://en.wikipedia.org/wiki/2014_Chinese_Grand_Prix
- 2014 Spanish GP, dry: https://en.wikipedia.org/wiki/2014_Spanish_Grand_Prix
- 2014 Monaco GP, dry: https://en.wikipedia.org/wiki/2014_Monaco_Grand_Prix
- 2014 Canadian GP, dry: https://en.wikipedia.org/wiki/2014_Canadian_Grand_Prix
- 2014 Austrian GP, dry: https://en.wikipedia.org/wiki/2014_Austrian_Grand_Prix
- 2014 British GP, dry: https://en.wikipedia.org/wiki/2014_British_Grand_Prix
- 2014 German GP, dry: https://en.wikipedia.org/wiki/2014_German_Grand_Prix
- 2014 Hungarian GP, wet: https://en.wikipedia.org/wiki/2014_Hungarian_Grand_Prix
- 2014 Belgian GP, dry: https://en.wikipedia.org/wiki/2014_Belgian_Grand_Prix
- 2014 Italian GP, dry: https://en.wikipedia.org/wiki/2014_Italian_Grand_Prix
- 2014 Singapore GP, dry: https://en.wikipedia.org/wiki/2014_Singapore_Grand_Prix
- 2014 Japanese GP, wet: https://en.wikipedia.org/wiki/2014_Japanese_Grand_Prix
- 2014 Russian GP, dry: https://en.wikipedia.org/wiki/2014_Russian_Grand_Prix
- 2014 United States GP, dry: https://en.wikipedia.org/wiki/2014_United_States_Grand_Prix
- 2014 Brazilian GP, dry: https://en.wikipedia.org/wiki/2014_Brazilian_Grand_Prix
- 2014 Abu Dhabi GP, dry: https://en.wikipedia.org/wiki/2014_Abu_Dhabi_Grand_Prix
- 2015 Australian GP, dry: https://en.wikipedia.org/wiki/2015_Australian_Grand_Prix
- 2015 Malaysian GP, dry: https://en.wikipedia.org/wiki/2015_Malaysian_Grand_Prix
- 2015 Chinese GP, dry: https://en.wikipedia.org/wiki/2015_Chinese_Grand_Prix
- 2015 Bahrain GP, dry: https://en.wikipedia.org/wiki/2015_Bahrain_Grand_Prix
- 2015 Spanish GP, dry: https://en.wikipedia.org/wiki/2015_Spanish_Grand_Prix
- 2015 Monaco GP, dry: https://en.wikipedia.org/wiki/2015_Monaco_Grand_Prix
- 2015 Canadian GP, dry: https://en.wikipedia.org/wiki/2015_Canadian_Grand_Prix
- 2015 Austrian GP, dry: https://en.wikipedia.org/wiki/2015_Austrian_Grand_Prix
- 2015 British GP, wet: https://en.wikipedia.org/wiki/2015_British_Grand_Prix
- 2015 Hungarian GP, dry: https://en.wikipedia.org/wiki/2015_Hungarian_Grand_Prix
- 2015 Belgian GP, dry: https://en.wikipedia.org/wiki/2015_Belgian_Grand_Prix
- 2015 Italian GP, dry: https://en.wikipedia.org/wiki/2015_Italian_Grand_Prix
- 2015 Singapore GP, dry: https://en.wikipedia.org/wiki/2015_Singapore_Grand_Prix
- 2015 Japanese GP, dry: https://en.wikipedia.org/wiki/2015_Japanese_Grand_Prix
- 2015 Russian GP, dry: https://en.wikipedia.org/wiki/2015_Russian_Grand_Prix
- 2015 United States GP, wet: https://en.wikipedia.org/wiki/2015_United_States_Grand_Prix
- 2015 Mexican GP, dry: https://en.wikipedia.org/wiki/2015_Mexican_Grand_Prix
- 2015 Brazilian GP, dry: https://en.wikipedia.org/wiki/2015_Brazilian_Grand_Prix
- 2015 Abu Dhabi GP, dry: https://en.wikipedia.org/wiki/2015_Abu_Dhabi_Grand_Prix
- 2016 Australian GP, dry: https://en.wikipedia.org/wiki/2016_Australian_Grand_Prix
- 2016 Bahrain GP, dry: https://en.wikipedia.org/wiki/2016_Bahrain_Grand_Prix
- 2016 Chinese GP, dry: https://en.wikipedia.org/wiki/2016_Chinese_Grand_Prix
- 2016 Russian GP, dry: https://en.wikipedia.org/wiki/2016_Russian_Grand_Prix
- 2016 Spanish GP, dry: https://en.wikipedia.org/wiki/2016_Spanish_Grand_Prix
- 2016 Monaco GP, wet: https://en.wikipedia.org/wiki/2016_Monaco_Grand_Prix
- 2016 Canadian GP, dry: https://en.wikipedia.org/wiki/2016_Canadian_Grand_Prix
- 2016 European GP, dry: https://en.wikipedia.org/wiki/2016_European_Grand_Prix
- 2016 Austrian GP, dry: https://en.wikipedia.org/wiki/2016_Austrian_Grand_Prix
- 2016 British GP, wet: https://en.wikipedia.org/wiki/2016_British_Grand_Prix
- 2016 Hungarian GP, dry: https://en.wikipedia.org/wiki/2016_Hungarian_Grand_Prix
- 2016 German GP, dry: https://en.wikipedia.org/wiki/2016_German_Grand_Prix
- 2016 Belgian GP, dry: https://en.wikipedia.org/wiki/2016_Belgian_Grand_Prix
- 2016 Italian GP, dry: https://en.wikipedia.org/wiki/2016_Italian_Grand_Prix
- 2016 Singapore GP, dry: https://en.wikipedia.org/wiki/2016_Singapore_Grand_Prix
- 2016 Malaysian GP, dry: https://en.wikipedia.org/wiki/2016_Malaysian_Grand_Prix
- 2016 Japanese GP, dry: https://en.wikipedia.org/wiki/2016_Japanese_Grand_Prix
- 2016 United States GP, dry: https://en.wikipedia.org/wiki/2016_United_States_Grand_Prix
- 2016 Mexican GP, dry: https://en.wikipedia.org/wiki/2016_Mexican_Grand_Prix
- 2016 Brazilian GP, wet: https://en.wikipedia.org/wiki/2016_Brazilian_Grand_Prix
- 2016 Abu Dhabi GP, dry: https://en.wikipedia.org/wiki/2016_Abu_Dhabi_Grand_Prix

### Data

- FastF1 documentation: https://docs.fastf1.dev/fastf1.html
- Jolpica laps endpoint: https://github.com/jolpica/jolpica-f1/blob/main/docs/endpoints/laps.md
- Jolpica repository: https://github.com/jolpica/jolpica-f1
- Wet-race list (weak source, verify): https://www.reddit.com/r/formula1/comments/g0plkr/list_of_wet_weather_races_and_wins_by_driver/




ran smoke test: 

import json
import pathlib
import time
import urllib.error
import urllib.request

BASE = "https://api.jolpi.ca/ergast/f1"
SEASON, ROUND = 2014, 1
DRIVERS = ["rosberg", "hamilton", "massa", "bottas", "perez", "hulkenberg"]
OUT = pathlib.Path("raw")
OUT.mkdir(exist_ok=True)
calls = 0


def get(path, name):
    """One request. Stops the whole script on any error, including HTTP 429."""
    global calls
    time.sleep(0.6)
    url = f"{BASE}/{path}"
    req = urllib.request.Request(url, headers={"User-Agent": "ipq-smoke-test"})
    calls += 1
    try:
        with urllib.request.urlopen(req, timeout=30) as resp:
            body = resp.read().decode("utf-8")
            status = resp.status
            headers = dict(resp.headers.items())
    except urllib.error.HTTPError as err:
        print(f"STOP: HTTP {err.code} for {url}")
        if err.code == 429:
            print("429 means throttled. Others on the same IP share the limit. Wait a few minutes and rerun.")
        raise SystemExit(1)
    except urllib.error.URLError as err:
        print(f"STOP: could not reach {url}: {err.reason}")
        raise SystemExit(1)
    (OUT / f"{name}.json").write_text(body, encoding="utf-8")
    print(f"{status} {url}")
    return json.loads(body)["MRData"], headers


def seconds(text):
    """Turn a lap time such as 1:30.559 into seconds."""
    if ":" in text:
        minutes, rest = text.split(":")
        return int(minutes) * 60 + float(rest)
    return float(text)


def first_race(data):
    races = data["RaceTable"]["Races"]
    return races[0] if races else None


print("== 1. Driver IDs for 2014 ==")
data, headers = get(f"{SEASON}/drivers.json?limit=100", f"drivers_{SEASON}")
ids = {d["driverId"] for d in data["DriverTable"]["Drivers"]}
for driver in DRIVERS:
    print(f"  {driver}: {'present' if driver in ids else 'MISSING'}")
extra = {k: v for k, v in headers.items() if k.lower().startswith(("x-", "retry", "ratelimit"))}
print("  rate limit headers:", extra if extra else "none shown")

print("== 2. Laps completed per the race results ==")
data, _ = get(f"{SEASON}/{ROUND}/results.json?limit=100", f"results_{SEASON}_{ROUND}")
race = first_race(data)
print("  race:", race["raceName"], "| result rows:", len(race["Results"]))
done = {r["Driver"]["driverId"]: int(r["laps"]) for r in race["Results"]}

print("== 3. Laps for each driver, one request per driver ==")
matches = 0
for driver in DRIVERS:
    data, _ = get(f"{SEASON}/{ROUND}/drivers/{driver}/laps.json?limit=100", f"laps_{SEASON}_{ROUND}_{driver}")
    race = first_race(data)
    laps = race["Laps"] if race else []
    numbers = [int(lap["number"]) for lap in laps]
    timings = [t for lap in laps for t in lap["Timings"]]
    expected = done.get(driver)
    contiguous = numbers == list(range(1, len(numbers) + 1))
    verdict = "MATCH" if expected == len(timings) and contiguous else "MISMATCH"
    matches += verdict == "MATCH"
    times = [seconds(t["time"]) for t in timings]
    shown = f"first {timings[0]['time']}, fastest {min(times):.3f}s" if timings else "no laps"
    print(f"  {driver}: {len(timings)} timings, results say {expected} laps, contiguous {contiguous}, {shown} -> {verdict}")
    if verdict == "MISMATCH" and numbers:
        missing = sorted(set(range(1, max(numbers) + 1)) - set(numbers))
        print(f"    missing lap numbers: {missing[:15]}")
print(f"  {matches} of {len(DRIVERS)} drivers match")

print("== 4. Page cap: all drivers, limit=1000 ==")
data, _ = get(f"{SEASON}/{ROUND}/laps.json?limit=1000", f"laps_{SEASON}_{ROUND}_all")
laps = first_race(data)["Laps"]
n_timings = sum(len(lap["Timings"]) for lap in laps)
cap = int(data["limit"])
print(f"  response limit = {cap} | total = {data['total']} | lap objects returned = {len(laps)} | timings returned = {n_timings}")
if n_timings == cap:
    print("  the limit counts timings (one driver's time on one lap)")
elif len(laps) == cap:
    print("  the limit counts laps (all drivers on one lap)")
else:
    print("  unit unclear: the cap did not bind. Read the numbers above.")

print("== 5. Pit stops ==")
data, _ = get(f"{SEASON}/{ROUND}/pitstops.json?limit=100", f"pitstops_{SEASON}_{ROUND}")
stops = first_race(data)["PitStops"]
print(f"  stops returned = {len(stops)} | total = {data['total']} | fields = {sorted(stops[0].keys()) if stops else 'none'}")

print(f"== Done: {calls} requests used. Raw responses are in ./{OUT} ==")

results:
== 1. Driver IDs for 2014 ==  
200 [https://api.jolpi.ca/ergast/f1/2014/drivers.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/drivers.json?limit=100)  
rosberg: present  
hamilton: present  
massa: present  
bottas: present  
perez: present  
hulkenberg: present  
rate limit headers: {'x-content-type-options': 'nosniff', 'x-frame-options': 'DENY'}  
== 2. Laps completed per the race results ==  
200 [https://api.jolpi.ca/ergast/f1/2014/1/results.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/results.json?limit=100)  
race: Australian Grand Prix | result rows: 22  
== 3. Laps for each driver, one request per driver ==  
200 [https://api.jolpi.ca/ergast/f1/2014/1/drivers/rosberg/laps.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/drivers/rosberg/laps.json?limit=100)  
rosberg: 57 timings, results say 57 laps, contiguous True, first 1:42.038, fastest 92.478s -> MATCH  
200 [https://api.jolpi.ca/ergast/f1/2014/1/drivers/hamilton/laps.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/drivers/hamilton/laps.json?limit=100)  
hamilton: 2 timings, results say 2 laps, contiguous True, first 1:46.128, fastest 106.128s -> MATCH  
200 [https://api.jolpi.ca/ergast/f1/2014/1/drivers/massa/laps.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/drivers/massa/laps.json?limit=100)  
massa: 1 timings, results say 0 laps, contiguous False, first 1:40.287, fastest 100.287s -> MISMATCH  
missing lap numbers: [1]  
200 [https://api.jolpi.ca/ergast/f1/2014/1/drivers/bottas/laps.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/drivers/bottas/laps.json?limit=100)  
bottas: 57 timings, results say 57 laps, contiguous True, first 1:49.766, fastest 92.616s -> MATCH  
200 [https://api.jolpi.ca/ergast/f1/2014/1/drivers/perez/laps.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/drivers/perez/laps.json?limit=100)  
perez: 57 timings, results say 57 laps, contiguous True, first 2:36.707, fastest 92.634s -> MATCH  
200 [https://api.jolpi.ca/ergast/f1/2014/1/drivers/hulkenberg/laps.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/drivers/hulkenberg/laps.json?limit=100)  
hulkenberg: 57 timings, results say 57 laps, contiguous True, first 1:46.986, fastest 92.568s -> MATCH  
5 of 6 drivers match  
== 4. Page cap: all drivers, limit=1000 ==  
200 [https://api.jolpi.ca/ergast/f1/2014/1/laps.json?limit=1000](https://api.jolpi.ca/ergast/f1/2014/1/laps.json?limit=1000)  
response limit = 100 | total = 951 | lap objects returned = 6 | timings returned = 100  
the limit counts timings (one driver's time on one lap)  
== 5. Pit stops ==  
200 [https://api.jolpi.ca/ergast/f1/2014/1/pitstops.json?limit=100](https://api.jolpi.ca/ergast/f1/2014/1/pitstops.json?limit=100)  
stops returned = 34 | total = 34 | fields = ['driverId', 'duration', 'lap', 'stop', 'time']  
== Done: 10 requests used. Raw responses are in ./raw ==

pull data py:

import json
import pathlib
import sys
import time
import urllib.error
import urllib.request

BASE = "https://api.jolpi.ca/ergast/f1"
OUT = pathlib.Path("raw")
OUT.mkdir(exist_ok=True)
DRIVERS = ["rosberg", "hamilton", "massa", "bottas", "perez", "hulkenberg"]
ROUNDS = {2014: 19, 2015: 19, 2016: 21}
WET_THROUGHOUT = {(2014, 15), (2016, 20)}  # Japan 2014, Brazil 2016
MIXED = {(2014, 11), (2015, 9), (2015, 16), (2016, 6), (2016, 10)}  # Hungary 2014, Britain 2015, USA 2015, Monaco 2016, Britain 2016
INCLUDE_MIXED = False  # set to True only for the optional check that keeps the 5 mixed races
MAX_NEW = 450
new_requests = 0


def stop(message):
    print(f"\nSTOP: {message}")
    print(f"New requests this run: {new_requests}. Files in ./raw are kept. Rerun to continue.")
    raise SystemExit(1)


def fetch(path, name):
    """Return the MRData for a path. Reads ./raw/name.json if it exists, otherwise requests it."""
    global new_requests
    file = OUT / f"{name}.json"
    if file.exists():
        return json.loads(file.read_text(encoding="utf-8"))["MRData"]
    if new_requests >= MAX_NEW:
        stop(f"reached {MAX_NEW} new requests this run.")
    time.sleep(0.6)  # stays under 4 requests per second
    url = f"{BASE}/{path}"
    req = urllib.request.Request(url, headers={"User-Agent": "ipq-pull"})
    new_requests += 1
    try:
        with urllib.request.urlopen(req, timeout=30) as resp:
            body = resp.read().decode("utf-8")
    except urllib.error.HTTPError as err:
        if err.code == 429:
            stop("HTTP 429, throttled. Wait at least 10 minutes. Others on the same IP share the limit.")
        stop(f"HTTP {err.code} for {url}")
    except urllib.error.URLError as err:
        stop(f"could not reach {url}: {err.reason}")
    file.write_text(body, encoding="utf-8")
    return json.loads(body)["MRData"]


def first_race(data):
    races = data["RaceTable"]["Races"]
    return races[0] if races else None


def pitstops(season, rnd):
    """All pit stops for a race, following pages of 100 if there are more."""
    stops, offset = [], 0
    while True:
        name = f"pitstops_{season}_{rnd}" + (f"_offset{offset}" if offset else "")
        data = fetch(f"{season}/{rnd}/pitstops.json?limit=100&offset={offset}", name)
        race = first_race(data)
        stops += race["PitStops"] if race else []
        offset += 100
        if offset >= int(data["total"]):
            return stops


skipped = WET_THROUGHOUT if INCLUDE_MIXED else WET_THROUGHOUT | MIXED
targets = [(s, r) for s in ROUNDS for r in range(1, ROUNDS[s] + 1) if (s, r) not in skipped]
print(f"{len(targets)} races to pull. Wet races skipped: {sorted(skipped)}")

report = []
problems = 0
for season, rnd in targets:
    before = new_requests
    results = first_race(fetch(f"{season}/{rnd}/results.json?limit=100", f"results_{season}_{rnd}"))
    done = {r["Driver"]["driverId"]: int(r["laps"]) for r in results["Results"]}
    for driver in DRIVERS:
        data = fetch(f"{season}/{rnd}/drivers/{driver}/laps.json?limit=100", f"laps_{season}_{rnd}_{driver}")
        if int(data["total"]) > 100:
            stop(f"{driver} {season} round {rnd} has {data['total']} timings, more than one page. Page it before continuing.")
        race = first_race(data)
        laps = race["Laps"] if race else []
        numbers = [int(lap["number"]) for lap in laps]
        timings = sum(len(lap["Timings"]) for lap in laps)
        expected = done.get(driver)
        contiguous = numbers == list(range(1, len(numbers) + 1))
        if expected is None:
            problems += 1
            report.append(f"{season} R{rnd} {results['raceName']}: {driver} is not in the results")
        elif expected != timings or not contiguous:
            problems += 1
            missing = sorted(set(range(1, max(numbers, default=0) + 1)) - set(numbers))
            report.append(f"{season} R{rnd} {results['raceName']}: {driver} has {timings} timings, results say {expected} laps, missing lap numbers {missing[:10]}")
    stops = pitstops(season, rnd)
    print(f"{season} R{rnd} {results['raceName']}: {len(stops)} pit stops, {new_requests - before} new requests (run total {new_requests})")

summary = f"{len(targets)} races checked, {problems} problems, {new_requests} new requests this run."
(pathlib.Path("pull_report.txt")).write_text("\n".join(report + [summary]) + "\n", encoding="utf-8")
print("\n" + "\n".join(report))
print(f"\nDone: {summary} Details in pull_report.txt")