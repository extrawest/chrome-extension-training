###Content and background scripts
Implement and inject content script which is mentioned in description.  
If extension is enabled, once user has selected some text with numeric value, append the button near the selected area (mock content_1).  
While fetching/converting the results button should be replaced with some loader (mock content_2).  
Once result is ready, display it in fixed popup dialog (mock content_3).

Popup includes:
- initial amount that has been converted
- button for opening the options page
- button for closing the popup
- list of conversions
- last time when rates were updated (provided by API)

Click outside also triggers the popup closing.

#
>Expected hours: **24**
