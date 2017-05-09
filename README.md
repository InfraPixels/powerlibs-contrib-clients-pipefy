# Powerlibs contrib: Pipefy client

A Python client for Pipefy API 


## Installation

```bash
pip install 'https://github.com/DroneMapp/powerlibs-contrib-clients-pipefy.git'
```


## Usage

```python
from powerlibs.contrib.clients.pipefy.client import PipefyClient
from prettyconf import config  # It's just a suggestion.

client = PipefyClient(config('pipefy_email'), config('pipefy_token'), 'https://api.pipefy.com/')
pipe = client.get_pipe(PIPE_ID)

pipe.create_card('Test Card', {
    'Field Label 1': 'Value 1',
    'Field Label 2': 'Value 2',
})
```
