# Build-A-Bearville Rewritten Validation Schemas

Validation schemas for Build-A-Bearville Rewritten.

## How to Use

To use these validation schemas, you will need to have
a JSON schema validator installed.

You can use libraries such as `ajv` for JavaScript,
`jsonschema` for Python, or any other JSON schema validation library
that supports the JSON Schema standard.

Once you have a validator set up, you can reference the schemas
in your JSON data to validate the structure and content
of your data against the defined schemas.

For example, for using the [`planet.schema.json` schema](./json/game-server/config/planet.schema.json)
and validating a JSON object representing a planet configuration file,
you must add the `$schema` property at the top of your JSON file, like this:

```json
{
    "$schema": "https://raw.githubusercontent.com/Build-A-Bearville-Rewritten/BABVR-Validation-Schemas/main/json/game-server/config/planet.schema.json",
    ...
}
```
