# Glossary

<p>
    This page contains a list of terms used throughout the documentation, and their definitions.
</p>

<deflist type="compact">
    <def title="Packet" id="packet">
        A packet is a message sent between the client and server, to communicate information about the game state such as the player's location.
    </def>
    <def title="BCrypt" id="bcrypt">
        BCrypt is a cryptographic hash function for secure password hashing. It includes salting, resists brute-force attacks with computational intensity, and adapts to hardware advancements.
        <p>The hash output, suitable for secure password storage, includes version, cost factor, salt, and hash. BCrypt is widely used to enhance password security.</p>
    </def>
    <def title="JWT" id="jwt">
        <p>JWT, or JSON Web Token, is a compact and self-contained method for securely transmitting information between parties as a JSON object.</p>
        <p>This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA.</p>
    </def>
    <def title="SSL" id="ssl">
        <p>SSL, or Secure Sockets Layer, is a standard security technology for establishing an encrypted link between a server and a client—typically a web server (website) and a browser, or a mail server and a mail client (e.g., Outlook).</p>
        <p>SSL allows sensitive information such as credit card numbers, social security numbers, and login credentials to be transmitted securely. Normally, data sent between browsers and web servers is sent in plain text—leaving you vulnerable to eavesdropping.</p>
        <p>If an attacker is able to intercept all data being sent between a browser and a web server, they can see and use that information.</p>
    </def>
    <def title="Netty" id="netty">
        <p>Netty is an asynchronous event-driven network application framework for rapid development of maintainable high performance protocol servers &amp; clients.</p>
        <p>In other words, Netty is a NIO client server framework which enables quick and easy development of network applications such as protocol servers and clients.</p>
        <p>It greatly simplifies and streamlines network programming such as TCP and UDP socket server.</p>
    </def>
    <def title="The Protocol" id="protocol">
        <p>The Protocol is the manager of the packets sent between the client and server. It contains a list of all the packets, and their identifiers, and manage if a packet is valid or not.</p>
        <p>We use it to verify if the packet sent by the client is valid, and if it is, we execute the code linked to this packet.</p>
    </def>
    <def title="The Database" id="database">
        <p>Saint Mary's Gate uses a PostgreSQL database to store all the data.</p>
        <p>PostgreSQL is a free and open-source relational database management system emphasizing extensibility and SQL compliance.</p>
    </def>
</deflist>