![wirvsviruslogo](https://wirvsvirushackathon.org/wp-content/uploads/2020/03/12-scaled.jpg, "WirVsVirus Hackathon")

# WirVsVirus Hackathon Projekt

This repository is part of a submission to the [WirVsVirus Hackathon](https://wirvsvirushackathon.org/) and aims to classify the infection risk of people in need before it connects them to a contact center. This project uses [Twilio](https://twilio.com) for connectivity via the telephony network (phone, sms) as well as WhatsApp. Incoming requests are routed to [Dialogflow](https://dialogflow.com) for natural language processing and intent detection, a classification is performed on a custom backend (see related repositories). The request is then sent to [Twilio Flex](https://twilio.com/flex), a fully programmable contact center that was modified to serve the needs of an ad-hoc crisis response center.

# Related repositories
- [Backend (node)](https://github.com/andrej-s/wirvsvirus-backend) used for the classification of callers and as fulfillment server for dialogflow requests
- [Frontend (React)](https://github.com/andrej-s/wirvsvirus-frontend), a React Component used to modify Twilio Flex
- [Config (Twilio Studio, Dialogflow)](https://github.com/andrej-s/wirvsvirus-config), configuration files for both platforms used

## Setup
- Create an account for [Dialogflow](https://dialogflow.com) and import files from the folder `/google-dialogflow`
- Create an account for [[Twilio](https://twilio.com), create a Flex instance and import files from the folder `/twilio-studio` in Studio