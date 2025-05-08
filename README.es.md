# THE LOVERS 

En este laboratorio vas a explotar una vulnerabilidad clásica de SQL Injection para acceder al panel de administración de una app de citas. A partir de allí, obtendrás credenciales sensibles y avanzarás hasta descubrir relaciones ocultas, directorios secretos y usuarios privilegiados. En este laboratorio aprenderás:

- Identificación y explotación de SQL Injection en formularios de login
- Acceso remoto a servidores Linux mediante SSH
- Búsqueda de información sensible en perfiles de usuario
- Cracking de hashes con herramientas como `hashcat`
- Escalada de privilegios basada en usuarios con permisos de root

<how-to-start>
   
## 🌱 Cómo iniciar este laboratorio

Sigue las siguientes instrucciones para comenzar:

1. **Descarga la máquina virtual** desde este [enlace](https://storage.googleapis.com/cybersecurity-machines/lovers-lab.ova).
2. **Importa la máquina** en tu gestor de virtualización preferido (VirtualBox, VMware, etc.).
3. Una vez iniciada la máquina, ¡ya puedes comenzar con el laboratorio!
</how-to-start>


## 📄 Instrucciones

Estás frente a una aplicación web romántica y vulnerable. Tu misión es usar tus habilidades técnicas para descubrir los secretos detrás de este panel.

1. **Descubre la dirección IP de la máquina THE LOVERS.**
   - Usa herramientas como `nmap`, `netdiscover` o `arp-scan` para escanear la red.

2. **Accede al sitio web alojado en el servidor.**: Encontrarás una landing con login típico de apps de citas. Usa SQL Injection para acceder sin credenciales reales.

3. **Accede al panel de administración del usuario Mike.**

4. **Conéctate por SSH al servidor como Mike.**

5. **Encuentra la primera flag.**

6. **Explora el directorio `secrets`.**

7. **Descubre la contraseña de Amanda y cambia de usuario.**

8. **Accede a la flag final como root.**

**Recuerda:** incluso los amores secretos dejan huellas digitales. 💔

¡Buena suerte!