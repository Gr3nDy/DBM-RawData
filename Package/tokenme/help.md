# ![app icon](./blob/master/Package/tokenme/Screenshot/icon.png) TokenMe

Convert <b>Member Data</b> into a reedemable <b>Token</b>

<b>Usage</b>
* `[p]token create <datatype> <value> <duration>`
* `[p]token gift <user> <datatype> <value> <duration>`
* `[p]token list`
* `[p]token check <token>`
* `[p]token delete <token>`
* `[p]redeem <token>`

# Installation

<b>Commands</b>

* [TokenMe](https://raw.githubusercontent.com/Gr3nDy/DBM-RawData/master/Package/tokenme/Commands/tokenme.json)
* [Redeem](https://raw.githubusercontent.com/Gr3nDy/DBM-RawData/master/Package/tokenme/Commands/redeem.json)

<b>Events</b>

* [Loop 1](https://raw.githubusercontent.com/Gr3nDy/DBM-RawData/master/Package/tokenme/Events/Loop%201.json)
* [Loop 2](https://raw.githubusercontent.com/Gr3nDy/DBM-RawData/master/Package/tokenme/Events/Loop%202.json)
<br>

Copy <b>Commands</b> & <b>Events</b> and import to
DBM.
* 1.Create New Command
* 2.Right click the command
* 3.Select Edit Raw Data
* 4.Paste Raw Data
* 5.Click on save

# Customization

<b>Commands:</b>

<b>Token</b>
* Put your <b>Log Channel ID</b> to <strong>Action #6 (Find Channel)</strong> 
* Edit <strong>Action #8 (Run Script)</strong>  and add any member data you'd like to be able to create token for an example `/(data1|data2|data3|data4)/g` (REMINDER! CASE SENSITIVE)
* Edit <strong>Action #241 (Set Embed Description)</strong> and put your <b>Bot Channel ID</b>

<b>Events:</b>

<b>Loop 1</b>
* On <strong>Action #2 (Loop Through List)</strong> Set it to call Event <b>Loop 2</b> (By default it's already set to Loop 2)

<b>Loop 2</b>
* Put your <b>Log Channel ID</b> to <strong>Action #6 (Find Channel)</strong>
