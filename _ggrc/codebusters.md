---
layout: ggrc
title: Codebusters
type: lab
docname: codebusters
version: 19.0
---

**Introduction**

Code Busters is a fun inquiry event in which students dive into the exciting new field of cryptanalysis -- the art of deciphering, encrypting, and analyzing coded messages without a given key. Through preparing for this event, you will learn how to encode and decode both historical and more modern ciphers. You will also develop tricks and gain the experience to quickly solve cryptography problems. During competition, you will encounter not only monoalphabetic ciphers but also those based in mathematical calculations. Most importantly, I hope this event draws you into this field that has rapidly growing importance in this internet era.

<br>**Preparation**

In this event there are two main types of ciphers you will encounter: monoalphabetic and non-monoalphabetic. Monoalphabetic codes include aristocrats, patristocrats, and xenocrysts, both those with and without hints/spaces/errors. The remaining ciphers -- Atbash, Caesar, Affine, Vigenère, Baconian, Hill, Running-Key, and RSA -- fall under the non-monoalphabetic category.

Monoalphabetic ciphers are simple substitution ciphers in which each letter of the plaintext alphabet is replaced by another letter. Deciphering these ciphers tends to be more about cleverness and the ability to accurately guessing the substitutions. However, determining the substitutions is not a complete guess in the dark. Knowing the following will help you make educated guesses:

1. **Most common letters in the English language --** The frequencies of letters are preserved in a monoalphabetic substitution cipher. Thus, analyzing frequency of certain letters in an encoded message can give you insight into the possible plaintext (decrypted) letter substitutions. Do keep in mind that the order of letter frequencies of the message will almost never be in the same order as that in the English (or Spanish) language. Similarly, knowing the last few least common letters is also useful as these will rarely, if ever, be encrypted into a high frequency encoded letter.
2. **Common words of a given length --** There are a limited number of common words with only one, two, or three letters. In particular, the only one letter words are &quot;a&quot; and &quot;I.&quot;
3. **Common words with an apostrophe --** There are relatively few contractions that are frequently used. The most common endings for them are: &#39;t, &#39;s, &#39;d, &#39;m, &#39;re, &#39;ve, &#39;ll.
4. **Common double letters --** Most letters will rarely be double letters. Knowing the most common ones (ex. EE, OO, LL) will help you narrow down the possibilities when you encounter double letters.
5. **Common word patterns --** Some word patterns appear relatively frequently, but are unique enough that you can almost guarantee what the plaintext word is. For instance, the pattern &quot;abcadb&quot; for a word is most likely the plaintext word &quot;people.&quot;

This may seem like a lot of information to memorize, but don&#39;t worry! You will naturally pick up on it as you continue to practice deciphering monoalphabetic ciphers.

Conversely, non-monoalphabetic ciphers tend to have a set method for encoding and decoding them. They are more straightforward: you apply the cipher encoding and/or decoding method and then just plug and chug as fast as possible. First and foremost, you should know the encrypting (and decrypting) schemes of these ciphers. Then, it is all about getting faster at executing these methods. Here&#39;s a few tips that have worked well for me:

1. **Baconian Cipher --** In some problems you may get two symbols rather than the typical &quot;A&quot; and &quot;B.&quot; You will need to figure out which symbol represents &quot;A&quot; and which &quot;B.&quot; After splitting the letters into groups of 5, as 5 letters represent a plaintext letter, look out for patterns such as &quot;ccccc.&quot; Then, &quot;c&quot; must represent &quot;a&quot; as &quot;aaaaa&quot; represents a plaintext letter but &quot;bbbbb&quot; does not.
2. **Vigenere Cipher --** To find the encrypted letter from plaintext and key letters, you can use the Vigenere Cipher table by find the intersection of the column with the plaintext letter and the row with the key letter. The key will repeat many times throughout the message. First, find the encrypted letter of every plaintext letter that is paired with the first letter of the key. Then, do those that are paired with the second letter, and so on. In this way, you only need to consider one row at a time, saving time by not needing to repeatedly find a different row.
3. **Modulo 26 --** When encrypting and decrypting using the affine or hill cipher, it is necessary to take values in modulo 26 (ie. find the reminder when a value is divided by 26) to determine the letter it represents (0 → A, 1 → B, … 25 → Z). To quickly find the remainder of a value, divide it by 26 in your four-function calculator. Then, subtract the whole number. Multiply the remaining fractional component by 26. The remaining result is your desired remainder. Note that due to some rounding error in the calculator you may end up with a remainder such as 2.9999. Without error this would just be 3.
4. **Be -Lazy- Efficient --** The encrypted messages given for Bacon and Vigenere ciphers are generally fairly long. You can first only decrypt every other letter, or some other variation. With enough letters filled in, you can guess the spaces that are left in between. If you are unable to guess the remaining letters, you can just use the traditional method to fill them in!

Fun fact, once during competition one of my partners completely solved an affine cipher as a monoalphabetic substitution cipher! While this may work, it&#39;s _probably_ not the easiest way to decipher one and I would not recommend it. Instead, find tricks and shortcuts that help make you faster at encrypting/decrypting messages using their given methods.

Still, knowing cipher definitions only gets you so far in this event. While preparing, keep in mind the key idea that solving any cipher, whether monoalphabetic or not, in this event is all about speed while still maintaining accuracy. The best way to increase your encoding/decoding speed is through practice! Practice, practice, and more practice!!

<br>**During the Competition**

During competition, there will be more problems available than there is time to solve them. The first problem will be timed, while the others are not. There will be at most one xenocrypt (cipher in Spanish) at the invitational and regional levels and at least one at the state and nationals levels.

Here&#39;s a few strategies my partners and I used:

1. **Two people work on the timed problem --** I find it unnecessary for all three people to be working on the timed problem. My partners and I start to get in one another&#39;s way and are not all super productive. Instead, it has been more efficient for one person to go ahead and start working on the other problems.
2. **Trade problems --** When you get stuck, hand off the problem to one of your partners. A fresh pair of eyes may find something that you overlooked. This strategy is particularly helpful for monoalphabetic substitution ciphers.
3. **Check what you can --** Check any messages you have decoded. Does it make sense? Encrypted messages may be hard to check, but you can still check some steps. For instance, are the values of a and b in an affine cipher correct? By checking anything you can, you won&#39;t lose points for silly reasons.
4. **Don&#39;t leave too many partially solved problems --** With too many errors and/or blanks, a problem will score you no points. Thus, near the end it&#39;s probably a better idea for everyone to work on the same one or couple problems to complete them rather than leaving 3 half-solved problems.

<br>**Some Helpful Resources**

Check out [http://crypto.interactive-maths.com/](http://crypto.interactive-maths.com/) to find the encrypting and decrypting methods for the ciphers. This site also gives you some historical context for and examples of each cipher.

A great place to practice monoalphabetic ciphers is: [https://www.cryptograms.org/](https://www.cryptograms.org/) There is also a tutorial with some basic methods used to solve cryptograms.

For even more practice, you can create your own encoded messages! Ask your partners and/or friends to come up with a phrase and use online resources to give you an encoded message.

Alternatively, you could also use them to check if you encoded a plaintext message correctly. Here are a few nice decoders:

- Hill Cipher -- [http://www.dcode.fr/hill-cipher](http://www.dcode.fr/hill-cipher)
- Affine Cipher -- [http://www.dcode.fr/affine-cipher](http://www.dcode.fr/affine-cipher)
- Vigenere Cipher -- [http://www.dcode.fr/vigenere-cipher](http://www.dcode.fr/vigenere-cipher)

<br>**About the Author**

Emily Wen is an undergraduate at Stanford University. She is a national runner-up and state champion in Code Busters.