# Authentication-And-Security
In this modern world of technology where the internet made things available at our fingertips, it also made it hard to secure important data. So I have 
implemented a 6 – Layers of security to make our database safe from intruders.

## Level-1(Using Database)
Using a database to authorize users.

## Level-2 (Database encryption)
To encrypt our user's password we will use mongoose-encryption package for this task. It uses AES-256-CBS with a random,unique initialization vector fro each operation.

#### AES - Advanced Encryption Standard
#### CBC - cipher block chaining

## Level-3 (Hashing Password)
While we were encrypting our data we were using a key to encrypt it. If someone found our key then he will be able to decode our data, so in this level we will use the concept of hashing where key is not required. Hashes are unique for same input so when user will try to login and enter his password we wiil generate the hash and we will match it with the stored hash to authorise the user.

#### MD5 (message-digest) algorithm is used here



