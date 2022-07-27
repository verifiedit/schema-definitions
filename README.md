# capture-validate-form-schema
It is a public repository for reference and validating Verified form json schema.

Then, every forms can be referred to this url on form schema validation.

e.g.

```
{
    "$schema": "https://raw.githubusercontent.com/verifiedit/capture-validate-form-schema/main/formSchema.json",
    "data": {
        "schema": [],
    }

}
```

-- Date: July 2022

Introduce @ symbol on "conditions" property - "when" clause, it indicates the condition is an event driven condition.
And, it can execute the function which name is on "do" clause.

e.g.
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
