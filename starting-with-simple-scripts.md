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

Now let me explain what this script means.

The very first line `#! /usr/bin/python` is called `shebang`, the meaning of this line is `this script needs to be executed using the exe /usr/bin/python`
