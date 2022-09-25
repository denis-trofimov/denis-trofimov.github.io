---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: Experience
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Lead Platform Engineer
    company: Huma Therapeutics Ltd.
    company_url: https://huma.com/
    location: London, UK
    date_start: "2021-01-11"
    date_end: 
    description: |-
      * Automated Pull Request Operation for Huma API backend team, making it possible to preview backend API in temporary cloud environments.
      * Created Kubernetes operators to reconcile application and application compositions, inspired by docker-compose, to abstract away Kubernetes API complexity for developers.
      * Created Kubernetes operators to reconcile cloud resources such as AWS S3 and GCS storages, Atlas and KubeDB provided MongoDBs, Redis cache, to enable managing these resources from controlling Kubernetes cluster.
      * Led internal platform team of 3 senior engineers
      * Automated CI/CD process, allowing the team to develop and test faster

      Technology

      * Golang, Kubernetes, Operator SDK Go, MongoDB, Docker, GitHub CI
      * Jira, Confluence, GitHub, VSCode
      * GCP GKE, AWS EKS, Azure AKS, Terraform, Helm, ArgoCD, Helmfile

  - title: "CTO"
    company: "Sittme. A revolutionary application that helps parents and nannies find each other"
    company_url: "https://sitt.me"
    location: Moscow, Russia
    date_start: "2019-11-20"
    date_end: "2020-06-30"
    description: |-
      Sitt.me – a babysitting crowd-sourced platform. My team consisted of PM, designer, QA, and developers: back-end, front-end, and mobile devs.

      * Designed and implemented features like in-app notifications, video calls, etc.
      * Handled deployment of 24 services to a private Kubernetes cluster production, staging environments
      * Automated CI/CD process, allowing the team to test and deploy faster
      * Detected and solved issues in our services
      * Mentored back-end, and front-end devs

      Technology
      
      * Golang, Bash, Ruby, ReactJS, SQL; PostgreSQL DB, Redis, Maria, RabbitMQ, Firebase; Jira, Confluence, GitLab
      * Engineering: Kubernetes, Docker, GitLab CI, ELK, Helm 

  - title: "Senior Software Developer"
    company: "Tinkoff"
    company_url: "https://tinkoff.ru"
    location: Moscow, Russia
    date_start: "2018-11-19"
    date_end: "2019-05-31"
    description: |-
      * Refactored Text-To-Speech API service, using in-house Python async gRPC server library
      * Designed and implemented CMS of a voice assistant using Flask, PostgreSQL
      * Redesigned and implemented low-latency Text-To-Speech API service on Golang, Redis, PostgreSQL
      * Deployed and tested services to a private Kubernetes cluster, automated CI/CD process using TeamCity 
      * Responsibilities included: code review, interviews, and mentoring developers from my team
      * The team consisted of a technical lead, PM, 2 backend developers, 4 AI data scientists, and a mathematical linguist

      Technology:

      * Languages: Python, Golang, C++, SQL, bash
      * Packages: gRPC, TensorFlow Serving, Flask, Gunicorn, NumPy, SQLAlchemy.
      * DB: PostgreSQL DB, Redis, MongoDB
      * tools: Docker, Kubernetes, Helm, Jira, Confluence, Bitbucket, TeamCity, PyCharm, Goland

  - title: "Lead Software Developer"
    company: "Vzor Systems, LLC"
    company_url: "https://vzorsystems.ru"
    location: Moscow, Russia
    date_start: "2017-05-03"
    date_end: "2018-09-10"
    description: |-
      Achivements:

      * Designed architecture and developed a bio-metric identification software (GUI client, server, and embedded).
      * Hired and spearheaded two software developers on this project.
      * Optimized identity recognition using classic image processing algorithms and CNN
      * Conducted a technological proof test and prepared a NIST compliant report.

      Technology:

      * Python, C++, C, SQL; Git (GitLab); Eclipse IDE, Qt Creator
      * OpenCV, Caffe, SciPy; SQLAlchemy; gRPC, MQTT; PostgreSQL; Ubuntu, MS Windows

  - title: "Backend Software Developer"
    company: "Bigur-consulting, LLC"
    company_url: "https://bigur.ru"
    location: Moscow, Russia
    date_start: "2016-11-01"
    date_end: "2017-05-01"
    description: |-
      Achivements:
      
      * Web-commerce site backend development for a wine importer, made on in-house Python framework from scratch.

      Technology:

      * Python 3.2, ExtJS 4; Git; vim, UMLet; PostgreSQL DB, SQLite, Apache HTTP Server, WSGI

  - title: "Software Developer C++"
    company: "Asoft, LLC"
    company_url: "http://www.asoft.ru"
    location: Moscow, Russia
    date_start: "2012-01-15"
    date_end: "2016-11-27"
    description: |-
      Achivements:
      
      * Developed and deployed a railroad technological process modeling client-server application.

      Technology:

      * С++, SQL, HTML, XML, JavaScript; VSC CVS; Eclipse IDE, KDEvelop, emacs
      * Oracle DB, MySQL, in-house RDBMS + Web Server; bash, Fedora Linux

  - title: "Engineer"
    company: "Khrunichev State Research and Production Space Center"
    company_url: "http://www.khrunichev.ru/"
    location: Moscow, Russia
    date_start: "2010-11-01"
    date_end: "2012-01-10"
    description: |-
      * Developed Borland C++ Builder applications for satellite trajectory computations

  # - title: CEO
  #   company: GenCoin
  #   company_url: ''
  #   company_logo: org-gc
  #   location: California
  #   date_start: '2021-01-01'
  #   date_end: ''
  #   description: |2-
  #       Responsibilities include:
        
  #       * Analysing
  #       * Modelling
  #       * Deploying

  # - title: Professor of Semiconductor Physics
  #   company: University X
  #   company_url: ''
  #   company_logo: org-x
  #   location: California
  #   date_start: '2016-01-01'
  #   date_end: '2020-12-31'
  #   description: Taught electronic engineering and researched semiconductor physics.

design:
  columns: '2'
---
