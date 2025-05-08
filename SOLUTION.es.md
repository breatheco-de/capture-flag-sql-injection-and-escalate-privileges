# Laboratorio "The Lovers"

Este laboratorio guía al alumno a través de una SQL Injection en una app estilo Tinder, que culmina en la obtención de acceso root tras descubrir secretos en metadatos y credenciales SSH.

##  Aprendizajes clave

- Explotación de formularios vulnerables a SQL Injection
- Acceso por SSH con credenciales expuestas
- Descubrimiento de información en imágenes vía EXIF
- Cracking de hashes
- Uso de `sudo` para escalar privilegios

## 🖥️ Especificaciones de la máquina

- **Sistema:** Debian o Ubuntu Server (sin GUI)
- **Servidor Web:** Apache + PHP
- **Ruta del sitio web:** `/var/www/html/index.php`
- **Vulnerabilidad:** SQLi en login (usuario y contraseña = `' OR '1'='1`)
- **Imagen:** `mike.jpg` (perfil ficticio de citas)
- **Credenciales SSH expuestas en el panel:**


## 📁 Estructura esperada

### Usuario `mike`

- **Acceso vía SSH**
- **Flag 1:** `/home/mike/flag.txt`  
- **Directorio secreto:** `/home/mike/secrets/`
- `letter.txt`: mensaje ficticio de amor
- `amanda.jpg`: contiene un **hash NTLM** incrustado en los metadatos EXIF

### Usuario `amanda`

- **Contraseña:** corresponde al hash que el alumno debe crackear (`Amandita123`)
- **Incluida en grupo `sudo`**
- **Flag 2:** `/root/flag.txt`  

##  Usuarios definidos

```bash
hostname: lovers-lab
users:
- student / 4geeks-lab
- mike / m1k3sP4ssword
- amanda / Amandita123 (root via sudo)
```