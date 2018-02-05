# Using qrcode.min.js
Implementing qrcode.min.js as it is for qr code display output for long encoded strings. 
# Reasons:
## 1)
Minimize client side javascript runtime. All non-esential features have been removed.
## 2)
Using PHP on the serverside, HTML/Javascript is sent to the client to display long and complicated hashes and encrypted strings. These codes cannot be edited in the client browser.
## Basic Use:
``
<div id="qrcode"></div>
<script type="text/javascript">
var qrcode = new QRCode(document.getElementById("qrcode"), {
	text: "http://jindo.dev.naver.com/collie",
	width: 128,
	height: 128,
	colorDark : "#000000",
	colorLight : "#ffffff",
	correctLevel : QRCode.CorrectLevel.H
});
</script>
``
## Optional methods:
``
qrcode.clear(); // clear the code.
qrcode.makeCode("http://naver.com"); // make another code.
``
## Browser Compatibility
IE6~10, Chrome, Firefox, Safari, Opera, Mobile Safari, Android, Windows Mobile, ETC.

## License
MIT License

## Contact
snailtrail@didlie.com

### Implentation:
https://www.didlie.com
