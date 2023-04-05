# foe-city-layout

Sourced from Sacah's City Layout Tool on 4/17/2022.

View the site [Sacah's City Layout Tool](https://sacah.github.io/foe-city-layout/)

## Updating building data
1. Find last ID from src/data/buildingInfo.js
2. Edit updateBuildingInfo.html, update buildingId to the ID from step 1 + 1. This is the first ID assigned to the new buildings being imported
3. In FoE open DevTools -> Console and paste 'JSON.stringify(MainParser.CityEntities)'
4. Copy output into src/data/buildingInfoFull.js, paste inside the JSON.parse
5. Open updateBuildingInfo.html in a browser
6. Open DevTools -> Console, JSON.stringify(newBuildings)
7. Copy output, paste this into a text editor, delete the first and last ' & { }
8. Copy from editor, paste at the end of buildingInfo.js
9. Format the file

## Change log

### 4/5/2023
* Added buildings for GE5 and 11th anniversery event

### 3/24/2023
* added new buildings

### 1/10/2023
* added halloween 2022 and winter 2022 buildings
* note: process has stopped inmporting building dimensions, so have to edit them in manually - not sure why, perhaps a change by inno on the format of the string?

### 11/14/2022
* Began adding generic buildings. Named "Generic WxH." they can be added to a city, not imported, to take the place of new buildings that have not yet been added to the tool

### 10/12/2022
* Added Fall Event 2022 buildings 

### 09/21/2022
* Added Summer Event 2022 buildings 

### 05/11/2022
* Added color coding bsed on building type

### 3/02/2022
* Importing latest building data
* Adding npm command to serve for local testing

### 5/12/2021
* Importing latest building data

### 31/10/2021
* Importing latest building data
* Adjusting updateBuildingInfo to handle new FoE Data format

### 14/10/2021
* Implemented ability to Alt + Click to multiselect and drag

### 8/10/2021
* Importing latest building data
* Adjusting updateBuildingInfo to handle new FoE data format

### 17/08/2021
* Importing latest building data

### 25/07/2021
* Importing latest building data

### 7/06/2021
* Removed old import method, only option is FoE Helpers 'Copy citymap data' button in the 'Town overview' modal
* Imported latest building data

### 19/05/2021
* Imported latest building data
* Updated Readme with steps to update buildings
* Fixed handling of copied text, not sure if Chrome changed JSON output

### 12/04/2021
* Imported latest building data
* Allow the importing of FoE Helper - Your city - Copy citymap data

### 27/12/2020
* Imported latest building data

### 03/11/2020
* Imported latest building data

### 20/09/2020
* FoE Helper changed data structure of city data, import now works again

### 16/09/2020
* Imported latest building data

### 13/05/2020
* Importing latest building data

### 11/05/2020
* Pull cityData from current building layout, rather than imported cityData

### 09/05/2020
* Added a Share button, which generates a link that others can use to load your layout

### 24/04/2020
* Fixed Save/Load bug where buildings shifted 4 tiles
* Added link in Help for logging issues
* Added Google Analytics to get an idea of usage