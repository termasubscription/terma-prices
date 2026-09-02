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
