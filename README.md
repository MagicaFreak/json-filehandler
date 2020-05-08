# NoirPi JSON Handler

This is a simple JSON Filehandler. 

### Installation
```
pip install noirpi-jsonhandler
```

## FileIO Json Load
Load a JSON file
```
from jsonhandler.FileIO import FileIO

def load_json():
    FileIO.fileio("./test.json", "load")
```

## FileIO Json Save
Save a JSON file
```
from jsonhandler.FileIO import FileIO

def save_json():
    FileIO.fileio("./tests.json", "save", {})

def save_json():
    jsondict = {"test": "value"}
    FileIO.fileio("./test.json", "save", jsondict)
```

## FileIO Json File Check
Check if JSON file has valid Syntax
```
from jsonhandler.FileIO import FileIO

def check_json():
    FileIO.fileio("./test.json", "check")
```

## FileIO Json Dict Validation
Check if JSON dictionary is has a valid syntax
```
from jsonhandler.FileIO import FileIO

def validate_json():
    jsondict = {"test": "value"}
    FileIO.validate(jsondict)
```

## FileIO Check file
Check if JSON File exists if not create it with given value
```
from jsonhandler.FileIO import FileIO

def check_json_file():
    jsondict = {"test": "value"}
    FileIO.check_file("./", "test.json", jsondict)
```

## FileIO get value 
Gets a value from JSON File
```
from jsonhandler.FileIO import FileIO

def check_json_file():
    jsondict = {"test": "value"}
    FileIO.check_file("./", "test.json", jsondict)

def get_value():
    FileIO.get_value("./test.json", ["test"])
```

## FileIO set value in json file
Sets or adds a value inside a JSON File
```
from jsonhandler.FileIO import FileIO

def check_json_file():
    jsondict = {"test": "value"}
    FileIO.check_file("./", "test.json", jsondict)

def set_value():
    FileIO.set_value("./setvaluetest.json", "Testing", "test")
```
