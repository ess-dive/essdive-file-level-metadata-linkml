
# Class: FileLevelMetadata


file level metadata for a data package uploaded on essdive

URI: [https://w3id.org/linkml/essdive/flmd/FileLevelMetadata](https://w3id.org/linkml/essdive/flmd/FileLevelMetadata)


[![img](https://yuml.me/diagram/nofunky;dir:TB/class/[Container]++-%20flmd_files%200..*>[FileLevelMetadata&#124;File_Name:string;File_Description:string;Standard:string%20%3F;UTC_Offset:string%20%3F;File_Version:string%20%3F;Contact:string%20%3F;Date_Start:date%20%3F;Date_End:date%20%3F;Northwest_Latitude_Coordinate:double%20%3F;Northwest_Longitude_Coordinate:double%20%3F;Southeast_Latitude_Coordinate:double%20%3F;Southeast_Longitude_Coordinate:double%20%3F;Latitude:double%20%3F;Longitude:double%20%3F;Missing_Value_Codes:string%20%3F;Data_Orientation:string%20%3F;Notes:string%20%3F],[Container])](https://yuml.me/diagram/nofunky;dir:TB/class/[Container]++-%20flmd_files%200..*>[FileLevelMetadata&#124;File_Name:string;File_Description:string;Standard:string%20%3F;UTC_Offset:string%20%3F;File_Version:string%20%3F;Contact:string%20%3F;Date_Start:date%20%3F;Date_End:date%20%3F;Northwest_Latitude_Coordinate:double%20%3F;Northwest_Longitude_Coordinate:double%20%3F;Southeast_Latitude_Coordinate:double%20%3F;Southeast_Longitude_Coordinate:double%20%3F;Latitude:double%20%3F;Longitude:double%20%3F;Missing_Value_Codes:string%20%3F;Data_Orientation:string%20%3F;Notes:string%20%3F],[Container])

## Referenced by Class

 *  **None** *[➞flmd_files](container__flmd_files.md)*  <sub>0..\*</sub>  **[FileLevelMetadata](FileLevelMetadata.md)**

## Attributes


### Own

 * [➞File_Name](fileLevelMetadata__File_Name.md)  <sub>1..1</sub>
     * Description: Name of the file. Provide the name of the associated file. File names should be unique and be as descriptive as possible about the file contents. Use only letters (e.g. CamelCase), numbers, and underscores. Do not include spaces. Hyphens allowed but not preferred. Use "*" wildcard when the FLMD applies to multiple files. For example - the same FLMD applies to all soil core files in this data package - "soil_cores_*.csv"
     * Range: [String](types/String.md)
 * [➞File_Description](fileLevelMetadata__File_Description.md)  <sub>1..1</sub>
     * Description: A brief description of the file. A brief description (minimum 30 characters) of the file and what distinguishes this file from other files in the data package. Include information about the type of data (images, observations, experimental, etc.)
     * Range: [String](types/String.md)
 * [➞Standard](fileLevelMetadata__Standard.md)  <sub>0..1</sub>
     * Description: Standard applied to the data file. Identify if an ESS-DIVE Reporting Format or any other data or metadata standard was applied to the data file.
     * Range: [String](types/String.md)
 * [➞UTC_Offset](fileLevelMetadata__UTC_Offset.md)  <sub>0..1</sub>
     * Description: Local Standard Time Offset. Report the Local Standard Time offset (+/- `hours`) or time zone (abbreviations allowed). Do not report time using Daylight Savings Time.
     * Range: [String](types/String.md)
 * [➞File_Version](fileLevelMetadata__File_Version.md)  <sub>0..1</sub>
     * Description: The version of the file. This is the version of the data file being described in the FLMD. The data file version is assigned by the data provider and not by the system. This would change if the data file is updated after the data package is published. Changes should be explained in the Notes field.
     * Range: [String](types/String.md)
 * [➞Contact](fileLevelMetadata__Contact.md)  <sub>0..1</sub>
     * Description: Contact for the file. Provide first and last name of the contact for the file. This should be someone with information already recorded at the Data Package Level.
     * Range: [String](types/String.md)
 * [➞Date_Start](fileLevelMetadata__Date_Start.md)  <sub>0..1</sub>
     * Description: The earliest date in the file. All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format.
     * Range: [Date](types/Date.md)
 * [➞Date_End](fileLevelMetadata__Date_End.md)  <sub>0..1</sub>
     * Description: The latest date in the file. All dates must follow the ISO 8601 standard. This field can be date only following the ISO 8601 standard (YYYY-MM-DD) and completed to known precision (e.g. YYYY-MM, YYYY). The FLMD Extractor can extract the start/end date from a CSV file following the CSV Reporting Format.
     * Range: [Date](types/Date.md)
 * [➞Northwest_Latitude_Coordinate](fileLevelMetadata__Northwest_Latitude_Coordinate.md)  <sub>0..1</sub>
     * Description: Northwest Latitude Coordinate for non-point location. This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
     * Range: [Double](types/Double.md)
 * [➞Northwest_Longitude_Coordinate](fileLevelMetadata__Northwest_Longitude_Coordinate.md)  <sub>0..1</sub>
     * Description: Northwest Longitude Coordinate for non-point location. This is part of a coordinate pair to form the Northwest corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
     * Range: [Double](types/Double.md)
 * [➞Southeast_Latitude_Coordinate](fileLevelMetadata__Southeast_Latitude_Coordinate.md)  <sub>0..1</sub>
     * Description: Southeast Latitude Coordinate for non-point location. This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
     * Range: [Double](types/Double.md)
 * [➞Southeast_Longitude_Coordinate](fileLevelMetadata__Southeast_Longitude_Coordinate.md)  <sub>0..1</sub>
     * Description: Southeast Longitude Coordinate for non-point location. This is part of a coordinate pair to form the Southeast corner of a bounding box for non-point locations. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
     * Range: [Double](types/Double.md)
 * [➞Latitude](fileLevelMetadata__Latitude.md)  <sub>0..1</sub>
     * Description: Coordinate for single point location. This field is paired with "Longitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
     * Range: [Double](types/Double.md)
 * [➞Longitude](fileLevelMetadata__Longitude.md)  <sub>0..1</sub>
     * Description: Coordinate for single point location. This field is paired with "Latitude" to create a coordinate pair for a single point. All geographic coordinates must be provided in WGS84 decimal format. It is strongly recommended to record the geographic coordinates in the FLMD in cases where the data file does not include geographic coordinates and the entire file consists of measurements collected at a single location. The FLMD Extractor can extract the geographic coordinates or bounding box coordinates from a CSV file following the CSV Reporting Format.
     * Range: [Double](types/Double.md)
 * [➞Missing_Value_Codes](fileLevelMetadata__Missing_Value_Codes.md)  <sub>0..1</sub>
     * Description: Report missing value codes. Report all Missing Value Codes. For columns containing numeric data, use "-9999" as the missing value code (or modify to match significant figures given the data). For columns containing character data, use "N/A" as the missing value code. If entering more than one missing value code, use a vertical bar "|" or semicolon ";" instead of a comma or protect the comma with matching double quotation marks around the entire value. For more information about commas not meant to be a delimiter (e.g. used within a cell), refer to the Delimiter section of the CSV Reporting Format Detailed Guide.
     * Range: [String](types/String.md)
 * [➞Data_Orientation](fileLevelMetadata__Data_Orientation.md)  <sub>0..1</sub>
     * Description: Orientation of tabular data. Describe how the data are organized within the data matrix. Choose between "horizontal" (i.e., data are organized in rows) or "vertical" (i.e., data are organized in columns).
     * Range: [String](types/String.md)
 * [➞Notes](fileLevelMetadata__Notes.md)  <sub>0..1</sub>
     * Description: Any information the provider would like to add. Information provided would be data file specific. Details may include details on data file versioning, reporting format, software requirements, data quality, etc.
     * Range: [String](types/String.md)
