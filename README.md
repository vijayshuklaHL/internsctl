# 🧰 internsctl — Custom Linux Command Tool

**`internsctl`** is a lightweight custom Linux command-line tool written in **Bash**, designed for system information and user management tasks.

> **Author:** Vijay Shukla
> **Files:**
>
> * `internsctl` → Bash script (main executable)
> * `internsctl-man.gz` → Manual (man) file

---

## ⚙️ Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/internsctl.git
   cd internsctl
   ```

2. Make the script executable:

   ```bash
   chmod +x internsctl
   ```

3. (Optional) Move it to your PATH for global access:

   ```bash
   sudo mv internsctl /usr/local/bin/
   ```

4. Install the man file:

   ```bash
   sudo cp internsctl-man.gz /usr/share/man/man1/
   sudo mandb
   ```

Now you can simply run:

```bash
man internsctl
```

---

## 🚀 Usage

```bash
internsctl [OPTIONS]
```

### Options

| Command / Option                    | Description                              |
| ----------------------------------- | ---------------------------------------- |
| `--help`                            | Display help message                     |
| `--version`                         | Display version information              |
| `cpu getinfo`                       | Display CPU information (uses `lscpu`)   |
| `memory getinfo`                    | Display memory information (uses `free`) |
| `user create <username>`            | Create a new user                        |
| `user list`                         | List all system users                    |
| `user list --sudo-only`             | List only users with sudo privileges     |
| `file getinfo [OPTIONS] <filename>` | Get file details                         |

#### File Info Options

| Option            | Short | Description             |
| ----------------- | ----- | ----------------------- |
| `--size`          | `-s`  | Show file size          |
| `--permissions`   | `-p`  | Show file permissions   |
| `--owner`         | `-o`  | Show file owner         |
| `--last-modified` | `-m`  | Show last modified time |

---

## 🧪 Examples

```bash
# Display CPU details
internsctl cpu getinfo

# Display memory information
internsctl memory getinfo

# Create a new user
internsctl user create john_doe

# List all sudo users
internsctl user list --sudo-only

# Get file information (multiple options allowed)
internsctl file getinfo --size --permissions example.txt
```

---

## 📖 Manual Page

To view the manual after installation:

```bash
man internsctl
```

If you haven’t installed it yet, place the man file manually:

```bash
sudo cp internsctl-man.gz /usr/share/man/man1/
sudo mandb
```

Then run:

```bash
man internsctl
```

---

## 🧑‍💻 Author
**Vijay Shukla**

