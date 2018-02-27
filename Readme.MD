# Derby JSON Schema
This project represents an attempt to encode the DerbyJSON spec (found in the [derbystatter](https://github.com/wftda/derbystatter) project) in JSON schema, to make it easier to work with in code generation and validation.  It also gave me an opportunity to learn more about 

# Layout
`root.json` represents the root object.  Additional files represent various types of objects that are used more than once in the schema, and while some (like `venue.json` and `league.json`) may be top-level objects per the spec, others may not.

# TODO

* I think some of the instance where a team reference is explicitly a uuid are incorrect per the spec
* Test data is necessary to ensure that these schemas actually validate a correct derby JSON object
* The schema is currently very non-strict, and there are probably opportunities to restrict the formatting and structure of the objects more.
* Descriptions are somewhat sparse, and probably need to be fleshed out so that the spec document can be generated off of the schema files. 
* Actually publishing these on my site to enable use and validation

# License
For now, the schema in this project is licensed under the Apache 2.0 license.