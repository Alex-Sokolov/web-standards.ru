# Веб-стандарты

Новый сайт сообщества: статьи, конференция, календарь, подкаст и всё остальное.

## Дизайн

[Макет в Figma](https://www.figma.com/file/kHj7Cs5lJsKDgFZS0UjOij/milestone-1).

## Разработка

- Установка зависимостей: `npm install`
- Старт сервера для локальной разработки: `npm start`
- Запуск сборки для деплоя: `npm run build`

---
Работает на [Eleventy](https://www.11ty.io/).

## Как помочь проекту
Вы можете выбрать [ишу](https://github.com/web-standards-ru/nouvelle/issues). Для удобства понимания, какие этапы разработки сайта заведены [проекты](https://github.com/web-standards-ru/nouvelle/projects), относитесь к ним, как к майлстоунам. Для удобства, у задач указаны требуемые навыки в лейблах — фильтруйте по ним, что нравится.

Форкните и присылайте пуллреквесты.

## Как работает сайт
Движок e11ty собирает маркдаун или json и насыщает этими данными njk-шаблоны страниц, генерируя на выходе статичные html-страницы. Стили пишутся на чистом CSS, соединяются импортами и потом ещё сожмутся и оптимизируются.

Все возможные конфигурации бережно хранятся в соответствующих файликах.

## Принципы верстки
**mobile-first.** Сначала мы делаем мобильную версию интерфейса, а потом начинаем увеличить с помощью `@media`. Например, кнопка открытия главного меню спрячется, когда для меню будет достаточно места на экране.

**Нет брекпоинтов для адаптации.** Каждый компонент для себя решает, когда ему адаптироваться. Например, когда пункты меню начинают помещаться — пора развернуть его во всю ширину и спрятать кнопку-гамбургер.
