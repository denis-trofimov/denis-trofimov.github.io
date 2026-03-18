---
title: ""
summary: ""
date: 2026-01-05
type: landing

design:
  spacing: "0"

sections:
  # Разработчик-герой
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Привет, я"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "Я проектирую и создаю"
        strings:
          - хранилища данных
          - "масштабируемые API"
          - "веб-приложения full-stack"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: Моя работа
          url: "#projects"
          icon: arrow-down
        - text: Связаться со мной
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

  # Фильтруемый портфолио
  - block: portfolio
    id: projects
    content:
      title: "Избранные проекты"
      subtitle: "Подборка моей недавней работы"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: Все
          tag: "*"
        - name: Backend
          tag: Backend
        - name: Обучение
          tag: Teaching
        - name: Full-Stack
          tag: Full-Stack
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Визуальный стек технологий
  - block: tech-stack
    id: skills
    content:
      title: "Стек технологий"
      subtitle: "Технологии, которые я использую для создания"
      categories:
        - name: Инженерия и анализ данных
          items:
            - name: Apache Airflow
              icon: devicon/apacheairflow
            - name: Metabase
              icon: custom/Metabase--Streamline-Svg-Logos
            - name: Apache Superset
              icon: custom/Apache-Superset-Icon--Streamline-Svg-Logos
            - name: Power BI
              icon: custom/icons8-power-bi
            - name: DBT
              icon: custom/Dbt--Streamline-Svg-Logos
            - name: DBeaver
              icon: devicon/dbeaver
            - name: SQL
              icon: devicon/azuresqldatabase
            - name: Jupyter Notebook
              icon: devicon/jupyter
            - name: NumPy
              icon: devicon/numpy
            - name: OpenCV
              icon: devicon/opencv
            - name: PyTorch
              icon: devicon/pytorch
            - name: TensorFlow
              icon: devicon/tensorflow

        - name: Backend
          items:
            - name: Go
              icon: devicon/go
            - name: Python
              icon: devicon/python
            - name: PHP
              icon: devicon/php
            - name: C++/C
              icon: devicon/cplusplus
            - name: OpenAPI
              icon: devicon/openapi
            - name: gRPC
              icon: devicon/grpc
            - name: REST API
              icon: devicon/djangorest
            - name: RabbitMQ
              icon: devicon/rabbitmq
            - name: PostgreSQL
              icon: devicon/postgresql
            - name: Redis
              icon: devicon/redis
            - name: MariaDB/MySQL
              icon: devicon/mariadb
            - name: MongoDB
              icon: devicon/mongodb
            - name: OracleDB
              icon: devicon/oracle
            - name: Flask
              icon: devicon/flask
            - name: Django
              icon: devicon/djangorest
            - name: Laravel
              icon: devicon/laravel
            - name: Kubernetes API
              icon: devicon/kubernetes
            - name: Kubernetes Operator SDK (Go)
              icon: devicon/kubernetes
            - name: Node.js
              icon: devicon/nodejs
            - name: Qt
              icon: devicon/qt
            - name: Swagger
              icon: devicon/swagger
            - name: SQLAlchemy
              icon: devicon/sqlalchemy
            - name: uWSGI
              icon: devicon/uwsgi
        - name: DevOps
          items:
            - name: Bash
              icon: devicon/bash
            - name: Docker/Docker Compose/Stack
              icon: devicon/docker
            - name: Nginx
              icon: devicon/nginx
            - name: Traefik
              icon: devicon/traefikproxy
            - name: Kubernetes
              icon: devicon/kubernetes
            - name: Helm
              icon: devicon/helm
            - name: Terraform
              icon: devicon/terraform
            - name: Argo CD
              icon: devicon/argocd
            - name: Grafana
              icon: devicon/grafana
            - name: Prometheus
              icon: devicon/prometheus
            - name: ElasticSearch
              icon: devicon/elasticsearch
            - name: Kibana
              icon: devicon/kibana
            - name: logstash
              icon: devicon/logstash
            - name: Firebase
              icon: devicon/firebase
            - name: GitHub Actions
              icon: devicon/githubactions
            - name: GitLab
              icon: devicon/gitlab
            - name: Jenkins
              icon: devicon/jenkins
            - name: TeamCity
              icon: custom/teamcity_logo_icon_249439
            - name: GCS
              icon: devicon/googlecloud
            - name: AWS
              icon: devicon/amazonwebservices-wordmark
            - name: Azure
              icon: devicon/azure
            - name: Ubuntu
              icon: devicon/ubuntu
            - name: Fedora
              icon: devicon/fedora
            - name: CentOS
              icon: devicon/centos
            - name: Windows Server
              icon: devicon/windows11
            - name: Apache HTTP Server
              icon: devicon/apache

        - name: Frontend
          items:
            - name: JavaScript
              icon: devicon/javascript
            - name: TypeScript
              icon: devicon/typescript
            - name: HTML5
              icon: devicon/html5
            - name: XML
              icon: devicon/xml
            - name: Vue.js
              icon: devicon/vuejs
            - name: Next.js
              icon: devicon/nextjs
            - name: Ruby On Rails
              icon: devicon/ruby
            - name: Hugo
              icon: devicon/hugo
            - name: Wordpress
              icon: devicon/wordpress
            - name: Figma
              icon: devicon/figma

        - name: Другие продукты и инструменты 
          items:
            - name: Bitrix24
              icon: custom/bitrix24-svgrepo-com
            - name: 1С:Бухгалтерия
              icon: custom/Product-1c
            - name: Jira
              icon: devicon/jira
            - name: Confluence
              icon: devicon/confluence
            - name: VSCode IDE
              icon: devicon/vscode
            - name: Cursor IDE
              icon: custom/cursor-ai-code-icon
            - name: LM Studio
              icon: custom/lmstudio
            - name: Perplexity AI
              icon: custom/perplexity-color
            - name: UML
              icon: devicon/unifiedmodelinglanguage

    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Опыт работы
  - block: resume-experience
    id: experience
    content:
      title: Опыт работы
      date_format: Янв 2006
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Последние записи в блоге
  - block: collection
    id: blog
    content:
      title: Последние записи
      subtitle: 'Мысли о веб-разработке, технологиях и многом другом'
      text: ''
      filters:
        folders:
          - blog
        exclude_featured: false
      count: 3
      order: desc
    design:
      view: card
      columns: 3
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Контактная информация
  - block: contact-info
    id: contact
    content:
      title: Свяжитесь со мной
      subtitle: "Давайте создадим что-то удивительное вместе"
      text: |-
        Я всегда заинтересован в обсуждении новых проектов и возможностей.
        Вы ищете нанять, сотрудничать или просто сказать привет, не стесняйтесь обращаться!
      email: alex@example.com
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Карточка CTA
  - block: cta-card
    content:
      title: "Открыт к возможностям"
      text: |-
        В настоящее время я ищу позиции **ведущего инженера** или **технического лидера**.
        
        Давайте свяжемся и обсудим, как я могу помочь вашей команде.
      button:
        text: 'Скачать резюме'
        url: uploads/resume.pdf
        new_tab: true
    design:
      card:
        css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
        text_color: dark
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---