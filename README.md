# winchtension_parser
Parses out winch tension data at a user-given threshold to a graphable .csv format

Two scripts, tension-report (granular, shows all data at 20hz), 
and tensionreport-20s (chooses max tension spike per 20 entries) parses existing winch data.  
Its purpose is to print out the max tension, in an excel-readable .csv format.  T
his is to comply with Appendix A, to show when our winches went over a certain threshold.  
Very basic and was quickly written at the time for Matt Durham to comply with his
requirements to parse specific winch data for a reports he works on.
