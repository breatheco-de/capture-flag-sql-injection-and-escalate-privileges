# Lab "The Lovers"

This lab guides the student through a SQL Injection in a Tinder-style app, culminating in gaining root access after discovering secrets in metadata and SSH credentials.

## Key Learnings

- Exploiting forms vulnerable to SQL Injection
- SSH access with exposed credentials
- Discovering information in images via EXIF metadata
- Hash cracking
- Using `sudo` for privilege escalation

## 🖥️ Machine Specifications

- **System:** Debian or Ubuntu Server (no GUI)
- **Web Server:** Apache + PHP
- **Website Path:** `/var/www/html/index.php`
- **Vulnerability:** SQLi in login (username and password = `' OR '1'='1`)
- **Image:** `mike.jpg` (fictitious dating profile)
- **Exposed SSH credentials in the panel:**

## 📁 Expected Structure

### User `mike`

- **SSH Access**
- **Flag 1:** `/home/mike/flag.txt`  
- **Secret Directory:** `/home/mike/secrets/`
- `letter.txt`: fictitious love message
- `amanda.jpg`: contains an **NTLM hash** embedded in EXIF metadata

### User `amanda`

- **Password:** corresponds to the hash the student must crack (`Amandita123`)
- **Included in `sudo` group**
- **Flag 2:** `/root/flag.txt`  

## Defined Users

```bash
hostname: lovers-lab
users:
- student / 4geeks-lab
- mike / m1k3sP4ssword
- amanda / Amandita123 (root via sudo)
```
