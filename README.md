# LB_haproxy
```
├── LB_haproxy
│   ├── ansible.cfg
│   ├── group_vars
│   ├── haproxy.yaml
│   ├── inventaire.ini
│   ├── README.md
│   └── roles
│       ├── apache
│       │   ├── files
│       │   ├── handlers
│       │   │   └── main.yml
│       │   ├── README.md
│       │   ├── tasks
│       │   │   ├── configure_apache.yaml
│       │   │   ├── install_apache.yaml
│       │   │   └── main.yml
│       │   └── templates
|       ├── haproxy
│       |   ├── files
│       |   │   └── haproxy.cfg
│       |   ├── handlers
│       |   └── tasks
│       |       ├── copy_cfg.yaml
│       |       ├── install_haproxy.yaml
│       |       └── main.yaml
│       ├── mysql
│       │   ├── files
│       │   ├── handlers
│       │   │   └── main.yml
│       │   ├── README.md
│       │   ├── tasks
│       │   │   ├── connexion_mysql.yaml
│       │   │   ├── create_user.yaml
│       │   │   ├── install_mysql.yaml
│       │   │   └── main.yml
│       │   └── templates
│       ├── php
│       │   ├── files
│       │   ├── handlers
│       │   │   └── main.yml
│       │   ├── README.md
│       │   ├── tasks
│       │   │   ├── install_php.yaml
│       │   │   └── main.yml
│       │   └── templates
│       └── requirements
│           └── tasks
│               └── install_requirements.yaml
```

To do 

-- Install haproxy (use xavki tutoriel) ok

-- Configuration de notre LB
    -- FrontEnd:reverse proxy
    -- BackEnd: ecoute/listner

Depuis le serveur 116 j'ai mis en place la config suivante sur haproxy: 
```
frontend myapp_front
	bind *:8080
	default_backend myapp_back

backend myapp_back
	server apache 172.24.64.115:8000
	server python 172.24.64.190:5000
```
C'est seuelement en lançant des serveurs virtuels (python3 -m -m http.server $port) sur la machine 115 et 190 qie j'ai pu loadbalancer, autrement j'ai un 503 si je le fait sur le port 80 de 115.
-- complete all tasks in playbook

-- Finalise the load balancing between servers

-- Creation de la page d'accueil du site devops-jug.com  (HTML & CSS)

