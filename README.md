PyAgresso
===================

Author: Osama Khan

License: MIT

Website: https://github.com/osamakhn/pyagresso


This module helps developers work with the Agresso Unit4 (ver. Milestone 4) Query Engine
SOAP webservice easily without worry about the transport layer/protocol and getting data in easible
ingestible formats: JSON, CSV

## Installation:

`$ pip install pyagresso`

## Example:

```python
from pyagresso.api import Agresso
username = os.getenv('AGRESSO_USERNAME')
password = os.getenv('AGRESSO_PASSWORD')
client = os.getenv('AGRESSO_CLIENT')
instance_url = os.getenv('AGRESSO_INSTANCE_URL')
ag = Agresso(username, password,client,instance_url)
about_response_as_xml = ag.about()
```

## Todo:
[*] Setup basic pypi project and Agresso class with test harness

[ ] Add methods to get response as JSON

[ ] Add methods to get response as CSV

[ ] Add internal helpers to parse xml (schema+records)

[ ] Make QueryEngine methods into submodule and add capability for extension into other Agresso modules

[ ] Version the SDK for various Agresso releases

## Other notes: 
_Not using bdd in this library due to small size of module undertest_

## Development:
_Please refer to `makefile`_