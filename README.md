# 🐍 Python Utility Scripts

A collection of lightweight, zero-dependency Python utility scripts for everyday tasks.

---

## Scripts

### `batch_rename.py` — Batch File Renamer

Rename multiple files at once with flexible rules.

```bash
# Add a prefix to all JPGs
python batch_rename.py ./photos --prefix "trip_" --ext .jpg

# Replace text in filenames
python batch_rename.py ./docs --replace "draft" "final"

# Rename files as numbered sequence (001, 002, ...)
python batch_rename.py ./files --number --pad 3

# Preview without making changes
python batch_rename.py ./photos --prefix "new_" --dry-run
```

---

### `convert_data.py` — JSON ↔ CSV Converter

Convert data files between JSON and CSV formats with auto type-casting.

```bash
# JSON → CSV
python convert_data.py data.json output.csv

# CSV → JSON
python convert_data.py data.csv output.json --indent 2

# Flatten nested JSON before converting
python convert_data.py nested.json flat.csv --flatten

# Print result to terminal
python convert_data.py data.json --stdout
```

---

### `dir_tree.py` — Directory Tree Visualizer

Print a visual tree of any directory (like the `tree` command), pure Python.

```bash
# Current directory
python dir_tree.py

# Limit depth and exclude folders
python dir_tree.py ./project --depth 3 --exclude dist build

# Save to a file
python dir_tree.py . --output project_structure.txt

# Include hidden files
python dir_tree.py . --include-hidden
```

Example output:
```
my_project/
├── src/
│   ├── main.py
│   └── utils.py
├── tests/
│   └── test_main.py
├── README.md
└── requirements.txt

2 directories, 4 files
```

---

## Requirements

- Python 3.10+
- No third-party dependencies (standard library only)

## License

MIT
https://www.syntechmetal.com
https://www.syntechmetal.com/aluminum-extrusions-products/aluminum-trims/
