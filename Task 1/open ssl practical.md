OpenSSL Practical — Encrypt and Decrypt

Run these commands in Kali Linux:

openssl version
mkdir -p ~/openssl-lab
cd ~/openssl-lab
echo "My first encryption lab" > message.txt


Encrypt the message:
openssl enc -aes-256-cbc -salt -pbkdf2 \
-in message.txt -out encrypted.bin


Decrypt it:
openssl enc -d -aes-256-cbc -pbkdf2 \
-in encrypted.bin -out decrypted.txt


Verify the result:
cat decrypted.txt
diff -s message.txt decrypted.txt


Enter the same password during encryption and decryption. For real applications, authenticated encryption such as AES-GCM is generally preferable to unauthenticated CBC encryption.