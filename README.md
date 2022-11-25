# Verified Schema Definitions

This repository provides definitions for auto-completion and validation of our JSON schemas.

## Usage

Add the `$schema` property with the corresponding definition to your JSON schema.

Example

```
{
    "$schema": "https://raw.githubusercontent.com/verifiedit/verified-schema-definitions/main/services.json",
    "data": {
        "schema": [],
    }

}
```

## Features

### Event driven conditions (@ prefix)

Add an `@` symbol on the `conditions.when` property of a component to make it an event driven condition. The name of the
function can be anything you want, however, must be implemented in each app to work.

Example

```
{
    "component": "TextInput",
    "name": "example",
    "conditions": {
        "do": "fn_submit",
        "on": "example",
        "when": "@click"
    }
}
```
