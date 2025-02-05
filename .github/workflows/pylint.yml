
def caesar_cipher_encrypt(plaintext, key):
    encrypted_text = ""

    for char in plaintext:
        if char.isalpha():
            shift_base = ord('A') if char.isupper() else ord('a')
            encrypted_text += chr((ord(char) - shift_base + key) % 26 + shift_base)
        else:
            encrypted_text += char  # Non-alphabetic characters remain unchanged

    return encrypted_text

def caesar_cipher_decrypt(ciphertext, key):
    decrypted_text = ""

    for char in ciphertext:
        if char.isalpha():
            shift_base = ord('A') if char.isupper() else ord('a')
            decrypted_text += chr((ord(char) - shift_base - key) % 26 + shift_base)
        else:
            decrypted_text += char  # Non-alphabetic characters remain unchanged

    return decrypted_text

# Example usage
plaintext = "Hello, World!"
key = 3

# Encrypt
ciphertext = caesar_cipher_encrypt(plaintext, key)
print("Encrypted Text:", ciphertext)

# Decrypt
decrypted_text = caesar_cipher_decrypt(ciphertext, key)
print("Decrypted Text:", decrypted_text)
