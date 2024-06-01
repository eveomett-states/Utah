# Utah Election Shapefile

This shapefile was processed by Professor Ellen Veomett and her student Ananya Agarwal.

# **Sources**
@author: eveomett AI for Redistricting, USF All data retrieved 05/31/24:

Obtain the following data from Restricting Data Hub

[Population data](https://redistrictingdatahub.org/dataset/Utah-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2021-utah-cong-adopted-plan/): 2021 Utah Congressional Districts plan enacted on 12/7/21.

[State House District data](https://redistrictingdatahub.org/dataset/2021-utah-state-house-adopted-plan/): 2021 State House Approved Plan

[State Senate District data](https://redistrictingdatahub.org/dataset/2021-utah-state-senate-adopted-plan/): 2021 State Senate Approved Plan

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-utah-precinct-boundaries-and-election-results-shapefile/)**:**  VEST 2020 Utah precinct and election results

[2018 election data](https://redistrictingdatahub.org/dataset/vest-2018-utah-precinct-and-election-results/)**:**  VEST 2018 Utah precinct and election results

[2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-utah-precinct-and-election-results/)**:**  VEST 2016 Utah precinct and election results

# **Processing**

Demographic data were aggregated from the census block level and precincts were assigned to districts using [MGGG's proration software](https://github.com/mggg/maup). Election data were also prorated onto VTDs from the original precinct shapefile using the `maup` package.

## Metadata
* `CountyID`: County ID
* `VistaID`: Precinct name and sub-precinct number
* `PrcncID`: Precinct name
* `SbPrcnc`: Sub-precinct number
* `AliasNm`: Municipality name (where applicable)
* `DsslvID`: Precinct unique identifier
* `cnty_nm`: County name
* `cnty_fp`: County FIPs code
* `jrsdctn`: Jurisdiction name
* `PRES16D`: Number of votes for 2016 Democratic presidential candidate 
* `PRES16R`: Number of votes for 2016 Republican presidential candidate 
* `PRES16I`: Number of votes for 2016 Independent presidential candidate (Evan McMullin)
* `SEN16D`: Number of votes for 2016 Democratic senate candidate 
* `SEN16R`: Number of votes for 2016 Republican senate candidate 
* `GOV16D`: Number of votes for 2016 Democratic gubernatorial candidate 
* `GOV16R`:  Number of votes for 2016 Republican gubernatorial candidate
* `TOTPOP`: Total population 
* `NH_WHITE`: White, non-hispanic, population
* `NH_BLACK`: Black, non-hispanic, population
* `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population
* `NH_ASIAN`: Asian, non-hispanic, population
* `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population
* `NH_OTHER`: Other race, non-hispanic, population
* `NH_2MORE`: Two or more races, non-hispanic, population
* `HISP`: Hispanic population
* `H_WHITE`: White, hispanic, population
* `H_BLACK`: Black, hispanic, population
* `H_AMIN`: American Indian and Alaska Native, hispanic, population
* `H_ASIAN`: Asian, hispanic, population
* `H_NHPI`: Native Hawaiian and Pacific Islander, hispanic, population
* `H_OTHER`: Other race, hispanic, population
* `H_2MORE`: Two or more races, hispanic, population
* `VAP`: Total voting age population
* `HVAP`: Hispanic voting age population
* `WVAP`: White, non-hispanic, voting age population
* `BVAP`: Black, non-hispanic, voting age population
* `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population
* `ASIANVAP`: Asian, non-hispanic, voting age population
* `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population
* `OTHERVAP`: Other race, non-hispanic, voting age population
* `2MOREVAP`: Two or more races, non-hispanic, voting age population
* `CD`: US congressional district ID
* `SENDIST`: State Senate district ID
* `HDIST`: State House district ID

## Projection
This shapefile uses a NAD83/UTM zone 12 North projection (EPSG:26912).
