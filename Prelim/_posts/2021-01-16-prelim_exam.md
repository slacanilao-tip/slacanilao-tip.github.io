---
layout: post
title:  "Hands-on Prelim Exam"
date:   2021-01-16 22:40:58 +0800
category: Prelim
image: /assets/prelim/Pexam/Pexam.png
---
Follow procedure:
1. Fork this repository https://github.com/ajcanlas-tip/sysad2-12021.git (Links to an external site.)

2. Clone your new repository in your VM https://github.com/< your username >/sysad2-12021.git

3. Create a branch named "prelim-exam" and checkout in that branch. 

4. Create an Ansible playbook that does the following with an input of a config.yaml file

    Role 1 (python):

      1. Installs the latest python3 and pip3

      2. use pip3 as default pip 

      3. use python3 as default python 

    Role 2 (Java)

      1. Install Java open-jdk

    Role 3 (Change motd)

      1. Create Motd containing the text defined by a variable defined in config.yaml file and if there is no variable input the default motd is "Ansible Managed node by (your user name)"

    Role 4 (Create user)

      1. Create a user with a variable defined in config.yaml

5. push and commit your prelim-exam branch in the VM (no need for ansible.cfg and inventory upon pushing)

6. Request a pull request from that branch in GitHub

7. For your prelim exam to be counted, please paste your repository link as an answer in this exam.

Output:  
[https://github.com/slacanilao-tip/sysad2-12021/tree/prelim-exam](https://github.com/slacanilao-tip/sysad2-12021/tree/prelim-exam)  
```
.  
├── Inventory  
├── README.md  
├── ansible.cfg  
├── config.yml  
├── roles  
│   ├── create_user  
│   │   ├── README.md  
│   │   ├── defaults  
│   │   │   └── main.yml  
│   │   ├── handlers  
│   │   │   └── main.yml  
│   │   ├── meta  
│   │   │   └── main.yml  
│   │   ├── tasks  
│   │   │   └── main.yml  
│   │   ├── tests  
│   │   │   ├── inventory  
│   │   │   └── test.yml  
│   │   └── vars  
│   │       └── main.yml  
│   ├── java  
│   │   ├── README.md  
│   │   ├── defaults  
│   │   │   └── main.yml  
│   │   ├── handlers  
│   │   │   └── main.yml  
│   │   ├── meta  
│   │   │   └── main.yml  
│   │   ├── tasks  
│   │   │   └── main.yml  
│   │   ├── tests  
│   │   │   ├── inventory  
│   │   │   └── test.yml  
│   │   └── vars  
│   │       └── main.yml  
│   ├── motd  
│   │   ├── README.md  
│   │   ├── defaults  
│   │   │   └── main.yml  
│   │   ├── handlers  
│   │   │   └── main.yml  
│   │   ├── meta  
│   │   │   └── main.yml  
│   │   ├── tasks  
│   │   │   └── main.yml  
│   │   ├── tests  
│   │   │   ├── inventory  
│   │   │   └── test.yml  
│   │   └── vars  
│   │       └── main.yml  
│   └── py3_pip  
│       ├── README.md  
│       ├── defaults  
│       │   └── main.yml  
│       ├── handlers  
│       │   └── main.yml  
│       ├── meta  
│       │   └── main.yml  
│       ├── tasks  
│       │   └── main.yml  
│       ├── tests  
│       │   ├── inventory  
│       │   └── test.yml  
│       └── vars  
│           └── main.yml  
└── variables  
    └── vars  
```