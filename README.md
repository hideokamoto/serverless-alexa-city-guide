## Serverless Alexa City Guide example

### Based codes
https://github.com/alexa/skill-sample-nodejs-city-guide

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
