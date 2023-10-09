# py_sign_verify
Python Sign and Verify Script

Python script to Sign a binary as well as verify the signature.

Usage:
            digi-sig -s  <priv-key> <data> <signature-file>
            digi-sig -v  <PUB-key> <data> <signature-file> 
  
--------------------------------------------
Command For Create Pubkey and Private:

openssl req -new -x509 -newkey rsa:2048 -keyout Private.out -pubkey -out Pubkey.out -days 365 -nodes -sha256

--------------------------------------------
Run the File :

python .\digi-sig.py -s .\Private.out .\myFile.txt signature.out
python .\digi-sig.py -v .\pub.out .\myFile.txt signature.out

--------------------------------------------
Source Video:

https://www.youtube.com/watch?v=b2pj0yDhDp4&ab_channel=SameerPasha

--------------------------------------------
Install pycrypto :

    pip uninstall pycrypto
    pip install pycryptodome

--------------------------------------------
