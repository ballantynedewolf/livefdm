# livefdm
Live fire danger meter for NSW, Australia

The app pulls the current fire danger rating and a boolean value for total fire ban from http://www.rfs.nsw.gov.au/feeds/fdrToban.xml 
which is the same data that constructs https://www.rfs.nsw.gov.au/fire-information/fdr-and-tobans
but which is NSW-wide.

The app requires a URL parameter for the region you want to query eg.?region=Greater%20Sydney%20Region
(some browsers let you use spaces instead of %20)

The app displays the FDR graphically, and scrolls one of two messages: "No fires without a permit - call your local fire control centre"
which applies at all times during the bushfire danger period of Oct to April inclusive; and "Total Fire Ban - no fires" when the field
FireBanToday is set to Yes
