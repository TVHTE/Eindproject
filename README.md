###### Minor programming, University of Amsterdam
###### Programmeerproject
###### 10556346
###### Raoul Lieben


# Proposal:

#### Problem Statement:

Not everyone is convinced if climate change is real and this could obstruct solving the problem. Especially with the U.S.
withdrawing from the Paris agreement it needs to be clear that this is a global issue and has to be addressed. An easy
interpretable, interactive graph with climate change data, could help people understand why the issue is urgent to
address and act on. This could benefit the individual as well as the global population.

#### Solution:
An interactive world map, showing graphs of greenhouse emissions (carbon-dioxide, methane and nitrous-oxide), energy use incl
renewable energy use, forest area and protected terrestial and marine areas.

(I already used renewable energy in a previous assignment as a scatterplot but now I want to use it as a line graph over time.
It is the same kind of data but an other interpretation and I use a lot more data now, so I assume that does not matter)

#### Main features:
- Interactive, clickable, coloured (colour defines the amount of emission) world map, with tooltip for how much greenhouse
emission, which triggers one out of these three graphs, selected by a dropdown menu (MVP):
    - Greenhouse emissions, with tooltip and checkbox for the kinds of emission (MVP)
    - Energy use, with tooltip and checkbox for renewable energy (MVP)
    - Forest area and protected terrestial and marine areas, with tooltip and checkbox which of the two has to be shown.

#### Data:
All data is from https://data.worldbank.org/. The data does not need to be transformed. 

#### External components:
- D3 library : "https://d3js.org/d3.v3.min.js"
- For world map : "https://d3js.org/d3.geo.projection.v0.min.js" and "https://d3js.org/topojson.v1.min.js"

#### Similar visualizations:
http://www.carbonmap.org/
The values are not in a graph but as an infobox and colour scheme on the map. The colour scheme is also possible for my
project, however an extra graph on the side will give more insight.
The map does not zoom in, this is difficult for selecting small countries. Some more info on the country is also nice to add,
for example population.

#### Hardest parts:
The hardest part is finding a way to correctly compare countries, maybe by showing two graphs of two selected countries.
Other difficulties are of sorting all data on all the countries. Linking data to the map and linking to an dropdown menu and
within a checkbox. 