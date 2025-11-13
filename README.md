# Trabajo Practico integrador Computacion Aplicada

### Participantes
- Santiago Araoz Bugallo
- Maximiliano Faita
- Iñaki Stroppiana
- Emanuel Martinez
- Milagros Peralta Ramos

### Descripción
Este repositorio contiene los archivos de configuración, respaldos y documentación correspondientes a la práctica de infraestructura Linux.

### Contenido
- `/root.tar.gz`
- `/etc.tar.gz`
- `/opt.tar.gz`
- `/www_dir.tar.gz`
- `/backup_dir.tar.gz`
- `/var` dividido en partes pequeñas (`var_parte_aa`, `var_parte_ab`, etc.)

- Diagrama topológico (`diagrama_topologia.png` o `.pdf`)

                        TOPOLOGÍA DE INFRAESTRUCTURA

                                ┌────────────────────┐
                                │     Internet       │
                                └─────────┬──────────┘
                                          │
                                   (Conexión Wi-Fi)
                                          │
                                ┌─────────┴──────────┐
                                │    Router Wi-Fi    │
                                └─────────┬──────────┘
                                          │
                   ┌──────────────────────┴───────────────────────┐
                   │                                              │
          ┌────────┴────────┐                          ┌──────────┴─────────┐
          │  Servidor Linux │                          │     Cliente(s)     │
          │    (Debian 11)  │                          │ (PC / Notebook)    │
          │ IP: 192.168.0.153│                         │ Conexión: Wi-Fi    │
          ├──────────────────┤                         │ Acceso: Navegador  │
          │ Servicios activos│                         │ o SSH              │
          │  • Apache (HTTP:80)                        └─────────────────────┘
          │  • MariaDB (3306)
          │  • PHP
          │  • SSH (22)
          ├──────────────────┤
          │ Estructura de directorios principales:
          │  • /www_dir      → Sitio web (index.php, logo.png)
          │  • /opt          → Scripts y componentes adicionales
          │  • /backup_dir   → Copias de seguridad del sistema
          │  • /etc          → Archivos de configuración
          │  • /root         → Directorio del administrador
          │  • /var          → Logs y datos variables
          └──────────────────┘
