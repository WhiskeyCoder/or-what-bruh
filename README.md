## or_what_bruh.py

### 💬 Description
A simple, chaotic little script that cracks open a text file and splits every line that contains the word "OR" into separate lines at each "OR". It’s dumb. It’s useful. It’s dumbly useful. Originally made during a moment of meme-induced frustration.

### 📂 File
Make sure your file is located at `../project/or_whatbruh.txt` — or adjust the path accordingly.

### 🔧 What It Does
- Reads each line from a `.txt` file
- If it finds the word `OR`, it splits the line at each `OR` into a new line
- Removes leading and trailing whitespace
- Skips empty lines (in theory)
- Prints the chaos to console

### 📜 Sample Input
```
You can have pizza OR pasta OR salad
Make your choice wisely OR suffer the consequences
```

### 📤 Sample Output
```
You can have pizza
pasta
salad
Make your choice wisely
suffer the consequences
```

### 💻 Code
```python
with open('../project/or_whatbruh.txt', encoding="utf-8") as f:
    lines = f.readlines()
    for line in lines:
        if "OR" in line:
            line = line.replace("OR", "\n")
            print(line)
        line = line.strip()
```

### ⚠️ Notes
- Doesn’t write to a new file — it just prints. You want that? Modify it.
- Won’t handle lowercase `or` — this script is petty like that.
- Yes, it’s messy. No, I won’t apologize. It does what it says.

### 📜 License
MIT License — because chaos is best when freely distributed.

