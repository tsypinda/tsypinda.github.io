---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Скачать резюме
        url: uploads/resume.pdf
      headings:
        about: 'О себе'
        education: 'Образование'
        interests: 'Интересы'
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 О моих исследованиях'
      subtitle: ''
      text: |-
        Интересуюсь **компьютерной алгеброй** и её применением в образовании и научных расчётах. Активно изучаю систему **SageMath** для решения задач линейной алгебры, теории чисел и символьных вычислений.

        Программирую на **C++** и **Python** — нравится как низкоуровневая работа с памятью, так и написание скриптов для анализа данных. В C++ меня привлекает эффективность и контроль над ресурсами, в Python — скорость разработки и богатая экосистема библиотек.

        В свободное время изучаю иностранные языки и играю на гитаре. Считаю, что музыка помогает развивать абстрактное мышление и чувство ритма в коде 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Избранные работы
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Недавние публикации
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Выступления и доклады
      filters:
        folders:
          - events
    design:
      view: card
  - block: collection
    id: news
    content:
      title: Новости и обновления
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 10
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the HugoBlox Kit demo site
    content:
      title: 👉 Хочешь такой же сайт?
      text: |-
        Этот сайт создан с помощью **HugoBlox Kit** — бесплатного конструктора академических сайтов с открытым кодом. Им пользуются более 250 000 исследователей по всему миру.

        <a class="github-button" href="https://github.com/HugoBlox/kit" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/kit on GitHub">Star</a>

        Создавай сайт из готовых блоков — без программирования!

        От личных страниц и блогов до курсов и конференций.
      button:
        text: Начать
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-300 dark:bg-primary-700'
        css_style: ''
---
