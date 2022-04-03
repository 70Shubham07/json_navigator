# json_navigator




## Usage

from navJson import jsonParsing

### If the object you want to inspect is Python list, use below code
returnedCollectionOfCodes, finalCodeSoFar = jsonParsing.listParserAndCodeCreator( jsonToBeParsed, rootCode = "jsonToBeParsed", collectionOfCodes = list() )

### If it is a python dictionary, use below code

returnedCollectionOfCodes, finalCodeSoFar = jsonParsing.jsonParserAndCodeCreator( jsonToBeParsed, rootCode = "jsonToBeParsed", collectionOfCodes = list() )











