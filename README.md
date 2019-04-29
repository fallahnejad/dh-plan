# DH-Plan Model
In this repository I provide explanation on DH-Plan model.
The Hotmaps district heating (DH) model is used for prefeasibility studies of DH grid investments and determination of economic DH areas on regional, national or European scale. Depending on the study area and input parameters, the model may suggest having one, two or more separated DH grids. The model is fully automatized and generates reports in various forms. The model is provided with the Hotmaps open data sets , which can assist users in preparation of required input data. Figure [1](*Fig. 1) shows the simplified structure of the model.

Fig. 1

## High performance
For the estimation of distribution grid costs, the concept of effective width  has been used. This allows the estimation of distribution grid related parameters such as linear heat density in a fast and efficient manner. By applying innovative mathematical approaches on raster data, the model finds coherent areas  swiftly. The coherent areas can be later on used for estimation DH potential or for determination of economic district heating grids. Figure XXXXXXXX shows how the specific distribution grid cost affects DH potential and its share from total useful energy demand in two different scenarios for DH market share.

Fig. 2


## High spatial resolution
The default data set fed into the model has spatial resolution of 100x100m. Figure XXXXXXXX shows a cut of the heat density map for the city of Brasov in Romania. Based on this map and plot ratio map, the coherent areas are determined.


Fig. 3


Street routes are obtained from Open Street Map . First, all un-drivable roads, service roads and private ways are filtered out. The remaining routes are fed to the optimization package and subsequently, the most economic routes for transmission lines are obtained. Figure XXXXXXXX illustrates the simplified representation of transmission lines with their heat flow direction and required capacity. Figure XXXXXXXX, on the other hand, shows the street routes used for the DH transmission grids.


## Determination of economic heat sources
All heat sources (conventional, excess heat, etc.) are analyzed not only based on their running costs, but also based on their location and required investment for constructing transmission pipeline from the heat source to demand zones. 

## Model Limitation
It is assumed that all supply sources supply heat throughout the year and at the same temperature level. The suggested transmission line routes are suitable for the prefeasibility studies and require additional in-situ studies. Pipeline dimensions are variables with discrete values and cost more CPU time for optimization. Therefore, it is recommended to run the model for problems with less than 200 coherent areas. For larger problems, the model should be run in relaxed mode, in which pipeline dimensions are considered as variables with positive real values.
