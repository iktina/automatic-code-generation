# Automatic Code Generation
## Welcome
## What’s the point?
The service receives a textual seed in English and thereafter generates code based on this in one of the programming languages.
You can use this model for several tasks such as:
- code summarization
- code generation
- code translation
- code refinement
- code defect detection
- code clone detection

## Model details:
We use the CodeT5, a unified pre-trained encoder-decoder Transformer model that better leverages the code semantics conveyed from the developer-assigned identifiers.
### The user must provide the following inputs in order to start the service and get a response:
#### Inputs:
`request`: json string

Example of input file content:

`{"start_text": "text", "max_len": 8}`

#### Outputs:
`answer`: json string

Example of output file content:
`{"result": "text"}`

## What to expect from this service?
### Inputs:
`{"start_text": "def greet(user): print(f'hello <extra_id_0>!')", "max_len": 8}`

### Outputs:
`{"result": "{user.username}"}`
