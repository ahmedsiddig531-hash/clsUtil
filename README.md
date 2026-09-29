 # C++ Utility Library – `clsUtil`

A reusable C++ utility class containing common helper functions for **random number generation, character generation, key generation, array manipulation, shuffling, swapping, and basic text encryption/decryption**.

This project was developed as part of my C++ programming and problem-solving practice, with a focus on building reusable functions instead of repeatedly writing the same logic.

## 🚀 Features

### 🎲 Random Number Generation

* Generate random numbers within a specified range.
* Initialize the random number generator using the current time.

```cpp
RandomNumber(1, 100);
```

### 🔤 Random Character Generation

Generate random:

* Small letters
* Capital letters
* Digits
* Special characters
* Mixed characters

```cpp
GetRandomCharacter(MixChars);
```

### 📝 Random Word Generation

Generate random words with a specified character type and length.

```cpp
GenerateWord(CapitalLetter, 6);
```

### 🔑 Random Key Generation

Generate formatted keys such as:

```text
ABCD-EFGH-IJKL-MNOP
```

The class can also generate multiple keys automatically.

```cpp
GenerateKeys(10, CapitalLetter);
```

### 🔀 Array Shuffling

Randomly rearrange elements in integer and string arrays.

```cpp
ShuffleArray(arr, arrLength);
```

### 🔄 Swap Functions

The class provides overloaded `Swap()` functions for:

* `int`
* `double`
* `bool`
* `char`
* `string`
* `clsDate`

Example:

```cpp
Swap(A, B);
```

### 📦 Fill Arrays with Random Data

The utility class can populate arrays with:

* Random numbers
* Random words
* Random keys

```cpp
FillArrayWithRandomNumbers(arr, 10, 1, 100);
```

### 🔐 Text Encryption & Decryption

The class provides a simple character-shifting encryption technique.

```cpp
string Encrypted = EncryptText("Hello", 5);
string Decrypted = DecryptText(Encrypted, 5);
```

The encryption works by shifting each character's character code by the specified key.

```text
Original
   ↓
Hello
   ↓ + Encryption Key
Encrypted Text
   ↓ - Encryption Key
Hello
```

> **Note:** This is a learning implementation of basic character-shift encryption and is not intended for securing sensitive information.

### 📑 Tab Formatting

A helper function is included for producing tab spacing in console applications.

```cpp
Tabs(3);
```

---

## 🏗️ Class Structure

The main utility class is:

```cpp
class clsUtil
```

It contains an enumeration for character types:

```cpp
enum enCharType
{
    SamallLetter = 1,
    CapitalLetter = 2,
    Digit = 3,
    MixChars = 4,
    SpecialCharacter = 5
};
```

---

## 🛠️ Technologies

* **C++**
* Object-Oriented Programming
* Static Member Functions
* Function Overloading
* Arrays
* Strings
* Random Number Generation
* Character Encoding
* Basic Encryption Concepts

---

## 📂 Main Functions

| Function                       | Purpose                            |
| ------------------------------ | ---------------------------------- |
| `Srand()`                      | Seeds the random number generator  |
| `RandomNumber()`               | Generates a random number          |
| `GetRandomCharacter()`         | Generates a random character       |
| `GenerateWord()`               | Generates a random word            |
| `GenerateKey()`                | Generates a formatted key          |
| `GenerateKeys()`               | Generates multiple keys            |
| `FillArrayWithRandomNumbers()` | Fills an array with random numbers |
| `FillArrayWithRandomWords()`   | Fills an array with random words   |
| `FillArrayWithRandomKeys()`    | Fills an array with random keys    |
| `Swap()`                       | Exchanges two values               |
| `ShuffleArray()`               | Randomly rearranges array elements |
| `Tabs()`                       | Produces tab formatting            |
| `EncryptText()`                | Encrypts text using a shift key    |
| `DecryptText()`                | Decrypts text using a shift key    |

---

## 🎯 Learning Objectives

This project helped me practice:

* Designing reusable utility functions
* Function overloading
* Working with arrays and strings
* Random number generation
* Random data generation
* Swapping and shuffling algorithms
* Character manipulation
* Basic encryption/decryption concepts
* Writing cleaner and more reusable C++ code

---

## 🔮 Future Improvements

Possible improvements include:

* Replace the current shuffle implementation with the **Fisher-Yates algorithm**
* Improve random number generation using modern C++ random utilities
* Add support for more data types
* Improve encryption using a stronger cryptographic approach
* Add automated tests for utility functions
* Improve error handling and input validation

---

## 👨‍💻 Author

**Ahmed**

This project is part of my ongoing journey in **C++ programming, algorithms, problem solving, and software development**.
