# Skip list

Brand ids whose real-world pricing depends on a personal configurator (data bundle,
contract length, existing-customer-only rates, consumption profile, insurance profile,
etc.) rather than one clear published rate. Price checks should skip these without
re-researching every run.

- engie: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- luminus: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- mega: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- totalenergies: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- eneco: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- essent: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- vattenfall: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- greenchoice: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- budgetenergie: energy, `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- aginsurance: insurance, `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- axa: insurance, `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- vodafonenl: telecom (mobile) - vodafone.nl presents pricing through a duration/bundle configurator (query params like ?subscription=...&duration=24), no single flat list price found for "Red mobiel"; "Onbeperkt mobiel" price wasn't findable either
- lebara: telecom (mobile) - not a single pan-EU rate; per-country storefronts (lebara.nl, lebara.co.uk, ...) each run multiple tiers, e.g. NL SIM-only ranges roughly EUR 2-33.50/month depending on tier, so the catalog's single "all" EUR price doesn't correspond to one real rate
- patreon: creator platform, `varies: true` / empty price in catalog.ts - membership amount is set by each individual creator, no single published price
- azg: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- greenpeace: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- wwf: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- rodekruis: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- amnesty: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- unicef: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- savethechildren: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- oxfam: charity, `varies: true` / empty price in catalog.ts - monthly gift amount is donor-chosen, no fixed rate
- eon: energy (DE), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- enbw: energy (DE), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- yello: energy (DE), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- allianz: insurance (DE), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- hukcoburg: insurance (DE), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- tk: health insurance (DE), `varies: true` / empty price in catalog.ts - statutory contribution depends on income and employer split, no single published rate
- sparkasse: finance (DE), `varies: true` / empty price in catalog.ts - tariff differs per regional Sparkasse, no single published rate
- iberdrola: energy (ES), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- endesa: energy (ES), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- naturgy: energy (ES), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- mapfre: insurance (ES), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- mutuamadrilena: insurance (ES), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- sanitas: insurance (ES), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- britishgas: energy (GB), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- octopusenergy: energy (GB), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- ovoenergy: energy (GB), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- eonnext: energy (GB), `varies: true` / empty price in catalog.ts - rate depends on consumption profile and region, no single published tariff
- directline: insurance (GB), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- aviva: insurance (GB), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- bupa: insurance (GB), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- geico: insurance (US), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- progressive: insurance (US), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- statefarm: insurance (US), `varies: true` / empty price in catalog.ts - premium depends on personal risk profile, no single published rate
- skystream: streaming (GB) - Sky discontinued the "Entertainment" tier naming on Sky Stream; replaced with Essential TV / Ultimate TV, and the 31-day rolling rate is now heavily dependent on new-vs-existing-customer status and retention offers (reported roughly GBP 18-37/month across sources), no clean 1:1 mapping to the catalog's old plan ids or a single published rate
- puregym: sport (GB) - pricing is set per gym location; official material frames the GBP 17.99/22.99/28.99 figures as "from" prices only, with real per-location rates ranging roughly GBP 18-45
- gymgroup: sport (GB) - pricing is set per gym location; the Live It tier alone spans roughly GBP 24.99-34.99 depending on which club, no single national rate
- classpass: sport (US) - pricing varies by city/market (confirmed premium in markets like NYC vs elsewhere) and the credit-tier lineup has been restructured, no single national rate card to verify against
- verisure: housing (BE) - Verisure's own pricing guide states monitoring cost depends on home size, number of sensors/cameras, and a personalized security assessment, no single published rate
