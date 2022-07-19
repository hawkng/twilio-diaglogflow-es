# twilio-diaglogflow-es
Integrate Twilio Flex with Google Dialogflow <b>ES</b> using <b>WhatsApp</b>

Adpated from Twilio Blog (https://www.twilio.com/blog/flex-dialogflow-cx-digital) which consists of
Twilio Flex + DialogFlow CX via SMS

#### Changes required:

1. The file <b><i>@google-cloud/dialogflow.protected.js </i></b> need to revised to use ES library

2. Modify **package.json** to include dialogflow CS library
  ```
"dependencies": {
    "twilio": "^3.56",
    "@twilio/runtime-handler": "1.2.3",
    "@google-cloud/dialogflow": "^5.1.0"
  }
```

3. Connect Studio flow to your WhatsApp number ("Sender"), example here using Whatsapp Sandbox
![image](https://user-images.githubusercontent.com/29279065/179701263-27a869fb-05d0-4954-a027-0f7b853a5217.png)


![image](https://user-images.githubusercontent.com/29279065/179699045-792cc210-194a-4bc8-99c2-cb721d8e4720.png)


4. Update the Widget DialogflowDetectIntent with the deployed Twilio Service and Function accordingly.


#### References:
https://www.twilio.com/docs/studio/tutorials/customer-support-menu#connect-your-whatsapp-sender-to-your-studio-flow
