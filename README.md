# audio_box_qr

## QR code generator :

Use python tools qrcode (https://pypi.python.org/pypi/qrcode)

``` sudo pip install qrcode ```

Required Pillow :

``` sudo pip install -U Pillow ```

example : `qr "mydirectory/myfile.mp3" > title.png`


## CD encoding :

use abcde tool:

``` sudo apt-get install abcde cd-discid lame cdparanoia id3 id3v2 eyed3 ```

remark : it requires postfix package which will prompt for e-mail setting configuration. Ask for no configuration and use [space] to validate your selection.

detail: https://doc.ubuntu-fr.org/abcde

usage :

```
cp /etc/abcde.conf ./
vi abcde.conf
. . .
abcde -c abcde.conf
```

## QR code reader required on your raspberry :

Use zbar tool :

``` sudo apt-get install zbar-tools ```

usage :

``` zbarcam --prescale=300x200 ```	

Put your QR code in front of your webcam --> you should get "mydirectory/myfile.mp3" printed on stdout

In order to be able to use zbar in python code :

``` 
sudo apt-get install libzbar-dev
pip install zbar
```




