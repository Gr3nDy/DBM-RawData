# ![app icon](https://github.com/Gr3nDy/DBM-RawData/blob/master/Package/tokenme/Screenshot/icon.png) TokenMe | Wiki
Here's a few guides of how to customize your **TokenMe** commands;
<br>(Some of these are optional)

# What is i supposed to fill on datatype
you supposed to fill a member data name by doing so it's allowing you to create the data into token <br>
<i>for an Example:</i> `/(datatype1|datatype2|datatype3|datatype4)/` to `/(coin|balance|XP|item|GEMS)/` <br> <em>(REMINDER!!! CASE SENSITIVE)</em>

# How do i change the token length
Edit **Action #95 (Run Script)** & **Action #254 (Run Script)** <br>
`[...Array(9)]` to `[...Array(length)]`

# How do i change my token to look like a steam code
Replace **Action #95 (Run Script)** & **Action #254 (Run Script)** to <br>
```
const ran = [..."ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"];
const com1 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
const com2 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
const com3 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
var chars = com1+"-"+com2+"-"+com3
chars
```
# How do i change the `create` Token Messsage
`create` msg started from **Action #98 (Create Embed Message)**

# How do i change the `gift` Token Messsage
`gift` msg started from **Action #257 (Create Embed Message)**


[Back To TokenMe Page](help.md)
