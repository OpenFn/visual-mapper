# visual_mapper

Objective
-----------
Open-source Zapier/IFTTT "mapping generator" to provide automation services to the international development sector—current projects are in public health, agriculture, and education.

The epic:
-----------------------
1. Given a schema in "JSON-schema" the user wants to be able to define an action (create or update records) in a destination database.

We'd like to use JSON-editor (https://github.com/jdorn/json-editor) to present the user with an HTML webform to define the insert/update action.

This webform will allow the user to type values for each field in the destination schema(s).

This webform will also allow the user to insert `source value placeholders` from a `source schema` that tell us what to expect from a triggering event.

	i.e., a trigger event triggers an action, based on a filtering rule defined later:
	
	When *a new patient record is created* in the mobile clinic system,
	Then *create a new outbound SMS record* in the sms gateway.

These are effectively "ingredients" in an If-This-Then-That recipie.

Individual stories will be documented as github issues.

![Image of Layout](https://github.com/OpenFn/visual_mapper/blob/master/layout.png)

Important artifacts:
--------------

1. Destination schema: this defines our HTML form. a composite schema (with several objects) can be found @composite_destination_schema.json

2. Source schema: this is used to mix-in `source value placeholders` (ingredients) to our final action directive. found @sample_source_schema.json

3. A sample "JOLT spec": this is what is currently being used to transform source payloads into destination payloads. found @sample_transform_spec.json

4. a sample source payload to play with: @sample_source_payload.json
5. a sample wished destination payload to aim for: @target_sample_destination_payload.json 
