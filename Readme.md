# json-body-stringifier - Burp Repeater Extension

This extension creates a new tab under Repeater and recursively converts all non-string JSON fields, such as int or boolean, to string to make them ready for fuzz testing. The extension supports complex JSON hierarchies with multiple nested dict/list levels.

Any request detected as having a JSON body within Repeater will trigger the creation of a new tab where all fields are recursively converted to string. To update the original request, simply change any field in the custom tab.

The request can then be fuzzed as usual (Active Scan or send to Intruder -> Active Scan insertion points).
