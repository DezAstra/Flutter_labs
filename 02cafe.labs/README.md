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
# Лабораторная работа №2 — Flutter: Приложение «Меню кафе»

**Курс:** Мобильная разработка  
**Среда разработки:** [FlutLab.io](https://flutlab.io)

## Описание

Приложение «Кафе "У Flutter"» — трёхэкранный каталог меню с навигацией, корзиной и поиском.

## Структура приложения

```
lib/
└── main.dart       # Весь код приложения
```

## Навигация

```
Список категорий → Список блюд → Карточка блюда
       ↓
    Корзина (из AppBar)
```

## Реализованные части

### Части 1–4 (основное задание)
- Модели данных: `Dish`, `Category`
- Экран категорий с градиентными карточками (`ListView.builder`, `LinearGradient`, `InkWell`)
- Экран блюд с передачей данных через конструктор
- Детальная карточка блюда: счётчик количества, кнопка «В заказ», `SnackBar`

### Задание 1 — Новая категория (базовое)
- Добавлена категория «Основные блюда» 🍽️ с 3 блюдами

### Задание 2 — Корзина (среднее)
- Глобальный список `cart`
- Кнопка корзины с бейджем в AppBar
- Экран `CartScreen`: список позиций, удаление, итоговая сумма, оформление заказа

### Задание 3 — Поиск (продвинутое)
- `TextField` поиска на экране категорий
- `CategoriesScreen` переведён на `StatefulWidget`
- Фильтрация по всем блюдам всех категорий
- При пустом поиске — список категорий, при вводе — результаты

## Виджеты

| Виджет | Применение |
|--------|-----------|
| `ListView.builder` | Списки категорий, блюд, корзины |
| `InkWell` | Нажимаемые карточки |
| `LinearGradient` | Фон карточек категорий |
| `Container` + `BoxDecoration` | Скруглённые блоки для эмодзи и цен |
| `Expanded` | Предотвращение переполнения в `Row` |
| `Navigator.push` | Переходы между тремя экранами |
| `StatefulWidget` | Счётчик порций, поиск, корзина |
| `TextField` | Строка поиска |
| `Stack` + `Positioned` | Бейдж на иконке корзины |

## Как запустить

1. Открыть [flutlab.io](https://flutlab.io)
2. Создать новый проект «Flutter Default Project»
3. Заменить содержимое `lib/main.dart` на код из этого репозитория
4. Нажать **Build**