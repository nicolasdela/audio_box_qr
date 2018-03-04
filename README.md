# audio_box_qr

## QR code generator :

Use python tools qrcode (https://pypi.python.org/pypi/qrcode)
	```
	sudo pip install qrcode
	```

Required Pillow :
	```
	sudo pip install -U Pillow
	```

example : `qr "mydirectory/myfile.mp3" > title.png`
	

## QR code reader :

Use zbar tool :
	```
	sudo apt-get install zbar-tools
	```

usage :
	```
	zbarcam --prescale=300x200
	```	
	Put your QR code in front of your webcam --> you should get "mydirectory/myfile.mp3" printed on stdout
