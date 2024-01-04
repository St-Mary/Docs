# Packets

> All packets are sent using the [Coral](https://github.com/st-mar/Coral) library.

## Packet Structure

<note>
    See <a href="Glossary.md#packet">Packet</a> to understand what a packet is.
</note>

All packets contain an identifier, which is a single byte to identify the packet type.

<seealso>
    <category ref="related">
        <a href="Networking.md">Networking</a>
        <a href="Glossary.md">Glossary</a>
    </category>
</seealso>

## Packet List

Here is a list of all the packets, and their identifiers.

| Identifier | Packet Name             | Description                                                                                      |
|------------|-------------------------|--------------------------------------------------------------------------------------------------|
| `1`        | `version`               | This packet is used to compare Luna and Cassandra versions to check if the client is up-to-date. |
| `2`        | `versionresult`         | The packet sent by the server to tell the client if it is up-to-date or not.                     |
| `3`        | `loginusingcredentials` | This packet is used to login with credentials (username, password) to the server.                |
| `4`        | `loginusingjwt`         | This packet is used to login with a JWT token to the server.                                     |
| `5`        | `loginresult`           | The packet sent by the server to tell the client if the login was successful or not.             |