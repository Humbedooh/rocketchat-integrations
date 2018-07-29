## Datadog Integration: Installation steps:

* Set up the integration in rocket.chat using the `incoming.js` file in this folder as the script
* Get the webhook URL from rocket.
* Add the WebHooks integration at [https://app.datadoghq.com/account/settings#integrations](https://app.datadoghq.com/account/settings#integrations)
* Use the following custom payload:
  ~~~
     {"host": "$HOSTNAME", "type": "$EVENT_TYPE", "title": "$EVENT_TITLE", "body": "$EVENT_MSG"}
  ~~~
* Name your webhook `rocketchat`
* Set the webhook URL to the one you got in step 2
* Add the webhook to metrics by referencing it as `@webhook-rocketchat`
* Done!
