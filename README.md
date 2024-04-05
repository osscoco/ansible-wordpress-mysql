Ansible Host WordPress (x2) & Host Sql (x1)
========================

Récupération (GIT)
------------
```bash
$ git clone https://github.com/osscoco/ansible-wordpress-mysql.git
```

## Pré requis

Lancer Docker

```bash
$ cd  ./ansible-tp
```

```bash
$ docker compose up
```

## Ansible Web

- Hub :
```bash
$ http://localhost:1000
```

- Ubuntu-c :
```bash
$ http://localhost:7681/
```

- Authentifiation :
```bash
$ ubuntu-c login:  ansible
$ Password: password
```

- Mettre à jour les dépendences :
```bash
$ sudo apt update
$ '[sudo] password for ansible': password
```

- Installer SSH :
```bash
$ sudo apt install sshpass
$ '[sudo] password for ansible': password
```

- Lancer le playbook :
```bash
$ cd workspace/wordpress-mysql/
$ ansible-playbook playbook.yml
```