# LB_haproxy
│       └── Dockerfile
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