# Set up SSL Certificates

Currently, this project use a self-signed certificate. This is not secure, and should be replaced with a proper certificate.

## How to generate a self-signed certificate

<procedure id="ssl-generation">
    <step>
        Generate the self-signed certificate:
        <code-block lang="shell">
            openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365
        </code-block>
    </step>
    <step>
        Create jks file for server (it will need private key included):
        <code-block lang="shell">
             keytool -import -v -trustcacerts -alias client-alias -file cert.pem -keystore client.jks -keypass tutorial123 -storepass tutorial123
        </code-block>
    </step>
    <step>
        Create jks file for server (it will need private key included):
        <code-block lang="shell">
             openssl pkcs12 -export -in cert.pem -inkey key.pem -certfile cert.pem -out keystore.p12
 keytool -importkeystore -srckeystore keystore.p12 -srcstoretype pkcs12 -destkeystore server.jks -deststoretype JKS
        </code-block>
    </step>
</procedure>

This will generate a self-signed certificate that will be valid for 365 days.

> Note: The password used in this example is `tutorial123`. This should be changed to something more secure.

These two .jks files will be used in the server and the client.
The `client.jks` file will be used in the client, and the `server.jks` file will be used in the server.
Both of these files should be placed in a folder called `ssl` in the root of their respective projects.