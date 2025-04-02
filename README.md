# RSA-Factoring-Challenge

![undraw_programming_re_kg9v](https://user-images.githubusercontent.com/110098940/219950176-b01d033c-dde0-4727-879b-cfe5575af5e0.png)

| PR.NO | PROJECT                                                                           | DESCRIPTION |
| ----- | --------------------------------------------------------------------------------- | ----------- |
|  🗂️  | [Tests 📁](./tests/)                                            | The "tests" folder in the RSA Factory challenge includes scripts to validate the RSA algorithm's functionality, covering encryption, decryption, key generation, prime number checks, and edge cases. It ensures the implementation is correct and efficient.          |
| 0x00  | [Factor](./factor.c/)                                         | The Factor.c file implements functions for prime factorization and primality testing, which are crucial for generating RSA keys and ensuring the security of the encryption process. It helps in breaking down large numbers and verifying their primality.            |
| 0x01  | [Factors](./factors/)                                         | The Factors file in the RSA Factory challenge likely contains functions related to factoring large numbers, such as finding prime factors and testing for primality. These functions are essential for tasks like RSA key generation and breaking down numbers used in encryption.            |
| 0x02  | [Rsa](./rsa/)                                                 | contains the core implementation of the RSA encryption and decryption algorithm. It includes functions for key generation (public and private keys), encryption, and decryption. The file also handles the mathematical operations required for RSA, such as modular exponentiation and the use of large prime numbers.  |
| 0x03  | [Rsa.c](./rsa.c/)                                             | The RSA.c file contains the implementation of the RSA encryption algorithm, including functions for key generation, encryption, and decryption. It handles essential operations like modular exponentiation and uses prime numbers for secure key creation.            |
| 0x04  | [Test](./test1/)                                              | contains a set of initial tests to verify the functionality of the RSA algorithm. It may check basic operations like key generation, encryption, and decryption to ensure the algorithm works correctly on a small scale before testing larger numbers or more complex scenarios.            |
| 0x05  | [Wfactors](./wfactors.py/)                                    |  contains functions for handling the factorization of large numbers, particularly for finding prime factors. It may include tools for efficiently factorizing numbers and testing for primality, which are important for tasks like key generation and breaking down RSA-encrypted data.           |

## Description
The RSA Factoring Challenge is a cryptographic challenge that involves factoring large semiprime numbers (numbers that are the product of two primes). The goal is to break RSA encryption by factoring these large numbers, which is central to the security of RSA. The challenge provides several large RSA-modulus values, and the task is to find their prime factors. Success in factoring these numbers undermines the RSA encryption system, demonstrating the importance of using sufficiently large primes for key generation.

This project is designed to factorize as many numbers as possible into a product of two smaller numbers.
It works perfectly for that except the case of bignums (numbers bigger than long long unsigned integers)
please any contribution towards making this project work for bignums will be highly appreciated.

## Information

- HTTPS uses Secure Socket Layer to encrypt data that is transferred between client and server. SSL uses the RSA algorithm, an asymmetric encryption technology. The precise details of how the algorithm works is complex, but basically it leverages the fact that whilst multiplying two large prime numbers together is easy, factoring the result back into the constituent primes is very, very hard. How all SSL/RSA encryption works is:

- The server generates two large prime numbers, and multiplies them together. This is called the "public key". This key is made available to any client which wishes to transmit data securely to the server. The client uses this "public key" to encrypt data it wishes to send. Now because this is an asymmetric algorithm, the public key cannot be used to decrypt the transmitted data, only encrypt it. In order to decrypt, you need the original prime numbers, and only the server has these (the "private key"). On receiving the encrypted data, the server uses its private key to decrypt the transmission.

- In the case of you browsing the web, your browser gives the server its public key. The server uses this key to encrypt data to be sent to your browser, which then uses its private key to decrypt.

- So yes all data transmitted to/from server over HTTPs is encrypted and encrypted well. Typical SSL implementations use 128 or 256 digits for their keys. To break this you need a truly vast amount of computing resources.

## Tasks

## Resources

- [RSA](<https://en.wikipedia.org/wiki/RSA_(cryptosystem%29)>)
- [How does HTTPS provide security?](https://stackoverflow.com/questions/3968095/how-does-https-provide-security)
- [Prime Factorization](https://privacycanada.net/mathematics/prime-factorization/)

### AUTHOR:
<details>
    <summary>KARLIE MOYO</summary>
    <ul>
        <li>
            <a href="https://github.com/karlie-moyo">Github</a>
        </li>
        <li>
            <a href="https://twitter.com/karlieemoyo">Twitter</a>
        </li>
        <li>
            <a href="https://karlieemoyo@gmail.com">e-mail</a>
        </li>
    </ul>
</details>

---

### Acknowledgements  :pray:
___
All of the work in this project was conducted as part of the UoS-SE program's curriculum.
