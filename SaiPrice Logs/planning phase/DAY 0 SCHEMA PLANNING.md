The three specs columns, legal_status, interior, direction. Dropped as standalone fields. They're redundant with specs_raw and you don't know yet which of those keys the ML stage actually needs as inputs. Query specs_raw directly for now. Revisit as derived fields once you've seen real data and know what's worth pulling out.

specs_raw itself, JSONField versus a separate normalized table. Left as JSONField. The decision to normalize it depends on which spec values the ML model ends up needing as features, and you don't have that answer until you've scraped real listings and started building the model.

district and ward human readable names. You have the raw IDs required and guaranteed from pageTrackingData, but the name columns stay nullable until you build the ID to name lookup table. Not urgent, not blocking, just not done yet.

price_unit. Column exists but stays unused for now. Every batdongsan listing is VND total, no unit variation to store. This only earns its keep once maisonoffice enters Stretch scope with per sqm and per seat pricing.

property_type value office. Defined in the enum, not populated. Nothing in Standard scope is an office listing. It sits there so you don't need a migration when maisonoffice comes online.

phone_number. Column added at your call, but the scraping mechanism is deferred. The real number sits behind a KYC gated endpoint, which means a second network request per listing, not a free field off the page you're already pulling. That's a Jul 6 or later build problem, not something resolved on paper today.

vip_type. Included as optional, no decision made on whether you'll actually use it. It's there in pageTrackingData, cheap to store, unclear yet if it earns a place in the model.

That's seven open items. None of them block Jul 6. All of them are either waiting on real scraped data to make the call, or waiting on the maisonoffice Stretch scope to activate.
![[listing table schema plan pt1.png]]
![[listing table schema plan pt2.png]]