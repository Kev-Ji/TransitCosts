# TransitCosts
An analysis of factors that affect the total cost of transit projects across the world.  
**Authors:** Kevin Ji, Sangey Rinchen, Blake Xu  

**Dataset Link**: https://github.com/rfordatascience/tidytuesday/blob/main/data/2021/2021-01-05/Merged%20Costs%20(1.0)%20-%20Sheet1.csv  
**Country Shapefile Source:** https://hub.arcgis.com/datasets/esri::world-countries-generalized  
**Country Categories**: https://datatopics.worldbank.org/sdgatlas/archive/2017/the-world-by-region.html  

### Data Dictionary

# `transit_cost.csv`

|variable         |class     |description |
|:----------------|:---------|:-----------|
|e                |double    | ID |
|Country          |character | Country Code - can be joined against `countrycode` via `ecb` or `iso2c` |
|City             |character | City where transit tunnel is being created |
|Line             |character | Line name or path |
|Start year       |character | Year started |
|End year         |character | Year ended (predicted or actual) |
|RR?               |double    | I think this is Railroad (0 or 1), where 1 == Railroad? |
|Length           |double    | Length of proposed line in km |
|TunnelPer       |character | Percent of line length completed |
|Tunnel           |double    | Tunnel length of line completed in km (can take this divided by length to get `tunnel_per`) |
|Stations         |double    | Number of stations where passengers can board/leave |
|Source1          |character | Where was data sourced |
|Cost             |double    | Cost in millions of local currency |
|Currency         |character | Currency type |
|Year             |double    | Midpoint year of construction |
|PPP rate         |double    | purchasing power parity (PPP), based on the midpoint of construction |
|Real cost        |character | Real cost in Millions of USD |
|Cost/km (millions) |double    | Cost/km in millions of USD |
|Source2          |character | Where was data sourced for cost |
|Reference        |character | Reference URL for source |

## TBD 

- Merge North America with Central America
- Merge South, North, and Western Europe
- Merge Northern Africa with Western Asia
- Merge Central Asia with Eastern Asia
- Merge Southeastern Asia with Australasia