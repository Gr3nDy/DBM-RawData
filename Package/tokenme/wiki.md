# ![app icon](https://github.com/Gr3nDy/DBM-RawData/blob/master/Package/tokenme/Screenshot/icon.png) TokenMe | Wiki
# FAQ
Here's a list of Frequently asked questions regarding **TokenMe**;

# <h3>1. how do i fix "ERROR: The action does not exist!"</h3>
This means you're missing an action/mod please updgrade your DBM to Beta and install Mods,
You can find mods on DBM Network Server

# <h3>2. it gives me "Invalid Datatype" everytime i create a token</h3>
Make sure you put a correct configuration on datatype section [Here](./wiki.md#1-what-is-i-supposed-to-fill-on-datatype).
if you think you already put the configuration correctly and it's still doesn't work it might be your "Check Variable" Mod is might be outdated since the command is using "Match Full regex" which you can only get on _betamods_

# Customization
Here's a few guides of how to customize your **TokenMe** command;
<br>(Some of these are optional)

# <h3>1. What is i supposed to fill on datatype</h3>
you supposed to fill a member data name by doing so it's allowing you to create the data into token <br>
<i>for an Example:</i> `/(datatype1|datatype2|datatype3|datatype4)/` to `/(coin|balance|XP|item|GEMS)/` <br> <em>(REMINDER!!! CASE SENSITIVE)</em>
<br>
<br>
the format for `datatype` would be; `/()/`
<br>inserting invalid format might make the command not function

# <h3>2. How do i change the token length</h3>
Edit **Action #95 (Run Script)** & **Action #254 (Run Script)** <br>
`[...Array(9)]` to `[...Array(length)]`

# <h3>3. How do i change my token to look like a steam code</h3>
Replace **Action #95 (Run Script)** & **Action #254 (Run Script)** to <br>
```
const ran = [..."ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"];
const com1 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
const com2 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
const com3 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
var chars = com1+"-"+com2+"-"+com3
chars
```
# <h3>4. How do i change the `create` Token Messsage</h3>
`create` msg started from **Action #98 (Create Embed Message)**

# <h3>5. How do i change the `gift` Token Messsage</h3>
`gift` msg started from **Action #257 (Create Embed Message)**


[Back To TokenMe Page](help.md)
