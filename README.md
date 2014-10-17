jQuery.xml2json
---------------
The XML to JSON Plugin (jQuery.xml2json) is a script you can use to convert simple XML into a JSON object by [fyneworks](https://www.fyneworks.com/jquery/xml-to-json/).
This is used by [jQuery Soap](https://github.com/doedje/jquery.soap) (optional).
 
Install
-------
Via bower:
`bower install jquery.xml2json --save`

Example
-------
```Javascript
$.soap({
    url: 'http://my.server.com/soapservices/',
    method: 'helloWorld',

    data: {
        name: 'Remy Blom',
        msg: 'Hi!'
    },

    success: function (soapResponse) {
        soapResponse.toJSON();
    },
    error: function (SOAPResponse) {
        SOAPResponse.toJSON();
    }
});
```