---
title: "Сервис записи трафика VoIP на Python"
summary: "Фриланс-заказ для De Novo Lab"
authors:
  - me
tags:
  - Python
  - Backend
  - VOIP
  - Запись трафика
  - tcpdump
  - Google Cloud Storage
  - PostgreSQL
  - SQLAlchemy
  - Flask
  - Linux
  - Git
tech_stack:
  - Python
  - tcpdump
  - Google Cloud Storage
  - PostgreSQL
  - SQLAlchemy
  - Flask
  - Linux
  - Git

date: 2017-05-01T16:54:03+03:00
---

Я разработал сервис записи трафика VoIP на Python Backend для De Novo Lab (фриланс-заказ).

* Рефакторил многопоточный сервис записи трафика VoIP с Python 2.7 на 3.4
* Добавил Google Cloud Storage, функции конфигурации, исправил ошибки JSON API, FTP, SFTP хранилищ
* В команде De Novo Lab были PM, системный администратор, 2 тестировщика

Технологии

* Python 2.7, 3.4, SQL; Git Bitbucket, Atlassian Jira; Eric Python IDE, vim;
* Flask, gcs-client, psycopg2 для PostgreSQL DB, SQLite, SQLAlchemy, tcpdump, tshark, mawk;
* Развернуто на Debian, CentOS Linux
