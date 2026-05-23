# 🔐 Substitution Cipher in Python

A simple encryption and decryption tool built in Python using a randomized substitution cipher.

---

## How It Works

A master list of every usable character is created (letters, digits, punctuation, and spaces), then shuffled to produce a unique key. Each character in your message is looked up in the original list, and its position is used to grab the replacement from the shuffled key. Decryption does the exact opposite — look up the character in the key, use the index to pull the original from the character list.

---

## What I Learned

- How to use the `string` module (`string.ascii_letters`, `string.digits`, `string.punctuation`) to build a complete character set
- How `random.shuffle()` generates a randomized key for encryption
- How list indexing maps one character to another — `chars.index(letter)` finds the position, then `key[index]` fetches the substitute
- That the same logic works in reverse for decryption — swap `chars` and `key` to go backwards
- How encryption and decryption are two sides of the same mapping

---

## Usage

Run the script and follow the prompts:

```bash
python cipher.py
```

**Encrypt:**
```
Enter a message to encrypt: hello world
original message: hello world
encrypted message: Xk22T%yT=28
```

**Decrypt:**
```
Enter a message to decrypt: Xk22T%yT=28
encrypted message: Xk22T%yT=28
original message: hello world
```

> ⚠️ The key is randomly generated each run. Encrypt and decrypt in the **same session** or the key won't match.

---

## Limitations
* The key is not saved between sessions
* Only supports characters in the predefined character set
* Single substitution ciphers are not cryptographically secure — this is a learning project!

---

## About

I'm a beginner learning Python and built this as a hands-on way to understand
how encryption works. Each project I build teaches me something new about the language.
- The key is not saved between sessions
- Only supports characters in the predefined character set
- Single substitution ciphers are not cryptographically secure — this is a learning project!
