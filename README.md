## US Street Address Parser

This is Node.js port for Perl [Geo::StreetAddress::US](http://search.cpan.org/~timb/Geo-StreetAddress-US-1.04/US.pm) package

*Description from Geo::StreetAddress::US*:

>Geo::StreetAddress::US is a regex-based street address and street intersection parser for the United States. Its basic goal is to be as forgiving as possible when parsing user-provided address strings. Geo::StreetAddress::US knows about directional prefixes and suffixes, fractional building numbers, building units, grid-based addresses (such as those used in parts of Utah), 5 and 9 digit ZIP codes, and all of the official USPS abbreviations for street types and state names... [more](http://search.cpan.org/~timb/Geo-StreetAddress-US-1.04/US.pm)

### Install:

`npm install parse-address`

### Usage:

```javascript
var parser = require('parse-address');
var parsed = parser.parseLocation('1005 N Gravenstein Highway Sebastopol CA 95472');

//Parsed address:
{ 
 number: '1005',
 prefix: 'N',
 street: 'Gravenstein',
 type: 'Highway',
 city: 'Sebastopol',
 state: 'CA',
 zip: '95472' }
 
```
 

TODO:

1. Freeform Address parser
2. Register with bower