## NodePing Integration - Installation Steps:

* Add the integration in rocket.chat with `incoming.js` as the script, get the webhook URL
* Log onto your nodeping account
* Go to `Checks & Contacts`
* Add a new contact, use `webhook` and set method to `POST`
* Set the URL to the one you got from rocket
* Set the `body` parameter in your webhook to:
  ~~~
  {"label":"{label}","event":"{event}","target":"{target}"}
  ~~~
* All done!
