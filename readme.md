# Be Honest


### Site Structure
The site is mostly static, hard-coded HTML and CSS (or rather, [LESS](http://lesscss.org/features/) using less.js). Student content is controlled via a Google Spreadsheet (contact Kate Bingaman-Burt for access to that), which is exported as CSV (comma-separated values) data, which is processed and converted into JS by a jQuery library ([jquery.csv.min.js](https://github.com/evanplaice/jquery-csv)).

##### scripts.js
Handles Most site interactions, animations, and a little bit of responsive stuff

##### bioModal.js
Manages student CSV data and interactions

##### jquery.csv.min.js
Parses CSV data from Google Spreadsheets and converts it to easy-to-use JSON (javascript) data

##### inliner.js
Converts SVG img tags into inline SVG, which is useful for styling and manipulating SVG elements


### Content Collection and Management
The Google Spreadsheet can be populated most efficiently by establishing a Google Form that exports to a Google Spreadsheet. From there the content of the spreadsheet can be copied to another spreadsheet where it can be better formatted and published.

To make the content on the data spreadsheet available to the site, go to File > Publish to the Web... in the Google Spreadsheet and publish the page as CSV.

**NOTE:** If you are collecting any private or sensitive info (Student IDs, email addresses, etc.), make sure to delete it from the spreadsheet BEFORE publishing it.
