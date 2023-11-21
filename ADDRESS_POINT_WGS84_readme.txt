This file requires third party Software to be viewed. It is comprised of geographical and atribute information.

Geographic data contained in this dataset best viewed with the Toronto Centreline file as a background. 

Column name  (Description)
======================================
GEO_ID = ADDRESS_POINT_ID  (unique geographic identifier)
LINK = CENTRELINE_ID  (link to geo_id of the primary address)
MAINT_STAG = MAINT_STAGE  (Maintenance stage (e.g. reserve, regular))
ADDRESS = ADDRESS_NUMBER  (address number with suffix)
LFNAME = LINEAR_NAME_FULL  (Street Name)
LONUM = LO_NUM  (Address low number)
LONUMSUF = LO_NUM_SUF  (Low number suffix)
HINUM = HI_NUM  (Address High Number)
HINUMSUF = HI_NUM_SUF  (High Number suffix)
ARC_SIDE = CENTRELINE_SIDE  (the location of the address point with respect to the street (left or right side of the direction)
DISTANCE = CENTRELINE_MEASURE  (the distance from the start of the street segment along the street segment)
FCODE = GENERAL_USE_CODE  (Feature code number)
FCODE_DES = GENERAL_USE  (Feature code description)
CLASS = ADDRESS_CLASS_DESC  (Address classification (Land, Land Entrance, Structure, Structure Entrance))
NAME = PLACE_NAME  ((if exists e.g. churches, schools, parks etc.))
X = X  (Easting, in MTM NAD 83 (3 degree) Projection)
Y = Y  (Northing, in MTM NAD 83 (3 degree) Projection)
LONGITUDE = LONGITUDE  (Longitude in WGS84 Coordinate System)
LATITUDE = LATITUDE  (Latitude in WGS84 Coordinate System)
OBJECTID = OBJECTID  (Unique system identifier)
MUN_NAME = MUNICIPALITY_NAME  (Former Municipality Name)
WARD_NAME = WARD_NAME  (Ward Name)

CLASS FEATURE DEFINITION

Land address identifies the one and only one Municipal Parcel in which it is located.

Land Entrance identifies an entrance to a Municipal Parcel.

Structure address identifies a building/structure that is located on a Municipal Parcel

Structure Entrance address identifies an entrance to a building or structure.


