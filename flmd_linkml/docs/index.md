
# flmd_schema


**metamodel version:** 1.7.0

**version:** None


schema for file level metadata (flmd) reporting format


### Classes

 * [Container](Container.md) - list of flmd files
 * [FileLevelMetadata](FileLevelMetadata.md) - file level metadata for a data package uploaded on essdive

### Mixins


### Slots

 * [➞flmd_files](container__flmd_files.md)
 * [➞Contact](fileLevelMetadata__Contact.md) - Contact for the file. Provide first and last name of the contact for the file. This should be someone with information already recorded at the Data Package Level.
 * [➞Data_Orientation](fileLevelMetadata__Data_Orientation.md) - Orientation of tabular data. Describe how the data are organized within the data matrix. Choose between "horizontal" (i.e., data are organized in rows) or "vertical" (i.e., data are organized in columns).
 * [➞Date_End](fileLevelMetadata__Date_End.md) - The latest date in the file. All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format.
 * [➞Date_Start](fileLevelMetadata__Date_Start.md) - The earliest date in the file. All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format.
 * [➞File_Description](fileLevelMetadata__File_Description.md) - A brief description of the file. A brief description (minimum 30 characters) of the file and what distinguishes this file from other files in the data package. Include information about the type of data (images, observations, experimental, etc.)
 * [➞File_Name](fileLevelMetadata__File_Name.md) - Name of the file. Provide the name of the associated file. File names should be unique and be as descriptive as possible about the file contents. Use only letters (e.g. CamelCase), numbers, and underscores. Do not include spaces. Hyphens allowed but not preferred. Use "*" wildcard when the FLMD applies to multiple files. For example - the same FLMD applies to all soil core files in this data package - "soil_cores_*.csv"
 * [➞File_Version](fileLevelMetadata__File_Version.md) - The version of the file. This is the version of the data file being described in the FLMD. The data file version is assigned by the data provider and not by the system. This would change if the data file is updated after the data package is published. Changes should be explained in the Notes field.
 * [➞Latitude](fileLevelMetadata__Latitude.md) - Coordinate for single point location. This field is paired with "Longitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
 * [➞Longitude](fileLevelMetadata__Longitude.md) - Coordinate for single point location. This field is paired with "Latitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
 * [➞Missing_Value_Codes](fileLevelMetadata__Missing_Value_Codes.md) - Report missing value codes. Report all Missing Value Codes. For columns containing numeric data, use "-9999" as the missing value code (or modify to match significant figures given the data). For columns containing character data, use "N/A" as the missing value code. If entering more than one missing value code, use a vertical bar "|" or semicolon ";" instead of a comma or protect the comma with matching double quotation marks around the entire value. For more information about commas not meant to be a delimiter (e.g. used within a cell), refer to the Delimiter section of the CSV Reporting Format Detailed Guide.
 * [➞Northwest_Latitude_Coordinate](fileLevelMetadata__Northwest_Latitude_Coordinate.md) - Northwest Latitude Coordinate for non-point location. This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
 * [➞Northwest_Longitude_Coordinate](fileLevelMetadata__Northwest_Longitude_Coordinate.md) - Northwest Longitude Coordinate for non-point location. This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
 * [➞Notes](fileLevelMetadata__Notes.md) - Any information the provider would like to add. Information provided would be data file specific. Details may include details on data file versioning, reporting format, software requirements, data quality, etc.
 * [➞Southeast_Latitude_Coordinate](fileLevelMetadata__Southeast_Latitude_Coordinate.md) - Southeast Latitude Coordinate for non-point location. This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
 * [➞Southeast_Longitude_Coordinate](fileLevelMetadata__Southeast_Longitude_Coordinate.md) - Southeast Longitude Coordinate for non-point location. This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
 * [➞Standard](fileLevelMetadata__Standard.md) - Standard applied to the data file. Identify if an ESS-DIVE Reporting Format or any other data or metadata standard was applied to the data file.
 * [➞UTC_Offset](fileLevelMetadata__UTC_Offset.md) - Local Standard Time Offset. Report the Local Standard Time offset (+/- `hours`) or time zone (abbreviations allowed). Do not report time using Daylight Savings Time.

### Enums


### Subsets


### Types


#### Built in

 * **Bool**
 * **Curie**
 * **Decimal**
 * **ElementIdentifier**
 * **NCName**
 * **NodeIdentifier**
 * **URI**
 * **URIorCURIE**
 * **XSDDate**
 * **XSDDateTime**
 * **XSDTime**
 * **float**
 * **int**
 * **str**

#### Defined

 * [Boolean](types/Boolean.md)  (**Bool**)  - A binary (true or false) value
 * [Curie](types/Curie.md)  (**Curie**)  - a compact URI
 * [Date](types/Date.md)  (**XSDDate**)  - a date (year, month and day) in an idealized calendar
 * [DateOrDatetime](types/DateOrDatetime.md)  (**str**)  - Either a date or a datetime
 * [Datetime](types/Datetime.md)  (**XSDDateTime**)  - The combination of a date and time
 * [Decimal](types/Decimal.md)  (**Decimal**)  - A real number with arbitrary precision that conforms to the xsd:decimal specification
 * [Double](types/Double.md)  (**float**)  - A real number that conforms to the xsd:double specification
 * [Float](types/Float.md)  (**float**)  - A real number that conforms to the xsd:float specification
 * [Integer](types/Integer.md)  (**int**)  - An integer
 * [Ncname](types/Ncname.md)  (**NCName**)  - Prefix part of CURIE
 * [Nodeidentifier](types/Nodeidentifier.md)  (**NodeIdentifier**)  - A URI, CURIE or BNODE that represents a node in a model.
 * [Objectidentifier](types/Objectidentifier.md)  (**ElementIdentifier**)  - A URI or CURIE that represents an object in the model.
 * [String](types/String.md)  (**str**)  - A character string
 * [Time](types/Time.md)  (**XSDTime**)  - A time object represents a (local) time of day, independent of any particular day
 * [Uri](types/Uri.md)  (**URI**)  - a complete URI
 * [Uriorcurie](types/Uriorcurie.md)  (**URIorCURIE**)  - a URI or a CURIE
