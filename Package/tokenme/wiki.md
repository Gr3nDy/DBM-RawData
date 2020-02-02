# ![app icon](https://github.com/Gr3nDy/DBM-RawData/blob/master/Package/tokenme/Screenshot/icon.png) TokenMe | Wiki
Here's a few guides of how to customize your **TokenMe** commands (Optional);

# How do i change the token length
Edit **Action #95 (Run Script)** & **Action #254 (Run Script)** <br>
`[...Array(9)]` to `[...Array(length)]`

# How do i change my token to look like steam code
Replace **Action #95 (Run Script)** & **Action #254 (Run Script)** to <br>
```
const ran = [..."ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"];
const com1 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
const com2 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
const com3 = [...Array(6)].map(i=>ran[Math.random()*ran.length|0]).join``;
var chars = com1+"-"+com2+"-"+com3
chars
```


[Back To TokenMe Page](https://github.com/Gr3nDy/DBM-RawData/edit/master/Package/tokenme/help.md)
