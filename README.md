# Hardened Web Server

🔐 **Hardened Web Server: LEMP/LAMP Stack with A+ TLS**

Deploy and secure a production-grade web server on Ubuntu, featuring:

- **Nginx** with directory listing disabled, security headers, and HTTPS  
- **MySQL/MariaDB** with least-privilege user  
- **PHP-FPM** locked down (`disable_functions`, error handling)  
- **UFW** firewall rules (OpenSSH, HTTP, HTTPS)  
- **Let’s Encrypt** TLS certs via Certbot for an **A+** rating on SSL Labs  

---

## 📝 Description

This repo contains all configuration files, scripts, and documentation you need to spin up a hardened web server on any Ubuntu 20.04+ machine (EC2, VM, or bare metal). Just clone, customize your domain in the configs, run the installer, and you’re done.

---

## 🚀 Quickstart

```bash
git clone https://github.com/your-org/hardened-web-server.git
cd hardened-web-server

chmod +x install.sh
sudo ./install.sh

Then visit https://yourdomain.com and verify an A+ on SSL Labs.
📂 Repo Structure

hardened-web-server/
├── install.sh         # installer script
├── nginx/             # Nginx site config and snippets
│   └── default
├── php/               # php.ini hardening
│   └── www.conf
├── mysql/             # SQL scripts
│   └── init.sql
├── ssl/               # Certbot hook scripts (optional)
├── README.md
├── LICENSE
└── CONTRIBUTING.md

🤝 Contributing

See CONTRIBUTING.md for details.

