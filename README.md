# Linux_Signing_Cert
This public key allows users to verify the veracity of the Acronis SCS Linux installer. 

# Verify Example

Download AcronisSCSIntCA.pub.pem, Sample.txt and Sample.txt.sha256 files

Place AcronisSCSinCA.pub.pem, Sample.txt.sha256, and Sample.txt in the same folder location

Run the following command:
`openssl dgst -sha256 -verify AcronisSCSIntCA.pub.pem -signature Sample.txt.sha256 Sample.txt`

You will see "Verified OK"