# Incremental slot filling and negation

## Basic Memory

```
def respond(message, params):
    # update params with entities in message
    # run query
    # pick response
    return response, params

# initial params
params = {}

# messages come in
response, params = respond(message, params)
```