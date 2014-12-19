# Selenium: Delete all messages in #general

![deleteslack](https://cloud.githubusercontent.com/assets/690703/5504929/9bd23af6-87c5-11e4-8ecf-377c09b3f3ba.gif)

## Problem

**May I delete entirely purge messages in #general channel?**
- The answer is NO. **ಠ_ಠ**

Below is the response from slack support team: (2014/12/19):
> You can bulk delete messages in batches of up 100 at a time from the archives page for a channel or group: https://my.slack.com/archives — the first time you use delete you'll be able to select up to 10 messages, but on subsequent attempts you'll be able to select up to 100.

## Solution

### Prerequisite
- [Firefox](https://www.mozilla.org)
- [selenium-ide-x.x.x.xpi](http://www.seleniumhq.org/download/) - Selenium IDE
- Selenium Scripts
  - [sideflow.js](https://raw.githubusercontent.com/darrenderidder/sideflow/master/sideflow.js) - A Selenium Core Extenstion
  - [deleteslacklog.html](https://raw.githubusercontent.com/imZack/slack-delete-all-general-chat-log/master/deleteslacklog.html) - A Selenium Test Case, we use it for delete all messages.
- Install Selenium just simply drag-and-drop `selenium-ide-x.x.x.xpi` into Firefox
- You are ready to go!

### Start
- Open https://my.slack.com/archives/general via Firefox
- Open Selenium IDE
  - Setup `Selenium Core Extenstion` in `options->general` choose `sideflow.js` and restart Selenium IDE.
  - Open Test(script) `ctrl-o` select `deleteslacklog.html` you have downloaded.
- Click the play button and take a coffee :coffee:


:tada:~ Now you have a whole new **#general** channel!
<a href="https://cloud.githubusercontent.com/assets/690703/5500537/4be018ea-8781-11e4-8daf-ff1fcedb3cc8.png" target="_blank">
<img width="500px;" src="https://cloud.githubusercontent.com/assets/690703/5500537/4be018ea-8781-11e4-8daf-ff1fcedb3cc8.png">
</a>


# License
MIT: http://yulun.mit-license.org
