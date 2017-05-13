## Serverless Alexa City Guide example

### Based codes
https://github.com/alexa/skill-sample-nodejs-city-guide

### Setup

```
$ git clone git@github.com:hideokamoto/serverless-alexa-city-guide.git
$ cd serverless-alexa-city-guide
$ npm install
```

### Run as local

#### LaunchRequest
```
$  sls invoke local -f hello -d '{
  "session":{
    "application":{
      "applicationId":""
    },
    "user":{
      "userId":""
    }
  },
  "request":{
    "type": "LaunchRequest"
  }
}'
```

#### Ask top five

```
$ sls invoke local -f hello -d '{
  "session":{
    "application":{
      "applicationId":""
    },
    "user":{
      "userId":""
    }
  },
  "request":{
    "type":"IntentRequest",
    "intent": {
      "slots": {},
      "name":"getTopFiveIntent"
    }
  }
}'
```
