# 🤝 Skill Swap

**Платформа для взаимного обмена навыками.**

> ⚠️ **Командный проект**. Платформа для взаимного обмена навыками - одностраничное веб-приложение (SPA) по модели «Я научу / Хочу научиться».

🔗 [🚀 Посмотреть демо](https://skill-swap-42-3.vercel.app/)

---

## 👨‍💻 Мой вклад в проект

### 🧱 Разработка UI-компонентов
- **Модальное окно** — универсальный компонент с логикой открытия/закрытия
- **Формы и элементы управления** — поиск, кнопки, чекбоксы, текстовые поля, календарь
- **Dropdown** — меню для перехода в личный кабинет

### ⚙️ Логика и хуки
- **Кастомные хуки** — вынесение переиспользуемой логики
- **Интерактив** — обработка лайков и кнопки «Предложить обмен»
- **Валидация** — проверка ввода в формах

### 🎨 Стилизация и поддержка кода
- **CSS-переменные** — настройка дизайн-системы и темизации
- **Шрифты** — подключение и оптимизация
- **Рефакторинг** — улучшение и оптимизация компонентов, написанных коллегами
- **Layouts** — разработка базовой структуры страниц

---

## 🛠 Стек технологий

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Redux](https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white)
![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

---

## Инструкция по запуску

### Установка зависимостей и запуск сервера

```
npm i && npm run dev
```

### Данные пользователя для теста

```
email: ivan@mail.ru
password: 12345678
```

## 🚀 Скрипты

```
- npm run dev Запуск dev-сервера Vite (localhost:5173)
- npm run build Сборка TypeScript + Vite проекта для продакшена
- npm run preview Превью продакшен сборки локально
- npm run lint Проверка кода на соответствие ESLint правилам
- npm run lint:fix Автоисправление ошибок ESLint
- npm run format Форматирование файлов через Prettier
- npm run check Полная проверка проекта: stylelint + eslint + prettier
- npm run commit Прогон check + commit через commitizen
- npm run prepare
- npm run lint-staged
- npm run storybook
- npm run build-storybook
- npm run cypress:open
```

## 📚 Структура проекта

```
src/
├── api/                 # Методы для работы с данными
│   ├── skillsApi/       # Функции для получание навыков с сервера ( getSkills(), getSkillById(id) )
│   ├── usersApi/        # Функции для получание пользователей с сервера ( getUser(id) )
│   ├── auth/            # Функции для авторизации пользователя
│   ├── likes/           # Лайки пользователя
│   └── requests/        # Заявки на обмен
├── app/                 # Конфигурация приложения
│   ├── layout/          # Компоненты компоновки страниц
│   ├── providers/       # Провайдеры для React Context, Redux и темы ( AppProvider.tsx )
│   ├── router/          # Конфигурация маршрутов ( AppRouter.tsx, ProtectedRoute.tsx, routes.ts )
│   ├── store/           # Redux Toolkit store и slices ( authSlice.ts, skillsSlice.ts, requestsSlice.ts )
│   └── styles/          # Глобальные стили, переменные
├── assets/              # статические ресурсы ( изображения, шрифты, икноки и svg )
│   ├── images/          # иллюстрации, фотографии навыков
│   ├── icons/           # иконки кнопок, SVG
│   └── fonts/           # шрифты
├── entities/            # модели домена, сущности приложения (типы, модели)
│   ├── Skill.ts         # интерфейс
│   ├── User.ts/         # интерфейс
│   └── Request.ts/      # интерфейс
├── features/            # бизнес логика приложения
│   ├── auth/            # login, register, хранение токена, редиректы
│   ├── skills/          # фильтры, поиск, карточки навыков
│   ├── likes/           # идобавление/удаление навыков из избранного
│   └── requests/        # управление заявками
├── mocks/               # мок сервисы
├── pages/               # Лениво загружаемые страницы приложения
├── shared/              # Переиспользуемые модули, библиотеки и ui
│   ├── ui/              # атомы/молекулы (Button, Input, Card, Loader)
│   ├── hooks/           # кастомные хуки
│   └── lib/             # вспомогательные функции
├── widgets/             # Композитные блоки, готовые UI-компоненты
│   ├── header/          #
│   ├── footer/          #
│   ├── skillCard/       # карточка навыка с кнопками
│   └── Sceletons/       # скелетоны загрузки
└── main.tsx/            # точка входа
public/
├── db/                  # json данные
└── mockServiceWorker.js # MSW worker
```
