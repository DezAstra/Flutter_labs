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
# Лабораторная работа №3 — Flutter: Приложение «FitDay»

**Курс:** Мобильная разработка  
**Среда разработки:** [FlutLab.io](https://flutlab.io)

## Описание

FitDay — трекер тренировок с четырьмя вкладками: тренировка, прогресс, настройки, история.

## Критерии приёмки 

| Критерий | Статус |
|----------|--------|
| Приложение запускается, отображает вкладки | выполнено |
| Вкладка «Тренировка»: 6+ упражнений с иконкой, названием, подходами | выполнено |
| Switch переключает выполнение, внешний вид меняется | выполнено |
| FAB открывает диалог добавления упражнения | выполнено |
| Вкладка «Прогресс»: 3 карточки с прогресс-барами | выполнено |
| Прогресс обновляется при отметке упражнений | выполнено |
| Вкладка «Настройки»: переключатели + слайдер калорий | выполнено |
| Переключение вкладок через TabBar | выполнено |

## Самостоятельные задания

### Задание 1 — Удаление упражнений (базовое)
- Длинное нажатие (`onLongPress`) на упражнение → `AlertDialog` с подтверждением
- `todayWorkout.removeAt(index)` удаляет упражнение
- Прогресс пересчитывается автоматически

### Задание 2 — История тренировок (среднее)
- Четвёртая вкладка «История» (`Icons.history`)
- Кнопка «Завершить день» сохраняет тренировку в глобальный список `history`
- Карточки с датой, упражнениями, калориями и временем
- После сохранения список тренировки сбрасывается на начальные данные

### Задание 3 — Таймер упражнения (продвинутое)
- Нажатие на упражнение открывает `TimerScreen`
- Обратный отсчёт 30 секунд с круговым `CircularProgressIndicator`
- Кнопки «Старт», «Пауза», «Сброс»
- При достижении 00:00 — `SnackBar` «Подход завершён! 💪»
- Таймер меняет цвет: зелёный → teal → красный (последние 10 сек)

## Новые виджеты

| Виджет | Применение |
|--------|-----------|
| `TabBar` + `TabBarView` | Четыре вкладки приложения |
| `Switch` / `SwitchListTile` | Отметка упражнений, настройки |
| `Slider` | Цель по калориям |
| `LinearProgressIndicator` | Прогресс-бары на вкладке «Прогресс» |
| `CircularProgressIndicator` | Таймер на экране упражнения |
| `FloatingActionButton` | Добавление упражнения |
| `AlertDialog` | Добавление, удаление, сброс, завершение дня |
| `Stack` | Наложение контента на градиент в карточках |
| `Timer` (dart:async) | Обратный отсчёт в таймере |

## Как запустить

1. Открыть [flutlab.io](https://flutlab.io)
2. Создать новый проект «Flutter Default Project»
3. Заменить содержимое `lib/main.dart` на код из этого репозитория
4. Нажать **Build**