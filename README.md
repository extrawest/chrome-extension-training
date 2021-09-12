# Chrome extension training: Currency Converter

### General use case:
- Once extension get installed *Options page* is opened programmatically.  
  The page includes title, short description, dropdown select for the base currency and multiple select for the target currencies.
  For example, base currency set to UAH and target ones to [USD, EUR].
- If extension is enabled, when user selects any text on any webpage content script checks whether selected text content includes any numeric value.  
  Parsing result examples:  
```javascript
input1 = '...before 1928 measured 7.42 in × 3.125 in (188.5 mm × 79.4 mm)...' // 1928
input2 = '...measured 7.42 in × 3.125 in (188.5 mm × 79.4 mm)...' // 7.42
input3 = '...Today, USD notes are made from cotton fiber paper...' // null
```
- If selection includes the numeric value (for example 100), content script appends a button near the selected text.
- If user clicks outside the button, it disappears.
- If user clicks the button, extension appends a closable popup with a table near the selected area.
- As the base currency is UAH, target ones are USD and EUR and selected value is 100, the table should include two rows:
  - USD - 3.6033
  - EUR - 2.9711
- When user clicks browser action (extension icon at the toolbar) it shows a popup with:
  - a title (extension name)
  - a button which allows to activate/deactivate the extension for all the webpages
  - a link to the options page
  
>Currency rates are provided by the [API](https://hovorun.herokuapp.com/).  
>As it's free, server falls asleep every hour and initial request may take about 5 seconds.  
>Every next request will be executed much faster.

>Mocks and images will be mentioned further can be found in **./assets** folder.

### Milestones
- [Basics](./milestones/basics.md)
- [Webpack configuration](./milestones/webpack.md)
- [Options page](./milestones/options.md)
- [Content and background scripts](./milestones/scripts.md)
- [Browser actions](./milestones/actions.md)
