# Encryption_Decryption
A command line application which can encrypt/decrypt strings using various encryption algorithms.

ABOUT

Today, encryption and decryption algorithms are used everywhere on the Internet to protect our data. This is especially important
for sites that handle sensitive data, such as e-commerce sites that accept online card payments and login areas that 
require users to enter their credentials. To ensure data security, there are complex encryption algorithms behind the scenes.

DESCRIPTION

The program must parse three arguments: -mode, -key and -data. The first argument should determine the program’s mode (enc for encryption, dec for decryption).
The second argument is an integer key to modify the message, and the third argument is a text or ciphertext to encrypt or decrypt.
The arguments -in and -out specify the full name of a file to read data and to write the result
When starting the program, the necessary algorithm should be specified by an argument (-alg). The first algorithm should be named shift, the second one 
should be named unicode. If there is no -alg it will default it to shift.

All the arguments are guaranteed to be passed to the program. If for some reason it turns out to be wrong:

    If there is no -mode, the program works in enc mode.
    If there is no -key, the program considers that key = 0.
    If there is no -data, the program assumes that the data is an empty string.
    If there is no -out argument, the program prints data to the standard output.
    If there are both -data and -in arguments, the program prefers -data over -in.

Keep in mind that the order of the arguments might be different. For example, -mode enc may be at the end, 
at the beginning or in the middle of arguments array.
