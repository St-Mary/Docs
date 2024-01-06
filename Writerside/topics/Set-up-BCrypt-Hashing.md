# BCrypt Hashing

## What is BCrypt Hashing?

<note>
    See <a href="Glossary.md#bcrypt">BCrypt</a> to understand what BCrypt is.
</note>

## Why do we need BCrypt Hashing?

For security and confidentiality reasons, Saint Mary's Gate never stores passwords in clear text in its database.

This is a very bad practice, because if a hacker manages to access the database, he will have access to all the passwords of all the players.

Instead, it stores a Hash, a password encrypted using the BCrypt algorithm, which uses a private key called Salt.


## How to set up BCrypt Hashing?


<procedure>
<step>
Create a key for the BCrypt salt. This key must be unique and secret. It is recommended to use a random string generator to create this key.
</step>
<step>
You need to include the following key in Luna's `.env` file:

```
PASSWORD_SALT=your_salt
```
</step>
</procedure>

<seealso>
    <category ref="related">
        <a href="Glossary.md">Glossary</a>
    </category>
</seealso>