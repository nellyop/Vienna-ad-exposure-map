# Vienna-ad-exposure-map
The dataset Advertisement_in_Vienna_8_Dataset.geojson includes 837 Points of different ad-vertisement types, categories, conditions, areas and heights. These points are referenced in EPSG:3857 – WGS84 / Pseudo-Mercator and have a timestamp. 
The background and motivation behind the dataset is that we wanted to capture outdoor advertising, as it is an element of contemporary urban environments and influences our perception of space, either directly or indirectly. While research exists on the effect of advertisement in public spaces exist, detailed spatial datasets describing the distribution and characteristics of advertisements are rare. The lack of openly available advertising datasets limits research on visual exposure, urban aesthetics, consumer behavior, and advertisement-aware navigation. Therefore this dataset provides a detailed, georeferenced inventory of outdoor advertisements within Vienna's 8th district (Josefstadt). The dataset enables the investigation of how advertising is distributed in urban space, and how advertisement information can be integrated into route planning applications.
The dataset contains a collection of outdoor advertisements recorded through field observa-tions in Vienna's 8th district. Each advertisement was georeferenced and documented using a standardized survey protocol, which can be seen in the appendix. The dataset consists of individual advertisement locations represented as point features and includes information about advertisement type, thematic category, physical condition, area (in square meters), height (in meters), time of recording and geographic coordinates. The recorded advertisement types include billboards, posters, digital screens, shop window advertisements, banners, stickers, con-struction fence advertisements, advertising columns, and other forms of outdoor advertising. Advertisement content was classified into categories such as food and beverage, retail, fashion, entertainment, services, tourism, education, political campaigns, tobacco, beverages, and bet-ting. The resulting dataset provides a detailed structure of the advertising landscape within the study area and can be used for spatial analysis, visualization, machine learning applications, and urban planning research.
Regarding the technical aspect, the dataset was collected through systematic field mapping and adheres to the principles of Volunteered Geographic Information. Firstly, the types, categories and conditions described above were set out in tabular form to facilitate the recording pro-cess. These were then transferred into a point layer as attributes in QGIS. In addition, the dis-trict boundaries of Vienna were imported from www.data.gv.at to ensure orientation within the survey area whilst in the field. This point and polygon layer was transferred to the field mapping tool Mergin Maps via the plugin in QGIS. In the field, every street in Josefstadt was systematically surveyed on 11 and 12 June 2026 in order to record as much of the advertising as possible in Mergin Maps. Following the survey, the data was synchronised and imported into QGIS, before being analysed as a CSV file in Jupyter Lab. This analysis involved data cleaning and exploratory data analysis. 

As a Use-Case of our Dataset we thought about the development of an advertisement-aware routing system. Traditional routing algorithms optimize routes according to distance, travel time, or accessibility. By integrating advertisement locations into the routing process, users can instead optimize routes according to advertisement exposure. For example, pedestrians could:  Minimize overall advertisement exposure, prioritize routes passing certain advertisement categories relevant for marketing analysis, study how advertising influences pedestrian movement and urban perception. Using the advertisement points together with street network data from Open-StreetMap, shortest-path algorithms can calculate routes while considering advertisement density and category preferences. Interactive dashboards can further allow users to dynamically select advertisement categories through checkboxes and immediately visualize their influ-ence on route selection. This demonstrates how a seemingly simple urban inventory can support applications in urban analytics, geocommunication, behavioral geography, and smart city research.

Appendix
Appendix 1: ad_type Encoding
Code	Description
1	Billboard
2	Poster
3	Digital Screen
4	Shop Window Advertisement
5	Banner
6	Sticker
7	Construction Fence Advertisement
8	Free-standing Advertising Column
9	Other

Appendix 2: ad_category Encoding
Code	Description
1	Food & Beverage
2	Retail / Shopping
3	Fashion
4	Entertainment / Culture
5	Services
6	Tourism
7	Real Estate
8	Education
9	Own advertising
91	Café
92	Grocery shop (from supermarkets to bakeries)
93	Tobacco shop
94	Clothing shop
95	Bank
96	Restaurants/Takeaways
97	Other
98	Betting
10	Political
11	Public Campaign
12	Tabacco
13	Drinks
131	Non-Alkoholic
132	Alkoholic
14	Other

Appendix 3: condition Encoding
Code	Description
1	Excellent / New
2	Good
3	Moderate Wear
4	Poor
5	Damaged

