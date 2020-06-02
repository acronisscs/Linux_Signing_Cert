# Linux_Signing_Cert
This public key allows users to verify the veracity of the Acronis SCS Linux installer. 

# Verify Example

Download AcronisSCS.pub.asc, Sample.txt, Sample.txt.gpg and Sample.txt.sig files into the same folder

Import the AcronisSCS.pub.asc public key into your local key ring.
`gpg --import AcronisSCS.pub.asc`


Run the following command:
`gpg --verify Sample.txt.sig Sample.txt`

You will see output similar to:

gpg: Signature made Wed, May 20, 2020  2:49:49 PM USMST
gpg:                using RSA key A042B6B30A7F4302
gpg: Good signature from "Acronis SCS <**@acronisscs.com>" [unknown]
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: 43DA 4FE5 7AF4 3AF2 D40F  D377 A042 B6B3 0A7F 4302


You can also run this command:
`gpg --verify Sample.txt.gpg`

You will see output similar to:

gpg: Signature made Wed, May 20, 2020  3:13:03 PM USMST
gpg:                using RSA key A042B6B30A7F4302
gpg: Good signature from "Acronis SCS <**@acronisscs.com>" [unknown]
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: 43DA 4FE5 7AF4 3AF2 D40F  D377 A042 B6B3 0A7F 4302
