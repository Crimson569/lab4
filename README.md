# Лабораторная работа №4: CSS-библиотеки.

## Лендинг на Bootstrap
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/74c5d5e9-d896-4411-b84a-331944712844" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9f73d154-0bc9-4b58-b485-45c8f5095dfb" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0d2ca6ea-fbf4-4222-82cc-bb87daa8078f" />


## Лендинг на Tailwind
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5ebf458b-1540-4ac6-8fa0-e9c3f3978047" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1581f35f-845d-47ac-9878-eb665deadd18" />

#Ответы на вопросы:
## -Какой подход (компонентный Bootstrap или utility-first Tailwind) показался вам удобнее для этой задачи и почему?
### -Bootstrap показался мне удобнее, так как он предоставляет уже готовые, комплексные стили. Однако он неудобен когда нам необходима более гибкая стилизация нашей страницы, для этого необходимо изменять компоненты библиотеки или использовать стандартный CSS. Tailwind в свою очередь удобен когда необходима гибкость в стилизации страницы. Однако код с его использованием получается громоздким и плохо-читаемым. Tailwind не очень подходит для небольших проектов.
## -Приведите пример кода для одного и того же элемента (например, кнопки) на Bootstrap и на Tailwind из вашей работы. В чем ключевое различие в разметке?
### -Bootstrap:
```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
        <div class="container">
            <a class="navbar-brand fw-bold" href="#">AI Assistant Pro</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#hero">Главная</a></li>
                    <li class="nav-item"><a class="nav-link" href="#about">О продукте</a></li>
                    <li class="nav-item"><a class="nav-link" href="#features">Преимущества</a></li>
                    <li class="nav-item"><a class="nav-link" href="#footer">Контакты</a></li>
                </ul>
            </div>
        </div>
    </nav>
```
### -Tailwind:
```html
<nav class="relative w-full bg-gray-900 text-white z-50">
    <div class="container mx-auto flex items-center justify-between px-4 py-3">
      <a href="#" class="text-xl font-bold">AI Assistant Pro</a>
      <button id="menu-toggle" class="lg:hidden focus:outline-none">
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"/>
        </svg>
      </button>

      <ul id="menu" class="hidden lg:flex space-x-6">
        <li><a href="#hero" class="hover:text-primary">Главная</a></li>
        <li><a href="#about" class="hover:text-primary">О продукте</a></li>
        <li><a href="#features" class="hover:text-primary">Преимущества</a></li>
        <li><a href="#footer" class="hover:text-primary">Контакты</a></li>
      </ul>
    </div>

    <!-- Мобильное меню -->
    <div id="mobile-menu" class="hidden lg:hidden bg-gray-800">
      <ul class="flex flex-col space-y-2 px-4 py-3">
        <li><a href="#hero" class="hover:text-primary">Главная</a></li>
        <li><a href="#about" class="hover:text-primary">О продукте</a></li>
        <li><a href="#features" class="hover:text-primary">Преимущества</a></li>
        <li><a href="#footer" class="hover:text-primary">Контакты</a></li>
      </ul>
    </div>
  </nav>
```
## -С какими сложностями вы столкнулись при работе с каждой из библиотек?
### -В Tailwind и Bootstrap множество классов-стилей названы неинтуитивно, из-за чего не всегда понятно, какой за что отвечает.
## -Какой блок вы добавили дополнительно?
### -В Bootstrap лендинге блок отзывов.
### -В Tailwind лендинге блок для контактной связи.
## -Какие запросы вы использовали для помощи ИИ? Насколько полезными были ответы?
```
Сгенерируй адаптивный лендинг для вымышленного продукта (например, "AI Assistant Pro") с использованием Bootstrap 5. Пусть будет хедер, секция с описанием, блок преимуществ (3 карточки), футер. Добавь теги meta для адаптивности.
```
```
страница должна иметь Навигационную панель (<nav class="navbar">...). ○ Главный экран («hero section») с заголовком и кнопкой (<div class="container">..., <button class="btn btn-primary">). ○ Секцию с описанием продукта (<section class="about">…) ○ Секцию с тремя карточками преимуществ продукта (<div class="card">...). ○ Подвал с навигацией (<footer>...).
```
```
Создай идентичную страницу, но полностью замени bootstrap на tailwind. Подключи Tailwind через CDN
```
```
«Сгенерируй блок отзывов для страницы, использующей библиотеку Bootstrap»
```
```
«Создай контактную форму для лендинга с Tailwind»
```
### Ответы оказались полезными, однако при генерации страницы с использованием Tailwind ИИ допустил ошибку в позиционировании навигационного блока.

