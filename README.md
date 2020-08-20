# README

This code repository aims to provide a basic for a do-nothing-script with Ansible. After reading [this](https://blog.danslimmon.com/2019/07/15/do-nothing-scripting-the-key-to-gradual-automation/) great article I started to play around with this concept. As many rely on Ansible for the automation of tasks, I thought: let's give it a try (with the help of [this](https://medium.com/@ayeshasilvia/testing-ansible-playbook-in-a-docker-container-21628e9ee256) perfect guideline).

And here it is.

## Structure

```
.
├── README.md
├── ansible
│   ├── env
│   │   └── local_docker
│   ├── my_fun_playbook.yml
│   ├── myplaybook.yml
│   └── roles
│       ├── role1
│       │   └── tasks
│       │       └── main.yml
│       └── role2
│           └── tasks
│               └── main.yml
├── container-start-and-playbook-run.sh
└── docker
    └── Dockerfile
```

## How to edit and extend

- update the main.yml for role1 or role2 (this is just a bit more funny example!)
- or add new roles and tasks
- update (if neccessary) the myplaybook.yml

## How to run

Simply start the script:

```
./container-start-and-playbook-run.sh
```