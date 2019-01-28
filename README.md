# RML Test Cases

The [RML](http://rml.io/) test cases are used to determine the conformance to the [RML specification](http://rml.io/spec.html) of tools that execute RML rules.

In the folder `test-cases` you can find the different test cases.
Each test case is contained in a single folder, containing three types of files:

- Zero or more files containing the data sources, in the case of JSON, XML, CSV, or 
containing the SQL statements to create the necessary tables, in the case of MySQL, PostgreSQL, and SQL Server. 
- One file with the RML rules, called `mapping.ttl`, in the Turtle format.
- Zero or one file with the expected RDF. No file is provided if an error is expected that must halt the generation of the RDF.

The details about the test cases cases are also available as a knowledge graph in `metadata.nt`.
The knowledge graph is generated by executing the RML rules in `rules.ttl`, available as [YARRRML](https://w3id.org/yarrrml) in `rules.yml`.
The data source used by the rules is `metadata.csv`.

## Documentation

A website describing the test cases is available in `docs`.
The website is generated by doing the following:

1. Install node.js dependencies: `npm i`
2. Run [Eleventy](http://11ty.io/): npx eleventy
3. Find the website in the folder `_site`

## License
This code is copyrighted by [Ghent University – imec](http://idlab.ugent.be/) and released under the [MIT license](http://opensource.org/licenses/MIT).
