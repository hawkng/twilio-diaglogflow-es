# twilio-diaglogflow-es
Integrate Twilio Flex with Google Dialogflow <b>ES</b> using <b>WhatsApp</b>

Adpated from Twilio Blog (https://www.twilio.com/blog/flex-dialogflow-cx-digital) which consists of
Twilio Flex + DialogFlow CX via SMS

1. The file <b><i>@google-cloud/dialogflow.protected.js </i></b> need to revised to use ES library

2. Modify package.json to include dialogflow CS library
  ```
"dependencies": {
    "twilio": "^3.56",
    "@twilio/runtime-handler": "1.2.3",
    "@google-cloud/dialogflow": "^5.1.0"
  }
```

3. Once the Twilio Function have been deployed, take down the widget URL and set it up in **Twilio Sandbox for WhatsApp** 
![image](https://user-images.githubusercontent.com/29279065/179699720-da3acff0-9c9c-4cf7-a5d0-c01511539b39.png)

![image](https://user-images.githubusercontent.com/29279065/179699045-792cc210-194a-4bc8-99c2-cb721d8e4720.png)
