# Ansible Role: httpd

This Ansible role installs, configures, and manages the **Apache HTTP Server (httpd)** on Linux servers.  
It is designed as a reusable role and demonstrates secure variable management using **Ansible Vault**.

---

## 📌 Use Case

- Automate Apache (`httpd`) installation
- Ensure the service is started and enabled
- Deploy a static `index.html` web page
- Secure sensitive variables using **Ansible Vault**

---

## 📁 Role Structure

httpd/
├── defaults/
│   └── main.yml
├── files/
│   └── index.html          # (used when copy module is required)
├── templates/
│   └── index.html.j2       # (used with template module)
├── handlers/
│   └── main.yml
├── tasks/
│   └── main.yml
├── vars/
│   └── vars.yml            # encrypted using Ansible Vault
├── meta/
│   └── main.yml
└── README.md
