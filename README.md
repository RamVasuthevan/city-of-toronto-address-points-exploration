# city-of-toronto-address-points-exploration

[Old Shapefile readme](ADDRESS_POINT_WGS84_readme.txt)

### ADDRESS_POINT_ID
### ADDRESS_ID
### ADDRESS_STRING_ID
### LINEAR_NAME_ID
### CENTRELINE_ID

### MAINT_STAGE
- > MAINT_STAG = MAINT_STAGE  (Maintenance stage (e.g. reserve, regular))
- maintenance_stage 
    - `REGULAR` - 518490
    - `RESERVED` - 7296
- What is the maintenance stage?

### ADDRESS_NUMBER
- > ADDRESS = ADDRESS_NUMBER  (address number with suffix)
- address_number
- The number (with suffix) component of the address
- Sample values
    - `1`
    - `1 1/2`
    - `1-11`
    - `1-11`
    - `1001R`
    - `2625A-2625G`
- (LO_NUM)(LO_NUM_SUF)-(HI_NUM)(HI_NUM_SUF)
- A formula to generate ADDRESS_NUMBER from 

### LINEAR_NAME_FULL
- >  LFNAME = LINEAR_NAME_FULL  (Street Name)
- linear_name_full
- The full street name with the street type
- Sample values:
    -  `Palisades`
    - `Abraham Welsh Rd`
    - `Colonel Samuel Smith Park Dr`

### LO_NUM
- > LONUM = LO_NUM  (Address low number)
- address_number_lower_digit
- The lower number of address number but not suffix
- Sample values:
    - `1`
    - `11753`

### LO_NUM_SUF
- > LONUMSUF = LO_NUM_SUF  (Low number suffix)
- address_number_low_suffix
- The suffix of the lower number of address number
- Sample value:
    - (Empty String)
    - `A`
    - `1/2`
- empty string should be `null`

### HI_NUM
- > HINUM = HI_NUM  (Address High number)
- address_number_higher_digit
- The high number of address number but not suffix
- If it does not exist, it is 0 in the geopackage. it should be 0


### HI_NUM_SUF
- > HINUMSUF = HI_NUM_SUF  (High Number suffix)
- address_number_high_suffix
- The suffix of the high number of address number
- Sample value:
    - (Empty String)
    - `A`
    - `1/2`
- empty string should be `null`

### LINEAR_NAME

### LINEAR_NAME_TYPE
- Not in the README
- linear_name_type
- Sample value:
    - (Empty String)
    - `Ave`
    - `Mews`
    - `Rdwy`

### LINEAR_NAME_DIR
- Not in the README
- linear_name_direction
- Value:
    - (Empty String)
    - `W`
    - `E`
    - `N`
    - `S`

### LINEAR_NAME_DESC
- Not in the README
- linear_name_description
- Sample values:
    - (Empty String)
    - `TORONTO`
    - `NORTH YORK`
    - `TO, EY, NY`
    - `N.OF CPR`
    - `no type`
    - `YORK UNIVERSITY`
- What is this?

### CENTRELINE_SIDE
### CENTRELINE_MEASURE
### CENTRELINE_OFFSET 

### GENERAL_USE_CODE
- > FCODE = GENERAL_USE_CODE  (Feature code number)
- > These attributes are GENERALUSE and GENERALUSE_CODE (also known as Feature Code and Feature Code Description). These two attributes are based on a historic dataset, have not been regularly maintained, and have no reliable, affordable sources for continued update.

    > Due to these factors, these attributes were nullified (made blank) on Thursday, July 29, 2021. It is important to note that the attribute columns will remain in the database to ensure this change does not affect existing applications, however there will be no values in them.
- Delete this
- Always `115001`

### GENERAL_USE
- > FCODE_DES = GENERAL_USE  (Feature code description)
- Delete this
- Always `Unknown`

### CLASS_FAMILY
### CLASS_FAMILY_DESC
### ADDRESS_CLASS
### ADDRESS_CLASS_DESC
### ADDRESS_POINT_ID_LINK
### ADDRESS_ID_LINK
### PLACE_NAME
### PLACE_NAME_ALL

### ADDRESS_STATUS
- Not in readme
- Always empty string

### OBJECTID

### MUNICIPALITY
- not in readme
- former_municipality_abbreviation
- 6 values
- Values:
    - `ET`
    - `EY`
    - `NY`
    - `SC`
    - `TO`
    - `YK`

### MUNICIPALITY_NAME
- > MUN_NAME = MUNICIPALITY_NAME  (Former Municipality Name)
- former_municipality_name
- 6 values
- Values:
    - `former Toronto`
    - `Scarborough`
    - `North York`
    - `Etobicoke`
    - `York`
    - `East York`

### WARD
- Not it README
- ward_number
- Ward number from 01 to 25
- Sample values:
    - `01`
    - `10`
    - `25`
- should be an integer

### WARD_NAME
- > WARD_NAME = WARD_NAME  (Ward Name)
- ward_name
- 25 values
- Ward names in titlecase
- Sample value:
    - `Toronto-Danforth`
    - `Toronto-St. Paul's`
    - `Don Valley East`
- Confirm these are offical names

### ADDRESS_FULL
- Not in readme
- Sample values:
    - ``
- Generate forumla to build from compents