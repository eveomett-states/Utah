# License
This data was generated using data from the Redistricting Data Hub.  Any use of this project shall also comply with restrictions on use of data and attribution requirements set forth in the Redistricting Data Hub terms and conditions found at: [https://redistrictingdatahub.org/terms-and-conditions/](https://redistrictingdatahub.org/terms-and-conditions/).

Use of this project is further governed by the terms of the [Creative Commons Attribution Noncommercial 4.0 International](https://creativecommons.org/licenses/by-nc/4.0/legalcode.en)

# Utah Json and Shapefile

This shapefile was processed by Professor Ellen Veomett and her students Arbie Hsu and Alusi, using the corresponding jupyter notebook. As part of the cleaning process, precincts were nested within counties and small rook adjacencies (under 30.5 m) were changed to queen adjacencies.

# **Sources**
@author: eveomett AI for Redistricting, USF All data retrieved 05/31/24:

Obtain the following data from Restricting Data Hub

[Population data](https://redistrictingdatahub.org/dataset/Utah-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2021-utah-cong-adopted-plan/): 2021 Utah Congressional Districts plan enacted on 12/7/21.

[State House District data](https://redistrictingdatahub.org/dataset/2021-utah-state-house-adopted-plan/): 2021 State House Approved Plan

[State Senate District data](https://redistrictingdatahub.org/dataset/2021-utah-state-senate-adopted-plan/): 2021 State Senate Approved Plan

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-utah-precinct-boundaries-and-election-results-shapefile/)**:**  VEST 2020 Utah precinct and election results

[2020 county data](https://redistrictingdatahub.org/dataset/utah-county-pl-94171-2020/)  from 2020 Census Redistricting Data (P.L. 94-171) Shapefiles

We attempted to incorporate the following data, but were unable to sufficiently clean them:[2018 election data](https://redistrictingdatahub.org/dataset/vest-2018-utah-precinct-and-election-results/) from VEST, [2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-utah-precinct-and-election-results/) from VEST, [2016 election data](https://redistrictingdatahub.org/dataset/mggg-utah-precincts-and-election-results/) from MGGG.

# **Processing**

Data were cleaned and aggregated in the corresponding jupyter notebook using MGGG’s python library [maup](https://github.com/mggg/maup).

## Metadata
- `CountyID20`: County ID
- `resultspre20`: string giving what we believe is the precinct name
- `vistapre20`: string giving what we believe is the precinct ID
- `CD`: Congressional district ID in 2021 enacted congressional map
- `SEND`: State Senate district for 2021 State Senate Adopted Plan
- `HDIST`: State House district for 2021 State House of Representatives Districts Plan
- `TOTPOP`: Total population in 2020 Census
- `NH_WHITE`: White, non-hispanic, population in 2020 Census
- `NH_BLACK`: Black, non-hispanic, population in 2020 Census
- `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population in 2020 Census
- `NH_ASIAN`: Asian, non-hispanic, population in 2020 Census
- `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population in 2020 Census
- `NH_OTHER`: Other race, non-hispanic, population in 2020 Census
- `NH_2MORE`: Two or more races, non-hispanic, population in 2020 Census
- `HISP`: Hispanic population in 2020 Census
- `H_WHITE`: White, hispanic, population in 2020 Census
- `H_BLACK`: Black, hispanic, population in 2020 Census
- `H_AMIN`: American Indian and Alaska Native, hispanic, population in 2020 Census
- `H_ASIAN`: Asian, hispanic, population in 2020 Census
- `H_NHPI`: Native Hawaiian and Pacific Islander, hispanic, population in 2020 Census
- `H_OTHER`: Other race, hispanic, population in 2020 Census
- `H_2MORE`: Two or more races, hispanic, population in 2020 Census
- `VAP`: Total voting age population in 2020 Census
- `HVAP`: Hispanic voting age population in 2020 Census
- `WVAP`: White, non-hispanic, voting age population in 2020 Census
- `BVAP`: Black, non-hispanic, voting age population in 2020 Census
- `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population in 2020 Census
- `ASIANVAP`: Asian, non-hispanic, voting age population in 2020 Census
- `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population in 2020 Census
- `OTHERVAP`: Other race, non-hispanic, voting age population in 2020 Census
- `2MOREVAP`: Two or more races, non-hispanic, voting age population in 2020 Census
- `ATG20D`: Number of votes for 2020 Democratic attorney general candidate
- `ATG20R`: Number of votes for 2020 Republican attorney general candidate
- `ATG20O`: Number of votes for 2020 other party's attorney general candidate
- `AUD20D`: Number of votes for 2020 Democratic Auditor candidate
- `AUD20R`: Number of votes for 2020 Republican Auditor candidate
- `GOV20D`: Number of votes for 2020 Democratic gubernatorial candidate
- `GOV20R`: Number of votes for 2020 Republican gubernatorial candidate
- `GOV20O`: Number of votes for 2020 other party's gubernatorial candidate
- `PRE20D`: Number of votes for 2020 Democratic Presidential candidate
- `PRE20R`: Number of votes for 2020 Republican Presidential candidate
- `PRE20O`: Number of votes for 2020 other party's  Presidential candidate
- `TRE18R`: Number of votes for 2018 Republican Treasurer candidate
- `TRE18O`: Number of votes for 2018 other party's Treasurer candidate
