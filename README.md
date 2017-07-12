## Linux to Slack
Send messages or contents of a file to slack from a terminal

To use this, you need to get the webhook link for your slack account. Instructions on getting the webhook link below,
- https://www.programmableweb.com/news/how-to-integrate-webhooks-slack-api/how-to/2015/10/20
- Go to the section titles "Incoming Webhook Integration Setup"
- Choose the channel which you would like to create a webhook URL for.
- Copy the 'Webhook URL' and save it somewhere

Clone this repo to your local directory.

Open the script named 'linux_to_slack.sh' and replace WEBHOOK_URL with your URL.

Provide permissions and execute the script,
```
chmod +x linux_to_slack.sh
./linux_to_slack.sh "<your_message>"
```

To send the contents of a file to slack,
So the command would be,
```
./linux_to_slack.sh "`cat <file_name>`"
```


