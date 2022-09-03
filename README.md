# Authentication-And-Security
In this modern world of technology where the internet made things available at our fingertips, it also made it hard to secure important data. So I have 
implemented a 6 – Layers of security to make our database safe from intruders.

## Level-1(Using Database)
Using a database to authorize users.

## Level-2 (Database encryption)
To encrypt our user's password we will use mongoose-encryption package for this task. It uses AES-256-CBS with a random,unique initialization vector for each operation.

#### AES - Advanced Encryption Standard
#### CBC - cipher block chaining

## Level-3 (Hashing Password)
While we were encrypting our data we were using a key to encrypt it. If someone found our key then he will be able to decode our data, so in this level we will use the concept of hashing where key is not required. Hashes are unique for same input so when user will try to login and enter his password we wiil generate the hash and we will match it with the stored hash to authorise the user.

#### MD5 (message-digest) algorithm is used here

## Level-4 (Salting and Hashing)
Most users keep their password small and repeatedly uses it everywhere. In this age of super computers small legth passwords can be easily detected so we add some random characters to our password then store it hashed value. It is more secure than just hashing passwords but still it is not enough. Here we use concept of <strong> Salt Rounds </strong> where we hash our already hashed data multiple times.

#### Benefits of this technique-
As the time passes we get more computational power in same amount. So instead of changing hashing algorithm we can just increase <strong>Salt Rounds.</strong> We will use <strong>bcrypt</strong> to implement it.

## Level-5 (Cookies and Sessions)



