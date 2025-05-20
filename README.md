# TextEncryptionIdea
A basic text encryption algorithm that should be reasonably difficult to break

This will be written in Java, but it can be converted to a variety of languages easily once the concept is known.

The idea behind this encryption algorithm is that it inserts a character at the start, randomly, which then determines the next character and so on. The key for each character is determined in advance through a given key, which is stored in a text file.

There are three versions contained within this repository. The first has support for 94 characters (Unicode characters from 32 to 126), and it breaks when operating beyond that boundary. It is sufficient for most message passing, and an example is below.

Encryption Key: 41 72 76 25 92 21 45 87 22 61 6 28 33 80 68 54 71 64 77 8 36 34 12 1 89 52 39 48 16 60 57 66 3 15 50 93 30 44 10 31 59 5 65 53 55 38 29 4 75 9 51 37 74 84 58 90 32 13 17 20 69 27 79 26 82 47 2 14 11 62 0 86 56 67 23 7 49 35 46 19 91 43 78 24 88 63 42 18 85 70 81 83 40 73
Input Text: Hello World
Output Text: eB"S&9b^qa4?)

The second version has support for a much wider section of the characters in Unicode. It is able to handle almost any character, but with the limitation of a few different ones being unable to be shown. It is optimized to only show characters that are readable. Its key is 56907 in length.

The final version has support for all characters, and it has the potential to delete characters. Use at your own risk.
