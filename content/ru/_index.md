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
---
