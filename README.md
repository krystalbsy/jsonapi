# jsonapi
Extended python's standard json library to encode and decode complex and range objects.

# Installation Instruction:
In the root directory, run the following: pip install -e .

# Sample Code:
```python
import json

class ExtendEncoder(json.JSONEncoder):
    ...

class ExtendDecoder(json.JSONDecoder):
    ...

def dumps(data, cls=ExtendEncoder):
    return json.dumps(data, cls=cls)

def loads(data, cls=ExtendDecoder):
    return json.loads(data, cls=cls)
```
