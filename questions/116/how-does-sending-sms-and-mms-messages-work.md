## How does sending SMS and MMS messages work?

- posted by: [DTing](https://stackexchange.com/users/-1/62-dting) on 2011-04-19
- tagged: `technology`, `cell-phone`, `communications`
- score: 5

Does sending SMS and MMS messages use the same towers/frequencies that are used for making cellular calls? Is data from MMS messages transferred via the same frequencies? 

What is the underlying technology/mechanism for these types of messages?


## Answer 119

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-19
- score: 4

SMS stands for Short Message service. It piggy backs off the control channel( which is how the Phone and cell tower communicate) This control channel informs the cell tower that you are still within the cell and the phone when you're receiving a call and then informs what frequencies to use for the voice connection. In SMS sending the senders phone contacts the SMS Gateway( AKA SMSG) and the SMSG sends it off to the tower which forwards it to your phone. Also most SMSGs are Email enabled so you can send an email as a text message to a phone.(For example Verizon Wireless in the US uses PH#@Vtext.com)



---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
