# 📘 Regular Expressions (Regex)

Regular expressions, commonly known as **regex**, are sequences of characters that form search patterns.  
They are widely used for **string searching, pattern matching, validation, and text manipulation**.  

Regex is supported across many programming languages such as **Python, Java, JavaScript, C#, and PHP**.

---

## 🔹 Why Use Regex?
- ✅ Search for patterns in text  
- ✅ Validate inputs (emails, phone numbers, passwords, etc.)  
- ✅ Extract useful information (like numbers, URLs, hashtags)  
- ✅ Replace or format text  
- ✅ Automate repetitive text-processing tasks  

---

## 🔹 Basic Syntax
| Symbol | Meaning |
|--------|----------|
| `.`    | Any character except newline |
| `^`    | Start of string |
| `$`    | End of string |
| `*`    | Zero or more repetitions |
| `+`    | One or more repetitions |
| `?`    | Zero or one repetition |
| `{n}`  | Exactly `n` repetitions |
| `{n,}` | At least `n` repetitions |
| `{n,m}`| Between `n` and `m` repetitions |
| `[]`   | Matches any character inside brackets |
| `[^]`  | Matches any character *not* inside brackets |
| `\d`   | Digit (0–9) |
| `\D`   | Non-digit |
| `\w`   | Word character (letters, digits, underscore) |
| `\W`   | Non-word character |
| `\s`   | Whitespace (space, tab, newline) |
| `\S`   | Non-whitespace |

---

## 🔹 Common Examples

### 1. Match a word
```regex
\w+
Matches: "Python", "Regex", "hello123"

2. Validate an email
regex
Copy
Edit
^[\w\.-]+@[\w\.-]+\.\w{2,3}$
Matches: user@example.com, my.email@domain.org

3. Extract all numbers
python
Copy
Edit
import re
text = "My phone number is 03001234567"
numbers = re.findall(r"\d+", text)
print(numbers)  # ['03001234567']
4. Find all URLs
python
Copy
Edit
import re
text = "Visit https://www.python.org or http://example.com"
urls = re.findall(r"https?://\S+", text)
print(urls)  # ['https://www.python.org', 'http://example.com']
5. Replace multiple spaces with one
python
Copy
Edit
import re
text = "Python    is   fun"
cleaned = re.sub(r"\s+", " ", text)
print(cleaned)  # Python is fun
🔹 Use Cases
Validation → emails, phone numbers, passwords

Data Extraction → hashtags, mentions, URLs, dates, numbers

Search & Replace → cleaning messy text, formatting data

Log Parsing → extract IP addresses, error messages

Web Scraping → filter required information

🔹 Tips for Beginners
Always test regex on small strings before using in real projects.

Use online testers like regex101.com for quick debugging.

Keep regex readable—complex expressions can be confusing.

Prefer raw strings in Python (r"pattern") to avoid escape issues.

🚀 Conclusion
Regex is a powerful tool for handling text.
Whether you’re validating input, extracting data, or cleaning up text, regex makes the job much faster and more efficient.

📝 Practice is the key—start with small patterns and build your way up!

pgsql
Copy
Edit




















