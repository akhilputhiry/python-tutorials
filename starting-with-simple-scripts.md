## Scripts ##

A sample python script looks like,

```
#! /usr/bin/python

import json

def serialize_data(data):
    return json.dumps(data)

if __name__ == "__main__":
    data = {
        "name": "Maria",
        "place": "Kottayam",
    }
    print serialize_data(data)
```

and suppose the above code is saved in a file called `serialize.py`, you can execute the code by simply calling `serialize.py` in the terminal

Now let me explain what this script means.

* The very first line `#! /usr/bin/python` is called `shebang`, the meaning of this is `this script needs to be executed using the exe /usr/bin/python`
* If `shebang` is not present in the script, then you cannot execute the script by simply calling the file name. You need to call the script with python explicitly `python serializer.py`
* After shebang, it will be normally import statements
* Your program may need other libraries or functions/classes from other modules, `import` is used to import the required libraries to your script
* After import statements it will be your functions or classes
* `if __name__ == "__main__"` this is the entry point of the script


## Practise problems ##

* Create a calculator script which can perform addition, substraction, division and multiplication
