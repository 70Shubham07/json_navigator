# json_navigator




## Usage

#### from navJson import jsonParsing

### If the object you want to inspect is a Python list, use the method below

### If jsonToBeParsed is the variable name - 

#### jsonToBeParsed = [ {"A":2}, {"B":3} ]

#### returnedCollectionOfCodes, _ = jsonParsing.listParserAndCodeCreator( jsonToBeParsed, rootCode = "jsonToBeParsed", collectionOfCodes = list() )

#### resultList = [  (code , eval(code) ) for code in returnedCollectionOfCodes   ]

### Output: (jsonToBeParsed[0]["A"], 2), (jsonToBeParsed[0]["B"], 3)

### If it is a python dictionary, use below method


#### jsonToBeParsed = {"A":2, "B":[3,4]}

#### returnedCollectionOfCodes, _ = jsonParsing.jsonParserAndCodeCreator( jsonToBeParsed, rootCode = "jsonToBeParsed", collectionOfCodes = list() )

#### resultList = [  (code , eval(code) ) for code in returnedCollectionOfCodes   ]

### Output: (jsonToBeParsed["A"], 2), (jsonToBeParsed["B"][0], 3), (jsonToBeParsed["B"][1], 4 )


### Try more complicated json structures.



