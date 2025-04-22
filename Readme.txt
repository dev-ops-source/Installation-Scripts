---

### 📦 `backup.sh` — Simple 5-Day File Backup Script

This Bash script backup a specified source directory into a ZIP file inside a destination directory, retaining only the **latest 5 backups**. It also checks for the `zip` utility and installs it if missing (Debian/RedHat-based systems only).

---

### 🔧 Features

- Automatically installs `zip` if not present
- Backs up any folder into timestamped `.zip` files
- Keeps the latest **5 backups** and deletes older ones
- Works on most Linux systems
- Cron-friendly (can run automatically every minute)

---

### 📦 Usage

```bash
./backup.sh <source_dir> <backup_dir>
```

- `source_dir`: Folder you want to back up  
- `backup_dir`: Where the backup `.zip` files will be stored

---

### ⏰ Cron Example

To run the backup every minute, add this to your crontab:

```bash
* * * * * /full/path/to/backup.sh /path/to/source /path/to/backup
```

Use `crontab -e` to edit your cron jobs.

---

Let me know if you want a Markdown version or a version with emojis stripped out!