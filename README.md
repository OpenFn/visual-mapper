# visual_mapper

Objective
-----------
Open-source Zapier/IFTTT "mapping generator" to provide automation services to the international development sector—current projects are in public health, agriculture, and education.

Stories will be documented as github issues. The epic is this:
-------------------------
1. Given a schema in "JSON-schema" the user wants to be able to define an action (create or update records) in a destination database.

We'd like to use JSON-editor (https://github.com/jdorn/json-editor) to present the user with an HTML webform to define the insert/update action.

This webform will allow the user to type values for each field in the destination schema(s).

This webform will also allow the user to insert `placeholders` from a `source schema` that tells us what to expect from a triggering event.

	i.e., When a new patient record is created in the mobile clinic system, create a new outbound SMS record in the sms gateway.

These are effectively "ingredients" in an If-This-Then-That recipie.