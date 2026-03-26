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
# Лабораторная работа №1 — Flutter UI: Профиль пользователя

**Среда разработки:** [FlutLab.io](https://flutlab.io)

## Описание

Приложение «Мой профиль» — учебный проект, демонстрирующий базовые возможности Flutter для построения пользовательского интерфейса.

## Структура приложения

```
lib/
└── main.dart       # Весь код приложения
```

## Реализованные части

### Части 1–5 (основное задание)
- Каркас приложения: `MaterialApp`, `Scaffold`, `AppBar`
- Экран профиля с аватаром, именем и статусом
- Информационные карточки (`Card`, `ListTile`)
- Теги интересов (`Chip`, `Wrap`)
- Интерактивность: счётчик лайков (`StatefulWidget`, `setState`)
- Навигация на экран «О приложении» (`Navigator.push`)

### Задание 1 — Персонализация профиля (базовое)
- Данные профиля заменены на свои
- Цветовая тема изменена на `Colors.deepPurple`
- Добавлена карточка «GitHub»

### Задание 2 — Переключение темы (среднее)
- `MyApp` переведён на `StatefulWidget`
- Кнопка в `AppBar` переключает между светлой и тёмной темой
- Функция `onToggleTheme` передаётся через параметры конструктора

### Задание 3 — Три вкладки (продвинутое)
- `BottomNavigationBar` с тремя вкладками
- **Профиль** — основной экран
- **Галерея** — `GridView.count` с изображениями из сети
- **Контакты** — `ListView.builder` с 5 контактами

## Виджеты

| Виджет | Применение |
|--------|-----------|
| `MaterialApp` | Корень приложения, темы |
| `Scaffold` | Каркас каждого экрана |
| `AppBar` | Верхняя панель с кнопками |
| `Column` / `Row` | Компоновка |
| `Card` / `ListTile` | Информационные блоки |
| `CircleAvatar` | Аватары |
| `Chip` / `Wrap` | Теги интересов |
| `ElevatedButton` | Кнопка «Нравится» |
| `SnackBar` | Уведомления |
| `Navigator` | Переходы между экранами |
| `BottomNavigationBar` | Навигация по вкладкам |
| `GridView.count` | Сетка изображений |
| `ListView.builder` | Список контактов |

## Как запустить

1. Открыть [flutlab.io](https://flutlab.io)
2. Создать новый проект «Flutter Default Project»
3. Заменить содержимое `lib/main.dart` на код из этого репозитория
4. Нажать **Build**