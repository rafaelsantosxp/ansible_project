# ansible_project

roles/  # Onde ficam os projetos. Dentro de cada função, deve existir um arquivo main.yml
├── database # -- nome do projeto
│   ├── defaults ; Permite adicionar variáveis a uma role. Prioridade mais alta.
│   ├── files ; Para trabalhar com arquivos, adicione ele aqui. É acionado através de uma task.
│   ├── handlers ; Eventos acionados através de uma task.
│   ├── meta ; Trata dependêbcias de uma role para outra. Execute a role database, para depois, a web.
│   ├── tasks ; Lista de tarefas para serem executadas.
│   ├── templates ; Modelo para deploy, que usa variáveis do host. Ex.: hostname
│   └── vars ; Permite adicionar variáveis a uma role.
└── webserver
    ├── defauls
    ├── files
    ├── handlers
    ├── meta
    ├── tasks
    ├── templates
    └── vars
