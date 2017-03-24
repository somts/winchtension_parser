# winchtension_parser
Parses out winch tension data at a user-given threshold to a graphable .csv format

Two scripts, tension-report (granular, shows all data at 20hz), 
and tensionreport-20s (chooses max tension spike per 20 entries) parses existing winch data.  
Its purpose is to print out the max tension, in an excel-readable .csv format.  T
his is to comply with Appendix A, to show when our winches went over a certain threshold.  
Very basic and was quickly written at the time for Matt Durham to comply with his
requirements to parse specific winch data for a reports he works on.

# Purpose: to print out max tension, and winch tension above a certain threshold
#Usage: 
* tension-report, to be used with winch-tension-threshold
* sh tension-report SP 15 /mnt/nas2/SIO-Cruises/Sproul 2000' where SP is ship initial, 15 is year, followed by cruise directory, then the threshold."
* sh tension-report SP 15 /mnt/nas2/SIO-Cruises/Sproul/SP1504 2000' You can also process a specific cruise directory

* Non-standard cruise directory names must be specified and processed individually '.../Sproul/CalFofi2000'
* Notice how none of the examples have a trailing slash.  Do not end your directory path with a trailing slash!

* Error: If you see this message with entered parameters, the target directory you've supplied does not exist, and/or you've entered insufficient paramters.


