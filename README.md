Archival data for geoBoundaries 2.0.1

Version 2.0.1; Released 3/4/2020
- No new boundary information in this build; technical fixes only.
- Minor fixes to zipfile builds (https://github.com/wmgeolab/gbRelease/issues/1)
- API has been rewritten in PHP to facilitate python calls.  This now works:
import requests
r = requests.get('https://www.geoboundaries.org/gbRequest.html?ISO=USA&ADM=ADM1')
r.json()
- API now supports wildcard "ALL" for ADM, ISO or both.  Requesting ALL / ALL gives you a json with download links for all data in the database.
- The website now links to this changelog.

Version 2.0.0 ('Temerant'); Released 12/7/2019
- A little late, but a big update!
- New schema adopted to guarantee cross-boundary unique IDs across all versions of geoBoundaries.
- New topology checks in place (Shapely)
- Standardized geoJson and Shapefile builds for each ADM.
- Standardized attribute tables.
- Dramatically improved coverage (ADM0 and AMD 1 for 100% of countries; 79% of ADM2)
- Standardization of acceptable licenses; full license checks in place.
- Buildtime checks that all sources are valid and accessible.
- New API!  https://www.geoboundaries.org/gbRequest.html?ISO=[3-LETTER-ISO-CODE]&ADM=[ADM-LEVEL]
- New website! http://www.geoboundaries.org
- All code is now on github - https://github.com/wmgeolab/gbRelease.
