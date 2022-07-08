# opc-cert

Generate Cert Files and Keys Needed for Matrikon OPC Tuneller

The mkcert script can be used to create both the server key for an OPC UA
server and the client key for the Matrikon OPC Tuneller. For example, you
may run the following commands to generate the cert and key files:

	./mkcert server opc-server password
	./mkcert client opc-client password

In each case, the first parameter is the name of the cert and key files,
the second is the host name of the OPC UA endpoint, and the third is the
password to be used to encrypt the key. The cert and key files will be
placed in the certs directory. The cert will be provided in both PEM form
with a crt extension, and DER form with a der extention.


