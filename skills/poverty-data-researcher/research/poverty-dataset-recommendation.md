# Poverty Dataset Recommendation for Nethra Data Explorer

## Recommendation

Use the **World Bank Poverty and Equity Database / Poverty and Inequality Platform (PIP)** as the primary test dataset for Nethra Data Explorer.

Best reasons:

- it is an official poverty source from the World Bank
- it provides country-level poverty indicators
- it includes clear download formats and API access
- it covers a long time span
- it has enough structure to test import, schema detection, ontology discovery, visualization, and explainability

Source:

- [World Bank Data Catalog: Poverty and Equity Database (Poverty and Inequality Platform)](https://datacatalog.worldbank.org/search/dataset/0038020/poverty-and-equity-database-poverty-and-inequality-platform)

## Why This Dataset Fits the MVP

Nethra’s first MVP needs a dataset with:

- country/year structure
- multiple poverty indicators
- downloadable metadata
- clear source provenance
- enough comparability caveats to test explainability

PIP fits those needs well.

It includes:

- poverty headcount ratio
- poverty gap
- number of poor
- inequality indicators
- income or consumption distributions
- national, regional, and global estimates

Our World in Data confirms that its poverty explorer is adapted from the World Bank’s PIP and that comparability issues remain across countries and over time.

Sources:

- [Our World in Data: Poverty](https://ourworldindata.org/extreme-poverty)
- [Our World in Data: Poverty](https://ourworldindata.org/poverty)

## Likely Schema Shape

The first schema Nethra should expect is roughly:

- `country`
- `year`
- `poverty_line`
- `poverty_headcount`
- `poverty_gap`
- `number_of_poor`
- `region`
- `survey_type`
- `welfare_type`
- `coverage_flag`
- `comparability_flag`
- `source`

This is an inference from the source descriptions and OWID’s poverty pages, not a direct schema dump.

## Likely Ontology Seed Set

Start semantic tags with:

- entity.country
- time.year
- indicator.poverty_headcount
- indicator.poverty_gap
- indicator.number_of_poor
- indicator.income_distribution
- indicator.consumption_distribution
- dimension.poverty_line
- dimension.region
- dimension.survey_type
- unit.percent
- unit.people
- unit.international_dollars

## Suggested MVP Test Scenarios

1. Import a PIP-style CSV and confirm country/year detection.
2. Detect poverty indicators and map them to semantic tags.
3. Generate a line chart for one poverty measure across years.
4. Generate a comparison view for several countries.
5. Surface comparability caveats in the explanation panel.
6. Produce a short report that cites the data source and warns about survey comparability.

## Fallback Dataset

If the main PIP dataset is too broad for early testing, use an OWID poverty chart download based on the same source.

Good candidates:

- [Our World in Data: Poverty](https://ourworldindata.org/poverty)
- [Our World in Data: Extreme Poverty](https://ourworldindata.org/extreme-poverty)

These are useful for early product validation because they already package poverty data into chart-friendly formats.

## Caveats

- poverty definitions vary across countries
- income and consumption surveys are not directly identical
- comparability across time can be limited
- regional and global estimates may rely on harmonization and projection rules

Those caveats are actually useful for Nethra because they let us test explainability, confidence, and data-quality warnings.

## Best Initial Setup

For the first product test:

- use PIP as the primary source
- use OWID poverty pages as a fallback and comparison reference
- begin with country/year poverty headcount
- add poverty gap and number of poor as secondary indicators
- show comparability flags in the UI
- treat the source description as part of the ontology metadata

## Bottom Line

The best first poverty dataset for Nethra Data Explorer is the **World Bank PIP / Poverty and Equity Database**, with OWID poverty pages used as a practical fallback and reference for testable chart-shaped outputs.
