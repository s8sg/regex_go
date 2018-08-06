## regex_go - OpenFAAS function to check Regex
[![OpenFaaS](https://img.shields.io/badge/openfaas-serverless-blue.svg)](https://www.openfaas.com)
    
This is build as a dummy app to check openfaas-cloud and Status integration with openfaas deployed at: 
`https://6803677a.ngrok.io` and can be reached at `https://6803677a.ngrok.io/function/s8sg-regex_go` and `https://6803677a.ngrok.io/function/s8sg-regex_py`




    
**Example:**
```
$ curl -H "Content-Type: application/json" -X POST http://0341c281.ngrok.io/function/s8sg-regex_go -d '{"data": "The moon is our natural satellite, i.e. it rotates around the Earth!", "regex": "(\\b[^\\s]+\\b)" }'
{
  "match": true,
  "matches": [
    "The",
    "moon",
    "is",
    "our",
    "natural",
    "satellite",
    "i.e",
    "it",
    "rotates",
    "around",
    "the",
    "Earth"
  ]
}

$ curl -H "Content-Type: application/json" -X POST http://0341c281.ngrok.io/function/s8sg-regex_py -d '{"data": "The moon is our natural satellite, i.e. it rotates around the Earth!", "regex": "(\\b[^\\s]+\\b)" }'
{
  "match": true,
  "matches": [
    "The",
    "moon",
    "is",
    "our",
    "natural",
    "satellite",
    "i.e",
    "it",
    "rotates",
    "around",
    "the",
    "Earth"
  ]
}
```

