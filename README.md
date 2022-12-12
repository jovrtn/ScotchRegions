# Scotch Whisky Region Map

## Regions

- Highlands
- Lowlands
- Speyside
- Islay
- Campbeltown

## Maps

- Combined: all regions as distinct features within a single file.
- Separate: Each region in separate files.
- Misc: For convenience, the boundary line between the Highlands and Lowlands is also provided separately.

**Note:** If all regions are displayed together, the full territory of Scotland will be visible, however the full Scotland territory is not provided as a single feature. If you require this, you can extract the region from the NUTS 1 UK regions map at the corresponding Full/Generalised/Super Generalised levels of detail described below.

## Quality Levels

- Full (Highest level of detail)
- Generalised (Moderate level of detail)
- Super Generalised (Lowest level of detail)

## The Scotch Whisky Regulations 2009

This data set was created using a close reading of the 2009 regulation text. The full law is available here: http://www.legislation.gov.uk/uksi/2009/2890/regulation/10/made

```
(5) The protected localities are—
    (a) “Campbeltown”, comprising the South Kintyre ward of the Argyll
        and Bute Council as that ward is constituted in the Argyll and
        Bute (Electoral Arrangements) Order 2006(1); and
    (b) “Islay”, comprising the Isle of Islay in Argyll.
(6) The protected regions are—
    (a) “Highland”, comprising that part of Scotland that is north of
        the line dividing the Highland region from the Lowland region;
    (b) “Lowland”, comprising that part of Scotland that is south of
        the line dividing the Highland region from the Lowland region; and
    (c) “Speyside”, comprising—
        (i) the wards of Buckie, Elgin City North, Elgin City South,
        Fochabers Lhanbryde, Forres, Heldon and Laich, Keith and Cullen
        and Speyside Glenlivet of the Moray Council as those wards are
        constituted in the Moray (Electoral Arrangements) Order 2006(2); and
        (ii) the Badenoch and Strathspey ward of the Highland Council as
        that ward is constituted in the Highland (Electoral Arrangements)
        Order 2006(3).
(7) In this regulation “the line dividing the Highland region from the
    Lowland region” means the line beginning at the North Channel and
    running along the southern foreshore of the Firth of Clyde to Greenock,
    and from there to Cardross Station, then eastwards in a straight line
    to the summit of Earl’s Seat in the Campsie Fells, and then eastwards
    in a straight line to the Wallace Monument, and from there eastwards
    along the line of the B998 and A91 roads until the A91 meets the M90
    road at Milnathort, and then along the M90 northwards until the Bridge
    of Earn, and then along the River Earn until its confluence with the
    River Tay, and then along the southern foreshore of that river and the
    Firth of Tay until it comes to the North Sea.

--------

(1) S.S.I. 2006/378. [http://www.legislation.gov.uk/ssi/2006/378/contents/made]
(2) S.S.I. 2006/372. [http://www.legislation.gov.uk/ssi/2006/372/contents/made]
(3) S.S.I. 2006/481. [http://www.legislation.gov.uk/ssi/2006/481/contents/made]
```

## Assumptions

The 2009 regulations lack sufficient clarity to precisely chart the boundary between the "Highlands" and "Lowlands" regions, therefore several assumptions have been made to facilitate map creation.

| Description  | Coordinates | Notes |
| ------------- | ------------- | ------------- |
| The western end of the Highlands/Lowlands dividing line is determined using the boundaries of the 'the Scottish marine region for the Clyde'[1] as defined in Scottish Marine Regions Order 2015, specifically the point at which the boundary meets the shoreline in the southwest of the Firth of Clyde. | Lat/Lng  | Though not mentioned in the Scotch Whisky Regulations 2009, this seemed the most authoritative way to determine a point at which the North Channel and the Firth of Clyde can be said to 'meet' at the shoreline. |
| Greenock is defined as its geographical center. | Lat/Lng | |
| Cardross Station is defined as its geographical center. | Lat/Lng | |
| The summit of Earl's Seat is defined as its geographical center. | Lat/Lng | |
| The Wallace Monument is defined as its geographical center. | Lat/Lng | |
| The line segment between the Wallace Monument and the B998 roadway takes a very literal approach and snaps directly north to B998 rather than a more organic line from the monument to some arbitrary eastern point along B998. | Lat/Lng | |
| For roadways, the line contour follows the *northern* curvature of any roundabouts—the same direction an automobile would follow while traveling in the 'eastwards' direction stipulated by the 2009 regulations. | | |
| The eastern end of the Highlands/Lowlands dividing line is determined using the boundaries of the ? | Lat/Lng | |

[1] Scottish Marine Regions Order 2015, Section 3: https://www.legislation.gov.uk/sdsi/2015/9780111027004

Please open an issue if you have suggestions on how to eliminate any of these assumptions and further refine the map.

https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/809209/SDVS-scotch-whisky-tech-guide.pdf

## Data Sources

### Highlands & Lowlands regions

- Highlands & Lowlands regions: NUTS
- Highlands/Lowlands Divide:
- Wards: Boundary-Line

	1:5,000,000

    UK Ordnance Survey, Open Roads
    https://www.ordnancesurvey.co.uk/business-government/products/open-map-roads

    Scale: 1:15,000 to 1:30,000

    UK Ordnance Survey, Open Rivers
    https://www.ordnancesurvey.co.uk/business-government/products/open-map-rivers

    Scale: 1:15,000 to 1:30,000

    "Clyde Scottish Marine Region" Map Data

    https://spatialdata.gov.scot/geonetwork/srv/eng/catalog.search#/metadata/Marine_Scotland_FishDAC_1609

### UK Wards
UK Ordnance Survey, Boundary-Line
https://www.ordnancesurvey.co.uk/business-government/products/boundaryline

Scale: 1:10,000

ONS

Office of National Statistics Open Geography
http://geoportal.statistics.gov.uk/

https://geoportal.statistics.gov.uk/datasets/wards-december-2017-generalised-clipped-boundaries-in-great-britain

National Grid

NS, NN, NO

## FAQ

### Where are the other Scotch regions, e.g. the "Islands"?

This project is meant to provide an accurate source for only the regions codified in UK law. As the Islands are considered an unofficial sixth region, they are not included.


### Why ONS data instead of UK Ordnance Survey maps?

The ONS maps are the only ones I was able to find that had multiple levels of detail available and are all in a consistent scale at each level of detail. The Or
