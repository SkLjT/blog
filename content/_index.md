---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:

  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Навыки
      items:
        - name: Программированние
          description: 80%
          icon: computer
          icon_pack: fas
        - name: Геймерство
          description: 80%
          icon: gamepad
          icon_pack: fas
        - name: Спорт
          description: 99%
          icon: volleyball
          icon_pack: fas
  - block: experience
    content:
      title: Опыт
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Cоздание приложения
          company: Создавал приложение для себя
          company_url: ''
          company_logo: java
          location: Москва
          date_start: '2019-01-01'
          date_end: '2019-09-01'
          description: |2-
              Этапы создания:

              * Обучение языку javascript
              * Создание приложения для смартфонов на Android 
              * Проверка на разных устройствах
        - title: Репетиторство
          company: Частный репетитор
          company_url: ''
          company_logo: person-chalkboard-solid
          location: Москва
          date_start: '2022-01-01'
          date_end: ''
          description: Подготовка учеников для сдачи ЕГЭ,ОГЭ и ВПР
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Достижения'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://bronschool2.edumsko.ru/
          date_end: ''
          date_start: '2022-05-29'
          description: 'Окончил школу с красным аттестатом и золотой медалью'
          organization: Школа
          organization_url:
          title: Окончание школы
          url: 'https://bronschool2.edumsko.ru/'
        - certificate_url: http://russwimming.ru/?ysclid=lg70j6yomz5502642
          date_end: ''
          date_start: '2018-07-01'
          description: Получил разряд "Кондидат в мастера спорта" по плаванию
          organization: ВФП
          organization_url: http://russwimming.ru/?ysclid=lg70j6yomz5502642
          title: Плавание
          url: http://russwimming.ru/?ysclid=lg70j6yomz5502642
        - certificate_url: https://rowingrussia.ru/
          date_end: '2020-10-07'
          date_start: '2018-09-01'
          description: Получил разряд "Кондидат в мастера спорта" по гребле каноэ
          organization: ФГСР
          organization_url: https://rowingrussia.ru/
          title: Гребля на каноэ
          url: https://rowingrussia.ru/
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Публикации
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Проекты
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: Всё
          tag: '*'
        - name: Программирование
          tag: Программирование
        - name: Работа
          tag: Работа
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Галерея
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Избранные публикации 
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: car
  - block: collection
    content:
      title: Последние публикации
      text: |-
        
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Прошедшие и предстоящие выступления
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Популярные темы
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Контакты
      subtitle:
      text: |-
        Связь со мной
      # Contact (add or remove contact options as necessary)
      email: lusin5745@gmail.com
      phone: +7 (929) 545-34-64
      
      address:
        street: Миклухо-Маклая
        city: Москва
        region: CA
        postcode: '117198'
        country: Российская Федерация
        country_code: Рус
      directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      office_hours:
        - 'Каждый день с 8:00 до 23:00'
      contact_links:
        - icon: telegram
          icon_pack: fab
          name: Пишите
          link: '@temo4ek'
        - icon: vk
          icon_pack: fab
          name: Можно и сюда писать
          link: 'https://vk.com/lusin05'
        - icon: discord
          icon_pack: fab
          name: Звонок
          link: 'sokol#6663'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---

