# Custom OpsGenie slack integration

This app will be deployed in heroku with scheduler, automatically send on-call rotation notification to team channel

## what you need?
- OpsGenie team integration API key. Team admin can create team level WEB API integration, and you get the key from there.
- A Slack webhook url, you need to use slack workflow builder tool to create a workflow, it will generate a unique webhook URL, 
you will call that URL to trigger the workflow. 
In our case, just send a message to a channel. You can do more with the builder.
- A free Heroku account, you will use heroku scheduler to run a task


### Note
You can skip the bot code, only one file is in use - `bin/opsgenie-oncall`.  
