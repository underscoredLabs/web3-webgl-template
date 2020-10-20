# web3-webgl-template

Article: https://medium.com/@leondo/unity-engine-metamask-wallet-6797d4699e45

Automagically connect your Unity game to Metamask

![Screen Shot 2020-10-19 at 9 53 06 PM](https://user-images.githubusercontent.com/19412160/96530472-87839600-1255-11eb-8db4-3139f2eadde5.png)

## How to use

Create a folder called `WebGLTemplates` under `/Assets`

Download `Web3Template` from here and paste under `WebGLTemplates`

![Screen Shot 2020-10-19 at 9 52 00 PM](https://user-images.githubusercontent.com/19412160/96530476-8a7e8680-1255-11eb-99ad-2e816cd5a06d.png)

In Unity

![Screen Shot 2020-10-19 at 9 42 27 PM](https://user-images.githubusercontent.com/19412160/96530483-8c484a00-1255-11eb-81ee-fcfcd3f8330c.png)

Change template

![Screen Shot 2020-10-19 at 9 41 36 PM](https://user-images.githubusercontent.com/19412160/96530489-8e120d80-1255-11eb-8e27-c6d8f0cb3dc1.png)

Build as webgl

## Under the hood

```javascript
// Web3Template/TemplateData/web3Connect.js

if (window.ethereum) {
  web3 = new Web3(window.ethereum);
  // connect popup
  ethereum.enable();
} else {
  alert("Non-Ethereum browser detected. Please connect to a wallet");
}
```
