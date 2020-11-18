# Robust language understanding with rasa NLU

## Rasa NLU

- Library for intent recognition & entity extraction
- Built in support for chatbot specific task

## Rasa data format

```
from rasa_nlu.converts import load_data
import json

training_data = load_data('./training_data.json')
print(json.dumps(data.training_example[22], indent=2))
```

## Interpreters

```
message = "I want to book a flight to London"
interpreter.parse(message)
```

## Rasa usage

```
from rasa_nlu.config import RasaNLUConfig
from rasa_nlu.model import Trainer

config = RasaNLUConfig(
    cmdline_args = {"pipeline": "spacy_sklearn"}
)
trainer = Trainer(config)
interpreter = trainer.train(training_data)
```

### About Rasa NLU

Rasa NLU (Natural Language Understanding) is a tool for understanding what is being said in short pieces of text.