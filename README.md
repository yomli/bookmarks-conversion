# Bookmarks Conversion

This script converts a bookmarks file in JSON to its Netscape HTML equivalent.


## Usage

Just paste the content of the JSON file into the textarea and press "Convert".


### WebKit-based browsers

WebKit-based browsers use a specific Windows timestamp, not the common Unix Epoch (for more info, see: http://timothycomeau.info/chrome-history/).

If dates are important, please uncomment the following lines :
``` javascript
tmp["date"] = (tmp["date"]/1000000-11644473600);
tmp["modified"] = (tmp["modified"]/1000000-11644473600);
```

## License
Licensed under the Beerware license, revision 42.