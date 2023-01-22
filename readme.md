# Work in Progress...

# Authcord python library
The Authcord library is a Python module that allows you to easily communicate with the Authcord API.

# Documentation 
see the <a href="https://docs.authcord.xyz">Authcord docs</a>

# Installation
If you don't want to install from the source you can run:
```
pip install authcord
```

If you do want to install from the source you can run:
```
python setup.py
```

# Usage 
Before using the authcord module you must set your Authcord APIKEY by writing the bellow code:
```py
authcord = Authcord("YOUR_USER_LEVEL_APIKEY")
```

once you have set your Authcord APIKEY you can now use the functions.

<b>Functions</b><br>
```check_hwid```

Example: 
```py
from authcord import Authcord

# Create an instance of the Authcord class and pass in your API key
api = Authcord("YOUR_USER_LEVEL_API_KEY")

# Use the check_hwid method to check the status of a HWID
hwid = "testhwid"
response = authcord.check_hwid(hwid)


# check the response 
if response["Response"] == "Valid":
    print("HWID is valid.")
else:
    print("HWID is not valid.")
   ```
