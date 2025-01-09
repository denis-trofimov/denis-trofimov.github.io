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
  - title: Lead Software Developer (Platform Team Lead SWE)
    company: Huma Therapeutics Ltd.
    company_url: https://huma.com/
    location: London, UK
    date_start: 2021-01-11
    date_end: 2024-06-17
    description: |-
      **Achievements**

      * I designed and developed a custom IDP solution for the company, which includes all Huma products such as patient monitoring, pre-trained AI models, and any docker container applications. This IDP allows for 0-day operations as well as some day-2 operations, such as data backup and restore.
      * Automated pull request feature for the back-end development team, allowing them to preview back-end APIs in temporary cloud environments. This effectively reduces the time it takes to deploy from eight hours to fifteen minutes!
      * To automate DevOps tasks related to managing cloud resources, I have created Kubernetes operators that provide instant access to AWS S3, Google Cloud Storage, and Atlas MongoDB PostgreSQL and Redis cache.
      * Furthermore, I automated the CI/CD (Continuous Integration and Continuous Deployment) process using Argo CD and Grafana Cloud, among other tools. This increases both speed and reliability.
      * For two years, I led an internal platform team consisting of two senior engineers.

      **Technology**

      * Golang, Kubernetes API, Typiscript, Vue.js, Operator SDK Go, MongoDB, Docker, GitHub CI, PostgreSQL, Redis
      * Jira, Confluence, GitHub, VSCode, Hugo
      * GCP GKE, AWS EKS, Azure AKS, Terraform, Helm, ArgoCD, Helmfile, Grafana Cloud, Atlas Cloud, KubeDB

  - title: Chief Technical Officer
    company: Sittme
    company_url: https://sitt.me
    location: Moscow, Russia
    date_start: "2019-11-20"
    date_end: "2020-06-30"
    description: |-
      Sitt.me is a community-based babysitting service that has a mobile platform. We had a team of professionals, including a project manager, a designer, a quality assurance expert, and developers: backend, frontend, and mobile.

      **Achievements**

      * I've designed and implemented some cool features like in-app notifications and video calls.
      * I helped deploy 24 services in a private Kubernetes cluster for production and staging environments.
      * I've automated the CI/CD process to allow the team to test and deploy faster.
      * During my time here, I detected and solved some issues with our services.
      * Additionally, I mentored both back-end and front-end developers.

      **Technology**
      
      * Golang, Bash, Ruby, ReactJS, SQL; PostgreSQL DB, Redis, Maria, RabbitMQ, Firebase; Jira, Confluence, GitLab
      * Engineering: Kubernetes, Docker, GitLab CI, ELK, Helm 

  - title: "Senior Software Developer"
    company: "Tinkoff"
    company_url: "https://tinkoff.ru"
    location: Moscow, Russia
    date_start: "2018-11-19"
    date_end: "2019-05-31"
    description: |-
      **Achievements**

      * I built and implemented a voice assistant CMS with Flask and PostgreSQL.
      * Redesigned the low-latency API with Golang, Redis, PostgreSQL.
      * I've refactored the text-to-speech API service using async gRPC Python library.
      * Deployed services to Kubernetes cluster, automated CI/CD with TeamCity. 
      * Responsibilities include code reviews, interviewing, mentoring.

      **Technology**

      * Languages: Python, Golang, C++, SQL, bash
      * Packages: gRPC, TensorFlow Serving, Flask, Gunicorn, NumPy, SQLAlchemy.
      * DB: PostgreSQL DB, Redis, MongoDB
      * Tools: Docker, Kubernetes, Helm, Jira, Confluence, Bitbucket, TeamCity, PyCharm, Goland

  - title: "Lead Software Developer"
    company: "Vzor Systems, LLC"
    company_url: "https://vzorsystems.ru"
    location: Moscow, Russia
    date_start: "2017-05-03"
    date_end: "2018-09-10"
    description: |-
      **Achievements**

      * I have designed the architecture and developed a biometric identification software solution, including a GUI client, server and embedded components.
      * I have led a team of two software developers in this project, hiring them and guiding them through the process.
      * To optimize identity recognition, I have used classic image processing algorithms and CNN.
      * I performed a technological proof test and prepared a report that complied with the NIST standards.
      * At three Russian conferences, "All-over-IP," "SKUD," and "TB Security Technology," I presented prototypes of the bio-metric identification solutions.

      **Technology**
      
      * Python, C++, Qt, C, SQL; Git (GitLab); Eclipse IDE, Qt Creator
      * OpenCV, Caffe, SciPy; SQLAlchemy; gRPC, MQTT; PostgreSQL; Ubuntu, MS Windows Server

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
    date_start: "2011-03-15"
    date_end: "2016-05-27"
    description: |-
      **Achievements**

      * I developed a client-server app that simulated the tech operation of train stations and handed it over to the client. Thanks to the solutions I implemented, the client successfully fulfilled the contract for upgrading the tracks at Syzran station 1.
      * I designed and delivered a custom client-server system to the client, which helped them predict energy usage in a train section, among other things.
      * During my time here, I gained experience on ongoing projects and picked up two projects that the lead programmer had left behind.
      * I successfully delivered software and managed MySQL and Oracle databases.
      * As part of a team, including a project manager, and 2 interns, we worked together to complete project goals.
        
      **Technology**

      * С++, SQL, HTML, XML, JavaScript; VSC CVS; Eclipse IDE, KDevelop, emacs
      * Oracle DB, MySQL, in-house RDBMS + Web Server; bash, Fedora Linux

  - title: "Engineer"
    company: "Khrunichev State Research and Production Space Center"
    company_url: "http://www.khrunichev.ru/"
    location: Moscow, Russia
    date_start: "2010-11-01"
    date_end: "2012-01-10"
    description: |-
      * Developed 2 Windows desktop applications for satellite trajectory computations.
      * С++, Borland C++ Builder

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
