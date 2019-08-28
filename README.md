# MongoExportToCSV
1. Use MongoDB to save json file
When scraping data from web, the response may be json format, we can use json library to handle this.
If the json file is in right format, then you can use mongoexport command to export to csv.

mongoexport --db database --collection collection  --type=csv --fields field1,field2 --out "dir\collection.txt"

2. Convert non-regular json to normal for exporting
For instance, the following json (from MongoDB) is not in the regular format, we cannot do much to the json (map reduce, aggregate, pipline operation etc.), we need convert it to normal table, export to csv/table or re-dump into MongoDB.