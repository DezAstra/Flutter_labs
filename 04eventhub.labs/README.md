# Stateful Click Counter

A new Flutter project created with FlutLab - https://flutlab.io

## Getting Started

A few resources to get you started if this is your first Flutter project:

- https://flutter.dev/docs/get-started/codelab
- https://flutter.dev/docs/cookbook

For help getting started with Flutter, view our
https://flutter.dev/docs, which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Getting Started: FlutLab - Flutter Online IDE

- How to use FlutLab? Please, view our https://flutlab.io/docs
- Join the discussion and conversation on https://flutlab.io/residents


____________________________________
# Лабораторная работа №4 — Flutter: Приложение «EventHub»

**Курс:** Мобильная разработка  
**Среда разработки:** [FlutLab.io](https://flutlab.io)

## Описание

EventHub — планировщик мероприятий с сеткой событий, фильтрацией, BottomSheet-формой, деталями и статистикой.

## Критерии приёмки

| Критерий | Статус |
|----------|--------|
| Приложение запускается без ошибок | выполнено |
| Сетка (GridView) по 2 карточки в ряд | выполнено |
| Фильтрация через ChoiceChip, «Все» показывает все | выполнено |
| FAB открывает BottomSheet с формой | выполнено |
| В форме: TextField, DropdownButton, DatePicker, TimePicker | выполнено |
| Новое событие появляется в сетке | выполнено |
| Нажатие на карточку открывает экран деталей | выполнено |
| ExpansionTile для описания и участников | выполнено |
| Свайп удаляет карточку + SnackBar с «Отменить» | выполнено |
| Строка статистики под фильтром | выполнено |

## Самостоятельные задания

### Задание 1 — Редактирование события (базовое)
- `IconButton(Icons.edit)` в AppBar экрана деталей
- Открывает тот же BottomSheet, но предзаполненный данными события
- Поля `Event` не `final` — мутируются напрямую, `setState` обновляет сетку

### Задание 2 — Поиск и сортировка (среднее)
- AppBar трансформируется в `TextField` при нажатии `Icons.search`
- Поиск фильтрует по названию в реальном времени
- `PopupMenuButton(Icons.sort)`: сортировка по дате, названию, категории
- Фильтр по категории и поиск работают одновременно

### Задание 3 — Экран статистики (продвинутое)
- Кнопка `Icons.pie_chart` в AppBar открывает `StatisticsScreen`
- Карточки по каждой категории с `CircularProgressIndicator` (доля от общего числа) и `LinearProgressIndicator`
- Сводка: общее количество событий и ближайшее по дате
- Раздел «Ближайшие 3 события» с `ExpansionTile` для каждого

## Новые виджеты

| Виджет | Применение |
|--------|-----------|
| `GridView.count` | Сетка карточек событий по 2 в ряд |
| `ChoiceChip` | Горизонтальный фильтр по категориям |
| `showModalBottomSheet` | Форма добавления/редактирования событий |
| `DropdownButtonFormField` | Выбор категории |
| `showDatePicker` / `showTimePicker` | Выбор даты и времени |
| `Dismissible` | Удаление карточки свайпом |
| `ExpansionTile` | Описание, участники, ближайшие события |
| `StatefulBuilder` | Состояние внутри BottomSheet |
| `Positioned` (в `Stack`) | Эмодзи-фон на баннере деталей |
| `PopupMenuButton` | Меню сортировки |
| `CircularProgressIndicator` | Доля категории на экране статистики |

## Как запустить

1. Открыть [flutlab.io](https://flutlab.io)
2. Создать новый проект «Flutter Default Project»
3. Заменить содержимое `lib/main.dart` на код из этого репозитория
4. Нажать **Build**