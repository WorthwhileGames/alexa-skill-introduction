## Alexa Skill Introduction

### Install and Test
- `npm install`
- `npm run test` (node testflow.js)

### aws-config.json
- in order to run/test the code:
- - Copy data/aws-config-template.json and rename it aws-config.json
- - Edit the appId field
```
{
    "region": "us-east-1",
    "appId": "[your skill's app id]"
}
```

### testflow.js
- provided by amazon in the alexa-cookbook repo
- invokes the intents specified in dialogs/default.txt
- - https://github.com/alexa/alexa-cookbook/tree/master/testing/TestFlow

- requests a valid alexa skill/app id (optional)
```
var appId = '[your skill's app id]';
```

### Speech Assets
- not part of the lambda build/test process but are helpful when creating the skill
- speechAssets/InteractionModel.json (can be pasted into a new skill)
- speechAssets/SampleUtterances.txt

### Deploy
- copy lib/index.js to the lambda code editor
- (or set up the aws CLI ...)
