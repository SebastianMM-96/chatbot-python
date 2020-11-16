# EchoBot I

We will be learning how to build chatbots in Python by writing two functions to build the simplest bot possible: EchoBot. EchoBot just responds by replying with the same message it receives.

```
def respond(message):
    return "I can hear you!. You said: {}".format(message)
def send_message(message):
    # calls respond() to get respond

send_message('hello')
```