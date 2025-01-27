Miscellaneous Public Data Sets
================
Created by Bradley Setzler, Pennsylvania State University

[Prepared Miscellaneous data sets are located
here.](https://github.com/setzler/EconData/tree/master/DataRepo/Miscellaneous/)

Included files and functions include:

- `state_fips_crosswalk.csv`: Cross-walk from state FIPS to name of the
  state. When `getCZ()` function is run, it downloads and cleans the
  data from the USDA.

- `cz_crosswalk_2000.csv`: Cross-walk from county FIPS to 2000 commuting
  zone. When `getStateFips()` function is run, it downloads and cleans
  the data from the Census.

- `MianSufi2014_tradables.csv`: Tradable vs non-tradable industry
  classification from Mian and Sufi (2014, Econometrica). When
  `getTradables()` is run, it downloads and cleans the data from Sufi’s
  website.

- `distances/county_distance_100miles.csv`,
  `distances/CZ_distance_100miles.csv`, and
  `distances/state_distance_100miles.csv`: Using county-to-county
  distances of up to 100 miles, it forms the minimum distance between
  counties, commuting zones, and states, respectively. Any pairs not
  included are over 100 miles apart. When `getDistances()` is run, it
  downloads and cleans the distances from the [NBER data
  repository](https://data.nber.org/distance/2000/sf1/county/).

- `FRED_CPI.csv`: Total all items CPI from
  [FRED](https://fred.stlouisfed.org/series/CPALTT01USA661S) covering
  1960-2020, measured on January 1 of each year. When `getCPI()` is run,
  it downloads and cleans the CPI from the FED website.

- `BEA_GDP.csv`: Annual GDP from
  [BEA](https://apps.bea.gov/regional/downloadzip.cfm) covering
  1960-2020, measured on January 1 of each year. When `getGDP()` is run,
  it downloads and cleans the GDP from the BEA website, aggregating to
  the CZ by 2-digit NAICS level. Warning: BEA only reports NAICS
  supersectors, e.g., manufacturing codes 31-33 are grouped together and
  coded as 31.

- `sector_names.csv`: Names of NAICS sectors and supersectors from
  [BLS](https://www.bls.gov/sae/additional-resources/naics-supersectors-for-ces-program.htm).
  When `getSectorNames()` is run, it creates this file.
