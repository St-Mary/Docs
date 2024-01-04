# SSL Integration

> SSL is a standard security protocol for establishing encrypted links between a server and a browser in an online communication.

## How Luna uses SSL

Luna uses SSL to encrypt the communication between the client and the server. This is done using the <a href="Coral.md">Coral</a> library.

To do this, Luna use a self-signed certificate for now. This certificate is separated into two files: `server.jks` and `client.jks`. The `server.jks` file is used in the server, and the `client.jks` file is used in the client.

<note>
    JKS files are Java KeyStore files. They are used to store certificates and private keys in Java.
</note>