# twilio-diaglogflow-es
Integrate Twilio Flex with Google Dialogflow <b>ES</b> using <b>WhatsApp</b>

Adpated from Twilio Blog (https://www.twilio.com/blog/flex-dialogflow-cx-digital) which consists of
Twilio Flex + DialogFlow CX via SMS

The simple chatbot is built based on the [How to Build an Appointment Scheduler with Dialogflow Tutorial](https://youtu.be/oU88sHd6ilE?list=PLIivdWyY5sqK5SM34zbkitWLOV-b3V40B)

#### Changes required:

1. Update the code <b><i>@google-cloud/dialogflow.protected.js </i></b> to use ES library

2. Modify **package.json** to include dialogflow CS library
  ```
"dependencies": {
    "twilio": "^3.56",
    "@twilio/runtime-handler": "1.2.3",
    "@google-cloud/dialogflow": "^5.1.0"
  }
```

3. Deploy to Twilio Functions

4. Connect Studio flow to your WhatsApp number ("Sender"), example here using the Sandbox
![image](https://user-images.githubusercontent.com/29279065/179701263-27a869fb-05d0-4954-a027-0f7b853a5217.png)


![image](https://user-images.githubusercontent.com/29279065/179699045-792cc210-194a-4bc8-99c2-cb721d8e4720.png)


5. Update the Widget DialogflowDetectIntent in Twilio Studio with the deployed Twilio Service and Function accordingly.<br/>
   [Sample json](https://github.com/hawkng/twilio-diaglogflow-es/blob/main/studio-sample.json)

#### References:
https://www.twilio.com/docs/studio/tutorials/customer-support-menu#connect-your-whatsapp-sender-to-your-studio-flow

