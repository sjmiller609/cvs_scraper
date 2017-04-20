# cvs scraper

lets you know when people buy things

this script alerts the user when items of a certain type are sold from any CVS near a location.

right now it's broken because it needs to interpret javascript, which previously it did not

It takes 3 input parameters, <item> <location> <item count>
	item: any item description, this will be sent to CVS' product search and will it will scrape <item count> product IDs from the results
	location: the script will check for inventory near this location. any location you could put in google maps should work
	item count: how many product IDs to get

limitations:

cannot alert user for any item sold in a region, can only check by search keyword or specific item (using skuid as <item> argument)
precision of time sold is traded off with number of items scanned
iterates through items checking their availability in store, lets you know when inventory amount changes
