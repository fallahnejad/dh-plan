# DH-Plan Model

In this repository I provide explanation on DH-Plan model.
The DH-Plan model is used for prefeasibility studies of DH grid investments and determination of economic DH areas on regional, national or European scale. Depending on the study area and input parameters, the model may suggest having one, two or more separated DH grids. The model is fully automatized and generates reports in various forms. The model can use the [Hotmaps open data sets](https://www.hotmaps-project.eu/wp-content/uploads/2018/03/D2.3-Hotmaps_for-upload_revised-final_.pdf), which can assist users in preparation of required input data. Figure 1 shows the simplified structure of the DH-Plan model.

![Fig. 1 Simplified structure of DH-Plan model](https://github.com/fallahnejad/dh-plan/blob/master/images/simplified_structure_of_dh-plan.png "Simplified structure of DH-Plan model")

## High performance
For the estimation of distribution grid costs, the concept of effective width  has been used. This allows the estimation of distribution grid related parameters such as linear heat density in a fast and efficient manner. By applying innovative mathematical approaches on raster data, the model finds coherent areas  swiftly. The coherent areas can be later on used for estimation DH potential or for determination of economic district heating grids. Figure 2 shows how the specific distribution grid cost affects DH potential and its share from total useful energy demand in two different scenarios for DH market share.

![Fig. 2 Potentials for district heating in EU-28](https://github.com/fallahnejad/dh-plan/blob/master/images/potentials_for_district_heating_EU-28.png "potentials_for_district_heating_EU-28")


## High spatial resolution
The default data set fed into the model has spatial resolution of 100x100m. Figure 3 shows a cut of the heat density map for the city of Brasov in Romania. Based on this map and plot ratio map, the coherent areas are determined.


![Fig. 3 Heat density map](https://github.com/fallahnejad/dh-plan/blob/master/images/heat_density_map.png "Heat density map")


Street routes are obtained from [Open Street Map](www.openstreetmap.org). First, all un-drivable roads, service roads and private ways are filtered out. The remaining routes are fed to the optimization package and subsequently, the most economic routes for transmission lines are obtained. Figure 4.a illustrates the simplified representation of transmission lines with their heat flow direction and required capacity. Figure 4.b, on the other hand, shows the street routes used for the DH transmission grids.

![Fig. 4 Transmission lines (a) simplified representation; (b) street routes used.](https://github.com/fallahnejad/dh-plan/blob/master/images/Transmission_lines.png "Transmission lines (a) simplified representation; (b) street routes used.")



## Determination of economic heat sources
All heat sources (conventional, excess heat, etc.) are analyzed not only based on their running costs, but also based on their location and required investment for constructing transmission pipeline from the heat source to demand zones. 


## Model Limitation
It is assumed that all supply sources supply heat throughout the year and at the same temperature level. The suggested transmission line routes are suitable for the prefeasibility studies and require additional in-situ studies. Pipeline dimensions are variables with discrete values and cost more CPU time for optimization. Therefore, it is recommended to run the model for problems with less than 200 coherent areas. For larger problems, the model should be run in relaxed mode, in which pipeline dimensions are considered as variables with positive real values.


# LICENSE
Copyright 2019 Mostafa Fallahnejad

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.