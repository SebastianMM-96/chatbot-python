# Creating a personality

- Difference between a command line app and a chatbot. 

- Makes chatbots and voice assistants more accessible to use. 

## Smalltalk

```
responses = {
    "what's your name?" : "my name is Bot",
    "what's the weather today?" : "it's sunny!"
}
```

```
def respond(message):
    if message in response:
        return responses[message]

respond("what's your name?")
```

## Including variables

```
responses = {
    "what's the weather today?" : "it's {} today!"
}

weather_today = "cloudy"

def respond(message):
    if message in response:
        return responses[message].format(weather_today)

respond("what's the weather today?")
```