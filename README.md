itdeas-app/
├── public/ # Статические файлы
│ ├── index.html # Основной HTML файл
│ ├── favicon.ico # Иконка сайта
│ ├── robots.txt # Для поисковых роботов
│ └── manifest.json # PWA манифест
├── src/ # Исходный код приложения
│ ├── assets/ # Статические ресурсы
│ │ ├── images/ # Изображения
│ │ │ ├── icons/ # Иконки
│ │ │ ├── logos/ # Логотипы
│ │ │ └── illustrations/ # Иллюстрации
│ │ ├── fonts/ # Шрифты
│ │ └── styles/ # Глобальные стили
│ │ ├── main.scss # Главный файл стилей
│ │ ├── \_variables.scss # CSS переменные
│ │ ├── \_mixins.scss # SCSS миксины
│ │ ├── \_base.scss # Базовые стили
│ │ ├── \_components.scss # Стили компонентов
│ │ └── \_utilities.scss # Вспомогательные классы
│ ├── components/ # Переиспользуемые компоненты
│ │ ├── ui/ # Базовые UI компоненты
│ │ │ ├── BaseButton.vue
│ │ │ ├── BaseInput.vue
│ │ │ ├── BaseModal.vue
│ │ │ ├── BaseCard.vue
│ │ │ ├── BaseAvatar.vue
│ │ │ ├── BaseLoader.vue
│ │ │ ├── BaseToast.vue
│ │ │ └── index.js # Экспорт компонентов
│ │ ├── layout/ # Компоненты layout'а
│ │ │ ├── AppHeader.vue
│ │ │ ├── AppFooter.vue
│ │ │ ├── AppSidebar.vue
│ │ │ ├── AppLayout.vue
│ │ │ └── Navigation/
│ │ │ ├── Navbar.vue
│ │ │ └── SidebarMenu.vue
│ │ ├── ideas/ # Компоненты для идей
│ │ │ ├── IdeaCard.vue
│ │ │ ├── IdeaList.vue
│ │ │ ├── IdeaForm.vue
│ │ │ └── IdeaFilters.vue
│ │ ├── messenger/ # Компоненты мессенджера
│ │ │ ├── ConversationList.vue
│ │ │ ├── MessageList.vue
│ │ │ ├── MessageBubble.vue
│ │ │ ├── MessageInput.vue
│ │ │ └── ChatHeader.vue
│ │ └── common/ # Общие компоненты
│ │ ├── EmptyState.vue
│ │ ├── ErrorState.vue
│ │ ├── SearchBar.vue
│ │ └── UserAvatar.vue
│ ├── views/ # Страницы приложения
│ │ ├── auth/ # Авторизация
│ │ │ ├── LoginView.vue
│ │ │ ├── RegisterView.vue
│ │ │ └── ForgotPasswordView.vue
│ │ ├── ideas/ # Идеи
│ │ │ ├── FeedView.vue
│ │ │ ├── IdeaDetailView.vue
│ │ │ ├── CreateIdeaView.vue
│ │ │ └── EditIdeaView.vue
│ │ ├── messenger/ # Мессенджер
│ │ │ ├── MessengerView.vue
│ │ │ ├── ConversationView.vue
│ │ │ └── NewConversationView.vue
│ │ ├── profile/ # Профиль
│ │ │ ├── ProfileView.vue
│ │ │ ├── ProfileEditView.vue
│ │ │ └── SettingsView.vue
│ │ ├── HomeView.vue # Главная страница
│ │ ├── AboutView.vue # О проекте
│ │ ├── NotFoundView.vue # 404 страница
│ │ └── MaintenanceView.vue # Техработы
│ ├── composables/ # Композаблы (Composition API)
│ │ ├── useApi.js
│ │ ├── useAuth.js
│ │ ├── useIdeas.js
│ │ ├── useMessenger.js
│ │ ├── useNotifications.js
│ │ ├── useForm.js
│ │ ├── usePagination.js
│ │ └── index.js # Экспорт композаблов
│ ├── stores/ # Хранилища (Pinia)
│ │ ├── modules/
│ │ │ ├── auth.store.js
│ │ │ ├── user.store.js
│ │ │ ├── ideas.store.js
│ │ │ ├── messenger.store.js
│ │ │ ├── notifications.store.js
│ │ │ └── ui.store.js
│ │ └── index.js # Экспорт хранилищ
│ ├── router/ # Маршрутизация
│ │ ├── index.js # Главный роутер
│ │ ├── routes/ # Маршруты
│ │ │ ├── auth.routes.js
│ │ │ ├── ideas.routes.js
│ │ │ ├── messenger.routes.js
│ │ │ ├── profile.routes.js
│ │ │ └── index.js # Объединение маршрутов
│ │ └── guards/ # Защитники маршрутов
│ │ ├── auth.guard.js
│ │ ├── guest.guard.js
│ │ └── admin.guard.js
│ ├── services/ # Сервисы API
│ │ ├── api.js # Базовый API клиент
│ │ ├── auth.service.js
│ │ ├── user.service.js
│ │ ├── ideas.service.js
│ │ ├── messenger.service.js
│ │ ├── upload.service.js # Загрузка файлов
│ │ └── socket.service.js # WebSocket сервис
│ ├── utils/ # Вспомогательные утилиты
│ │ ├── constants.js # Константы приложения
│ │ ├── helpers.js # Вспомогательные функции
│ │ ├── validators.js # Валидаторы форм
│ │ ├── formatters.js # Форматтеры данных
│ │ ├── debounce.js # Дебаунс функции
│ │ ├── storage.js # Работа с localStorage
│ │ └── errors.js # Обработка ошибок
│ ├── types/ # TypeScript типы (опционально)
│ │ ├── user.ts
│ │ ├── idea.ts
│ │ ├── message.ts
│ │ ├── api.ts
│ │ └── index.ts
│ ├── locales/ # Локализация (i18n)
│ │ ├── en.json
│ │ ├── ru.json
│ │ └── index.js
│ ├── config/ # Конфигурация приложения
│ │ ├── app.config.js # Настройки приложения
│ │ ├── api.config.js # Настройки API
│ │ └── theme.config.js # Настройки темы
│ ├── App.vue # Корневой компонент
│ ├── main.js # Точка входа
│ └── error-handler.js # Глобальная обработка ошибок
├── tests/ # Тесты
│ ├── unit/ # Юнит-тесты
│ │ ├── components/
│ │ ├── composables/
│ │ ├── stores/
│ │ └── utils/
│ ├── e2e/ # End-to-end тесты
│ │ ├── specs/
│ │ ├── pages/
│ │ └── support/
│ └── fixtures/ # Фикстуры для тестов
├── dist/ # Собранное приложение (генерируется)
├── node_modules/ # Зависимости (генерируется)
├── .env # Переменные окружения
├── .env.development # Переменные для разработки
├── .env.production # Переменные для production
├── vite.config.js # Конфигурация Vite
├── package.json # Зависимости и скрипты
├── jsconfig.json # Конфигурация JavaScript
├── .eslintrc.js # Конфигурация ESLint
├── .prettierrc # Конфигурация Prettier
├── .gitignore # Игнорируемые файлы Git
├── README.md # Документация проекта
└── CHANGELOG.md # История изменений
