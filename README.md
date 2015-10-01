# visual_mapper

Preamble
-----------
Open-source Zapier/IFTTT "mapping generator" to provide automation services to the international development sector. Current projects are in public health, agriculture, and education.


	i.e., a trigger event triggers an action based on a filtering rule:
	
	When *a new patient record is created* in a mobile clinic system,
	Then *create a new outbound SMS record* in an sms gateway.

The epic:
-----------------------
1. Given a schema in "JSON-schema" the user wants to be able to define an action (create or update records) in a destination database.

We'd like to use JSON-editor (https://github.com/jdorn/json-editor) to present the user with an HTML webform to define the insert/update action. This webform will allow the user to type values for each field in the destination schema(s). This webform will also allow the user to insert `source value placeholders` (SVPs) from a `source schema` that tell us what data to expect from a triggering event. These SVPs are effectively "ingredients" in an "If-This-Then-That" recipie.

![Image of Layout](https://github.com/OpenFn/visual_mapper/blob/master/layout.png)

Important artifacts:
--------------

1. Destination schema: this defines our HTML form. a composite schema (with several objects) can be found @composite_destination_schema.json

2. Source schema: this is used to mix-in `source value placeholders` (ingredients) to our final action directive. found @sample_source_schema.json

3. Target output file: [target_mapper_output.json](https://github.com/OpenFn/visual_mapper/blob/master/target_mapper_output.json)

------------------------------------
Data to play with.

a. a sample source payload to play with: @sample_source_payload.json

b. a sample wished destination payload to aim for: @sample_destination_payload.json
