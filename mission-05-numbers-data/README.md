# Mission 5 - Number Systems, Python, and Text Encoding

## 1. Task / objective
Convert values manually across decimal, binary, and hexadecimal systems, verify results using Python's interactive shell, build a working Python number-converter script, and explain how computers store text using character encoding standards.

## 2. Work completed
* Completed step-by-step manual conversions across decimal (base 10), binary (base 2), and hexadecimal (base 16).
* Verified every manual conversion in the Python 3 interactive shell (`python3`).
* Built and tested `number_converter.py` with three positive integer inputs (`10`, `42`, and `255`).
* Documented ASCII codes and explained why computers need encoding standards like ASCII and UTF-8.

## 3. Commands / tools used
* `python3` — Launches the Python 3 interactive shell for verifying conversions and executes `number_converter.py`.
* `input()` and `int()` — Reads user input from Terminal as text and converts it into an integer.
* `bin()` — Built-in Python function that converts an integer into a base-2 binary string prefixed with `0b`.
* `hex()` — Built-in Python function that converts an integer into a base-16 hexadecimal string prefixed with `0x`.
* **Git (`git add`, `git commit`, `git push`)** — Stages, commits, and pushes Mission 5 files to GitHub.

## 4. My understanding

### Task 5.1 - Convert Numbers by Hand

| Question | Your Working and Answer |
| :--- | :--- |
| **Convert decimal `13` to binary.** | $13 \div 2 = 6\text{ R }1 \rightarrow 6 \div 2 = 3\text{ R }0 \rightarrow 3 \div 2 = 1\text{ R }1 \rightarrow 1 \div 2 = 0\text{ R }1$. Reading remainders from bottom to top: **`1101`** |
| **Convert decimal `25` to binary.** | $25 \div 2 = 12\text{ R }1 \rightarrow 12 \div 2 = 6\text{ R }0 \rightarrow 6 \div 2 = 3\text{ R }0 \rightarrow 3 \div 2 = 1\text{ R }1 \rightarrow 1 \div 2 = 0\text{ R }1$. Reading remainders from bottom to top: **`11001`** |
| **Convert binary `1010` to decimal.** | $(1 \times 2^3) + (0 \times 2^2) + (1 \times 2^1) + (0 \times 2^0) = 8 + 0 + 2 + 0 =$ **`10`** |
| **Convert binary `1101` to decimal.** | $(1 \times 2^3) + (1 \times 2^2) + (0 \times 2^1) + (1 \times 2^0) = 8 + 4 + 0 + 1 =$ **`13`** |
| **Convert hexadecimal `A` to decimal.** | In base 16, $A$ represents **`10`**. |
| **Convert hexadecimal `1F` to decimal.** | $(1 \times 16^1) + (15 \times 16^0) = 16 + 15 =$ **`31`** |
| **Convert binary `1111` to hexadecimal.** | $(1 \times 2^3) + (1 \times 2^2) + (1 \times 2^1) + (1 \times 2^0) = 8 + 4 + 2 + 1 = 15$, which equals **`F`** in hexadecimal. |

---

### Task 5.2 - Verify Using Python

| Expression Tested | Python Result | Matches Manual Calculation? |
| :--- | :--- | :--- |
| `bin(13)` | `'0b1101'` | Yes (`1101`) |
| `bin(25)` | `'0b11001'` | Yes (`11001`) |
| `int('1010', 2)` | `10` | Yes (`10`) |
| `int('1101', 2)` | `13` | Yes (`13`) |
| `int('A', 16)` | `10` | Yes (`10`) |
| `int('1F', 16)` | `31` | Yes (`31`) |
| `hex(0b1111)` | `'0xf'` | Yes (`F`) |

---

### Task 5.3 - Build a Small Number Converter

**How the conversion functions work:**
* `bin(number)` takes a decimal integer and returns its base-2 binary representation as a string starting with the `0b` prefix.
* `hex(number)` takes a decimal integer and returns its base-16 hexadecimal representation as a string starting with the `0x` prefix.

| Test Number | Binary Output | Hexadecimal Output |
| :--- | :--- | :--- |
| `10` | `0b1010` (`1010`) | `0xa` (`A`) |
| `42` | `0b101010` (`101010`) | `0x2a` (`2A`) |
| `255` | `0b11111111` (`11111111`) | `0xff` (`FF`) |

---

### Task 5.4 - How Is Text Stored?
* **ASCII decimal codes:** Uppercase `A` = **`65`**, Lowercase `a` = **`97`**.
* **Why a computer needs an encoding standard:** Computer hardware can only store and process binary digits (`0`s and `1`s), so a character-encoding standard provides a universal rulebook mapping every letter, number, and symbol to a specific numeric code that any computer can decode consistently.
* **Example of a character not in basic ASCII:** Emojis (such as `🚀`) or Hindi Devanagari characters (such as `अ`), which require multi-byte standards like UTF-8.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
* `mission-05-numbers-data/number_converter.py`
* `mission-05-numbers-data/README.md`

## 8. Commit details
Committed with message: `"Build number converter and practise data representation"` and pushed to GitHub.