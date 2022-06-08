# Validate-akamai-schema
Example code for validating akamai ruleset against product specific api schema

**In order to use this script, 

- you will need to edit it to include your '.edgerc' location (the file containing your API authorizations).

- Using a text editor, edit line 16 and provide the full system path to your .edgerc file.
Example: edgeRcLoc = '/Users/bob/.edgerc'

**This script takes one argument:
validate-akamai-schema.py <akamai ruleset json file>

This script will produce a non-zero exit code if the JSON does not conform to the product schema. It will also log output to the shell indicating what specific JSON elements are incorrect, including their placement in the rule hierarchy
