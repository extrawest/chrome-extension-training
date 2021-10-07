##Options page
Options page created with Vue includes (mock options_1):
- title
- checkbox for toggling extension state
- dropdown select for the base currency (mock options_2)
- multiple select for the target currencies (mock options_3)

Base currency and target currencies properties are a part of the extension config which is going to store in [chrome.storage.sync](https://developer.chrome.com/docs/extensions/reference/storage/).

Base currency is preselected (f.e. USD) and required.  
Target currencies are preselected (f.e. [EUR]) and required as well.

#
>Expected hours: **16**
