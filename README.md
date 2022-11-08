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

-- Install haproxy (use xavki tutoriel) OK

-- Configuration de notre LB: 
    
    -- FrontEnd:reverse proxy
    
    -- BackEnd: ecoute/listner

-- complete all tasks in playbook  In Progress

-- Finalise the load balancing between servers  OK

-- Configuration et accès à l'interface haproxy  OK

-- Creation de la page d'accueil du site devops-jug.com  (HTML & CSS) ToDo

