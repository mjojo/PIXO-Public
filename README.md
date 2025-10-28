=======
# PIXO - Professional Pixel Art Maker


```
██████╗ ██╗██╗  ██╗ ██████╗ 
██╔══██╗██║╚██╗██╔╝██╔═══██╗
██████╔╝██║ ╚███╔╝ ██║   ██║
██╔═══╝ ██║ ██╔██╗ ██║   ██║
██║     ██║██╔╝ ██╗╚██████╔╝
╚═╝     ╚═╝╚═╝  ╚═╝ ╚═════╝ 
```

## 🚀 VERSION 2.9.3 - REFERENCE & DITHERING TOOLS - RELEASED! 🎉

Мощный профессиональный редактор пиксельной графики, анимации и тайлсетов, созданный на Godot Engine 4.5. Превосходит Aseprite по функционалу работы с тайлами и автотайлингом.

**Разработчик:** BitVit (mjojo GLK Dev)  
**Текущая версия:** 2.9.3 ✅ **PRODUCTION READY**  
**Дата релиза:** 22 октября 2025

---

## ⚡ Что нового в v2.9.3 - REFERENCE & DITHERING TOOLS:

### 🎲 Dithering System (NEW!)

**Профессиональный дизеринг для ретро пиксель-арта!**

#### Возможности:
- 🎨 **7 Dithering Patterns** - Bayer (2×2, 4×4, 8×8), Ordered (3×3, 4×4), Checkerboard, Diagonal
- 🖌️ **Dithering Brush** - кисть 4-64px с настраиваемой плотностью (0-100%)
- 🌊 **Floyd-Steinberg** - high-quality error diffusion алгоритм для плавных градиентов
- 📊 **Threshold Dithering** - pattern-based дизеринг для ретро-эстетики
- 🌈 **Gradient Mode** - плавные переходы цветов с дизерингом
- 👁️ **Real-time Preview** - 8×8 превью паттерна на курсоре
- 💾 **Pattern Import/Export** - сохранение и загрузка custom паттернов
- 🎯 **Perfect for:** Retro games (GB, NES, C64), limited palette art, texture creation

### 🖼️ Moodboard - Reference Manager (NEW!)

**Floating панель для работы с референсами без импорта в проект!**

#### Возможности:
- 📁 **Multi-Image Support** - PNG/JPG/WebP с auto-thumbnails
- 🔄 **Transform Controls:**
  - 🖱️ Drag - перемещение
  - 🔄 Mouse Wheel - масштабирование
  - 🔁 Ctrl+Drag - вращение
- 🎨 **Eyedropper Integration** - pick цветов прямо из референсов → палитра
- 📑 **Z-Index Layering** - контроль порядка отображения
- 💾 **Project Persistence** - сохраняется с .pixo файлом
- 🔒 **Lock System** - защита от случайных изменений
- 🎯 **Perfect for:** Character design, color extraction, composition planning, style references

---

## 📚 Previous Updates - v2.9 ANIMATION & PERFORMANCE SUITE:

### 🎬 Animation Timeline UI (NEW!)

**Профессиональная визуальная шкала времени анимации!**

#### Возможности:
- 📽️ **Visual Timeline** - визуальная шкала времени с превью кадров (64×64)
- 🎮 **Playback Controls** - полное управление воспроизведением (Play/Pause, First/Prev/Next/Last)
- ⌨️ **Keyboard Shortcuts** - Space (Play/Pause), Left/Right (Prev/Next), Home/End (First/Last)
- 👻 **Onion Skinning** - показ предыдущих/следующих кадров как полупрозрачных слоёв
- 🖼️ **Frame Thumbnails** - автоматическая генерация превью для всех кадров
- ➕ **Frame Management** - добавление, дублирование, удаление кадров из таймлайна
- 🔄 **Auto-Update** - автоматическое обновление при изменении кадров

### 📦 Sprite Sheet Generator (NEW!)

**Оптимизированная генерация спрайтшитов с 4 режимами упаковки!**

#### Режимы упаковки:
- ➡️ **HORIZONTAL** - горизонтальная полоса (для простых анимаций)
- ⬇️ **VERTICAL** - вертикальная полоса (для UI анимаций)
- 🔲 **GRID** - сетка NxM (оптимальный размер)
- 📐 **COMPACT** - компактная упаковка (минимум пустого места)

#### Функции:
- 🎯 **Power-of-2 Sizing** - NONE/FIT/EXPAND (для игровых движков)
- ✂️ **Trim Transparent** - обрезка прозрачных пикселей
- 💾 **Export Formats** - PNG + JSON/XML метаданные
- 📊 **Frame Metadata** - позиции, размеры, длительность кадров

### 📊 Performance Profiler (NEW!)

**Инструмент мониторинга производительности в реальном времени!**

#### Метрики:
- 📈 **FPS Tracking** - текущий и средний FPS
- 💾 **Memory Monitoring** - отслеживание использования памяти
- 🎨 **Draw Calls Estimation** - оценка нагрузки рендеринга
- 💡 **Optimization Suggestions** - автоматические рекомендации по оптимизации
- 📊 **Real-time Display** - обновление метрик в реальном времени

### 🗺️ Advanced Tilemap Tools (NEW!)

**Профессиональные инструменты для работы с тайлмапами!**

#### Инструменты:
- 🖌️ **Tilemap Brush** - кисть с поворотом, отзеркаливанием, случайным выбором тайлов
- 📚 **Multi-layer Support** - управление несколькими слоями тайлмапа
- 🎨 **Tile Picker** - eyedropper для выбора тайлов с canvas
- 🌊 **Flood Fill** - заливка области одним тайлом (BFS алгоритм)
- 🔄 **Rotation & Flip** - 4 режима поворота, горизонтальное/вертикальное отзеркаливание

### 🎓 Tutorial System (NEW!)

**Интерактивная система обучения с локализацией!**

#### Возможности:
- 📖 **16-Step Tutorial** - пошаговое обучение основам PIXO
- 🌍 **Multi-language** - Русский и Английский (автоопределение языка)
- ⌨️ **Keyboard Shortcuts** - N/P (Next/Previous), Esc (Close)
- 📊 **Progress Tracking** - отслеживание прогресса с сохранением
- ✨ **Action Validation** - проверка выполнения действий пользователем
- 🎯 **Pixel Tracking** - отслеживание количества нарисованных пикселей

**Статус v2.9:** ✅ **100% COMPLETE** | **[SESSION SUMMARY](SESSION_SUMMARY_V2.7-2.9.md)**

---

## 🚀 VERSION 2.6.1 - PERFORMANCE & BUG FIXES - RELEASED! 🎉

Мощный профессиональный редактор пиксельной графики, анимации и тайлсетов, созданный на Godot Engine 4.5. Превосходит Aseprite по функционалу работы с тайлами и автотайлингом.

**Разработчик:** BitVit (mjojo GLK Dev)  
**Текущая версия:** 2.6.1 ✅ **PRODUCTION READY**  
**Дата релиза:** 19 октября 2025

---

## ⚡ Что нового в v2.6.1 - PERFORMANCE & BUG FIXES:

### 🚀 Performance Optimizations (NEW!)

**Критические исправления производительности - 60-100× улучшение!**

#### Оптимизации:
- ⚡ **Deferred Display Updates** - отложенное обновление дисплея (50% меньше overhead)
- � **Cache Invalidation Optimization** - 60-100× меньше инвалидаций кэша
- 🔄 **Queue Redraw Loop Prevention** - устранение бесконечных циклов перерисовки
- 🖌️ **Line Tool Preview Performance** - 20-100× быстрее превью Line tool
- 🗑️ **Eliminated Console Spam** - больше нет "[CACHE] Rendering new composite"

#### Метрики производительности:
```
Cache Invalidations: 7,176 → 1 (7,176× улучшение)
Line Preview Calls:  10,000+ → 100-500 (20-100× улучшение)
Render Loops:        2-3 → 1 (2-3× улучшение)
Console Spam:        60+ msg/sec → 0 (∞ улучшение)
Memory Allocations:  High → Low (50-70% reduction)
```

### 🐛 Bug Fixes (NEW!)

**Исправлены критические баги Line tool!**

#### Фиксы:
- ✅ **Line Mirroring Bug** - линии больше не рисуются зеркально/инвертированно
- ✅ **Drawing Functionality Restored** - восстановлена работа рисования после оптимизаций
- ✅ **Symmetry Fixed** - симметрия работает корректно во всех направлениях
- ⚡ **Cache Reuse** - кэш теперь переиспользуется вместо пересоздания

**Статус v2.6.1:** ✅ **100% COMPLETE** | **[RELEASE NOTES](RELEASE_V2.6.1.md)** | **[CHANGELOG](CHANGELOG.md)**

---

## 🎨 Что было в v2.6 - REFERENCE IMAGES & PIXEL PERFECT LINES:

### �️ Reference Image System (NEW!)

**Профессиональная система референсных изображений для скетчинга!**

#### Возможности:
- 📥 **Import PNG/JPEG** - загрузка референсов через View → Load Reference Image
- 👁️ **Non-destructive** - референс отображается позади canvas без изменения работы
- 🎚️ **Adjustable Opacity** - настройка прозрачности (0-100%, по умолчанию 50%)
- 👀 **Show/Hide Toggle** - быстрое переключение видимости (View → Show Reference Image)
- 🧹 **Clear Reference** - удаление референса одним кликом

### ✏️ Pixel Perfect Lines (NEW!)

**Улучшенный алгоритм рисования линий для идеальной пиксельной графики!**

#### Преимущества:
- 🎯 **Anti-Jaggies Algorithm** - минимизация "ступенек" на линиях
- �🖌️ **Smooth Rendering** - плавные эстетически приятные линии
- ⚡ **Better than Bresenham** - улучшенный алгоритм с интерполяцией
- 🎛️ **Toggle Control** - включение/выключение через View → Pixel Perfect Lines
- 🎨 **Pixel Art Optimized** - создан специально для пиксельной графики

### 🪞 Mirror Drawing Mode Improvements (NEW!)

**Улучшенная визуализация осей симметрии!**

#### Улучшения:
- - - **Dashed Guide Lines** - пунктирные линии вместо сплошных (профессиональный вид)
- 🔄 **Improved Radial Symmetry** - улучшенная визуализация радиальной симметрии
- 👁️ **Show/Hide Axes** - переключение видимости осей (View → Show Symmetry Axes)
- 🎨 **Better Aesthetics** - более чистый и профессиональный интерфейс рисования

**Статус v2.6:** ✅ **100% COMPLETE** | **[CHANGELOG](CHANGELOG.md)**

---

## 🛠️ Что нового в v2.5 - TOOL SYSTEM REFACTORING:

### 🔧 Tool System Architecture (NEW!)

**Полная реструктуризация системы инструментов для лучшей поддерживаемости!**

#### Изменения:
- 🏗️ **7 Tool Classes** - ToolBase, PencilTool, EraserTool, BucketTool, LineTool, RectangleTool, CircleTool
- 📦 **708 Lines of Clean Code** - выделение инструментов в отдельные классы
- 🐛 **12 Bugs Fixed** - исправлены проблемы с переключением, предпросмотром, симметрией
- 🧹 **240 Lines Removed** - очистка устаревшего кода
- 📑 **Tile Animation Tab** - перемещение из окна в TabContainer для лучшей UX

**Статус v2.5:** ✅ **100% COMPLETE** | **[CHANGELOG](CHANGELOG.md)**

---

## 🖌️ Что было в v2.3 - CUSTOM BRUSHES EDITION:

### � Custom Brushes System (NEW!)

**Профессиональная система кастомных кистей для выразительного рисования!**

#### Возможности:
- ✨ **8 встроенных кистей** - Square, Circle, Cross, Diagonal, Noise, Soft Circle, Grass, Star
- 🎛️ **Brush Panel UI** - визуальные превью, быстрый выбор (Ctrl+B)
- ⚙️ **Настраиваемые параметры** - Size (1-32), Spacing (0.5-2.0), Jitter (0.0-0.5)
- 📥 **Import/Export** - импорт PNG/JPG, сохранение в user://brushes/
- 🛠️ **Интеграция** - работает с Pencil, Line, Rectangle, Circle, Eraser
- ⚡ **Real-time drawing** - мгновенная визуальная обратная связь

**Статус v2.3:** ✅ **100% COMPLETE** | **[RELEASE NOTES](RELEASE_V2.3.md)**

### ✅ Предыдущие функции (v2.0-2.2):
- ✨ **Tile Animation Editor** - отдельное окно для создания анимаций
- 🎞️ **Multi-frame animations** - неограниченное количество кадров на тайл
- ⚡ **Live preview** - превью анимации в реальном времени на canvas
- 🎮 **Godot Export** - экспорт в AnimatedTexture одним кликом
- 📦 **Полная структура экспорта** - PNG кадры + .tres ресурсы + metadata

#### Технические характеристики:
```
FPS Control:      1-60 FPS
Loop Modes:       Loop, Ping-Pong, Once
Frame Management: Add, Remove, Reorder
Export Format:    Godot 4.5 AnimatedTexture (.tres)
File Output:      tiles/ + animations/ + metadata.json
```

#### Использование в Godot:
```gdscript
var animated_texture = load("res://animations/tile_0_animation.tres")
var sprite = Sprite2D.new()
sprite.texture = animated_texture
add_child(sprite)
# Анимация воспроизводится автоматически!
```

### ✅ Другие функции v2.0-2.2:
- **🎯 Tile Selection Tool** - выбор и перестановка тайлов с copy/paste
- **🎨 Tile Palette** - быстрый выбор тайлов из палитры
- **🔄 Auto-Tile System** - 3×3 автотайлинг с bitmask (RPG Maker style)
- **🌈 10 новых палитр** - Tileset Pro, RPG Terrain, Cyberpunk Neon и др.
- **💡 UI/UX Improvements** - статус-бар, подсказки, горячие клавиши (F1)
- **📦 Collision Shapes Editor** - визуальный редактор коллизий для тайлов
- **⚡ Performance Optimizations** - кэширование рендеринга (~100x ускорение)

**Статус v2.2:** ✅ **100% COMPLETE** (7/7 основных функций) | **[RELEASE NOTES](RELEASE_NOTES_V2.2_FINAL.md)**

---

## 💎 Ключевые особенности PIXO

### 🎨 **Мощные инструменты рисования**
- **14+ профессиональных инструментов:**
  - Рисование: Карандаш, Ластик, Заливка, Линия, Прямоугольник, Круг, Градиент
  - Выделение: Прямоугольное, Волшебная палочка, Перемещение
  - Дополнительно: Пипетка, Текст (bitmap шрифт), Tile Selection
- **Продвинутые возможности:**
  - 🖼️ **Reference Images** - скетчинг поверх референсов (v2.6)
  - ✏️ **Pixel Perfect Lines** - улучшенный алгоритм без "ступенек" (v2.6)
  - 🪞 **Mirror Drawing** - симметрия с пунктирными осями (v2.6)
  - 🖌️ **Custom Brushes** - 8 встроенных + импорт PNG/JPG (v2.3)
  - Симметричное рисование (Horizontal, Vertical, Quad, Radial)
  - Настройка размера кисти (1-32px) и параметров
  - Предпросмотр курсора в реальном времени
  - Алгоритм для плавных pixel-perfect линий

### 🏗️ **Профессиональная работа с тайлсетами** (v2.1+)
- Создание тайлсетов любого размера (8×8 до 128×128)
- Визуальная сетка тайлов
- Auto-Tile System с 3×3 bitmask (как в RPG Maker)
- Tile Palette для быстрого рисования
- Collision Shapes Editor (Rectangle, Circle, Polygon)
- Экспорт в Godot (.import файлы + collision data)
- Импорт существующих тайлсетов

### 📚 **Продвинутая система слоёв**
- Неограниченное количество слоёв
- 5 режимов наложения (Normal, Multiply, Screen, Overlay, Add)
- Настройка прозрачности (0-100%)
- Layer groups (планируется в v2.4)

### 🎬 **Анимация**
- Покадровая анимация
- Onion skinning (просмотр предыдущих/следующих кадров)
- Настройка FPS (1-60)
- Управление длительностью кадров
- Экспорт в sprite sheets
- 2D rigging (планируется в v3.0)

### 🎨 **31 профессиональная палитра**
- DB16, PICO-8, Game Boy (классика)
- Tileset Pro, RPG Terrain (для тайлсетов)
- Cyberpunk Neon, Pixel Fantasy (стилизованные)
- Retro Console, Dungeon Master (retro)
- Импорт/экспорт .pixopal и .gpl (GIMP)

### 🎭 **Фильтры и эффекты**
- 10 фильтров: Blur, Sharpen, Brightness/Contrast
- Hue/Saturation, Posterize, Dither
- Invert, Grayscale, и др.

### 💾 **Универсальные форматы**
- Собственный формат .pixo (полное сохранение)
- PNG импорт/экспорт
- Sprite sheet экспорт/импорт
- Godot integration (.import, .tres)
- Collision data (JSON, Godot)

### ⚡ **Производительность**
- 🚀 **v2.6.1 Optimizations** - 60-100× улучшение производительности!
- Кэширование рендеринга (~100x ускорение на idle)
- Оптимизация для больших холстов (512×512+)
- Устранение бесконечных циклов перерисовки
- Оптимизированное превью инструментов
- GPU acceleration (планируется в v3.0)

### 💰 **Marketplace & Monetization** (планируется v2.9.5-v3.0)
- 📦 **Create & Sell Assets:**
  - Custom Brushes (уникальные кисти)
  - Color Palettes (авторские палитры)
  - Tilesets (тайлсеты для игр)
  - Custom Tools (пользовательские инструменты)
  - Effect Presets (пресеты эффектов)
- 💼 **Seller Dashboard:**
  - Asset upload wizard
  - Sales analytics & revenue tracking
  - Payout system (Tokens → $)
- 🛒 **Integrated Asset Store:**
  - Browse & purchase community assets
  - One-click install
  - Auto-update system
- 🎨 **Platform for creators** - превращает PIXO в маркетплейс для заработка!

## Возможности

### 🎨 Инструменты рисования (Drawing Tools)
- **Карандаш (P)** - основной инструмент для пиксель-арта с настройкой размера кисти (1-10px)
- **Ластик (E)** - стирание пикселей с настройкой размера, работает как обратная кисть
- **Заливка (B)** - умная заливка области с учётом прозрачности и связности пикселей
- **Линия (L)** - рисование прямых линий по алгоритму Брезенхема (pixel-perfect)
- **Прямоугольник (R)** - рисование прямоугольников и квадратов с предпросмотром
- **Круг (C)** - рисование окружностей идеальной формы с предпросмотром
- **Градиент (G)** - линейный градиент между двумя точками с плавными переходами
- **Текст (T)** - встроенный bitmap шрифт 5×7 с масштабированием для pixel art надписей
- **Пипетка (I)** - быстрый выбор цвета с холста (также работает Alt+ЛКМ)

### ✂️ Инструменты выделения и трансформации (Selection Tools)
- **Выделение (S)** - прямоугольное выделение области с визуальной рамкой и маркерами
- **Волшебная палочка (W)** - умное выделение по цвету с настройкой толерантности (0-255)
- **Перемещение (M)** - перемещение выделенной области или всего слоя
- **Копировать/Вырезать/Вставить** - полная поддержка буфера обмена (Ctrl+C/X/V)
- **Трансформация** - поворот на 90°, отражение по горизонтали/вертикали
- **Delete** - удаление выделенной области (заполнение прозрачностью)

### 🖌️ Дополнительные возможности рисования
- **Симметричное рисование** - 4 режима (Horizontal, Vertical, Quad, Radial)
- **Настройка размера кисти** - от 1 до 10 пикселей для карандаша и ластика
- **Предпросмотр курсора** - визуализация размера и позиции для всех инструментов
- **Onion Skinning** - просмотр предыдущих/следующих кадров с полупрозрачностью
- **Grid (Сетка)** - помощь в выравнивании пикселей

### 👁️ Улучшения интерфейса
- **Предпросмотр курсора** - визуализация размера кисти и позиции для всех инструментов
- **Настройка размера кисти** - от 1 до 10 пикселей
- **Настройка толерантности** - для инструмента "Волшебная палочка"

### 📚 Система слоев
- Создание, удаление и управление слоями
- Перемещение слоев вверх/вниз
- Видимость слоев
- Работа с прозрачностью

### 🎬 Анимация
- Создание и редактирование кадров анимации
- Дублирование кадров
- Предварительный просмотр анимации
- Настройка FPS (1-60 кадров/сек)

### 💾 Работа с файлами
- Импорт PNG изображений
- Экспорт в PNG
- Сохранение текущего кадра со всеми слоями

### 📐 Адаптивность
- Автоматическое масштабирование под любые разрешения
- Поддержка Full HD, 2K, 4K и ультрашироких мониторов
- Полноэкранный режим (F11)
- Изменяемый размер окна

---

## ⌨️ Горячие клавиши

### 🎨 Инструменты рисования
| Клавиша | Инструмент |
|---------|------------|
| **P** | Карандаш (Pencil) |
| **E** | Ластик (Eraser) |
| **B** | Заливка (Bucket) |
| **L** | Линия (Line) |
| **R** | Прямоугольник (Rectangle) |
| **C** | Круг (Circle) |
| **G** | Градиент (Gradient) |
| **I** | Пипетка (Eyedropper) |
| **T** | Текст (Text) |

### ✂️ Инструменты выделения
| Клавиша | Инструмент |
|---------|------------|
| **S** | Выделение (Selection) |
| **W** | Волшебная палочка (Magic Wand) |
| **M** | Перемещение (Move) |

### 🔧 Управление
| Клавиша | Действие |
|---------|----------|
| **Ctrl+Z** | Отмена (Undo) |
| **Ctrl+Y** | Повтор (Redo) |
| **Ctrl+C** | Копировать |
| **Ctrl+X** | Вырезать |
| **Ctrl+V** | Вставить |
| **Ctrl+S** | Сохранить проект |
| **Ctrl+O** | Открыть проект |
| **Ctrl+N** | Новый проект |
| **Delete** | Удалить выделение |

### 🖥️ Интерфейс
| Клавиша | Действие |
|---------|----------|
| **F1** | Справка по горячим клавишам |
| **F11** | Полноэкранный режим |
| **Alt+F** | Полноэкранный режим (альт.) |
| **Space + Drag** | Панорамирование холста |
| **Mouse Wheel** | Масштабирование (Zoom) |

**💡 Подсказка:** Наведите мышь на любой инструмент для подсказки!

## Использование

### Запуск проекта
1. Откройте проект в Godot Engine 4.5 или новее
2. Откройте сцену `main.tscn`
3. Нажмите F5 для запуска

### Рисование
1. Выберите инструмент из панели слева
2. Выберите цвет с помощью палитры
3. Рисуйте левой кнопкой мыши на холсте

### Работа со слоями
- **+** - добавить новый слой
- **-** - удалить текущий слой
- **↑** - переместить слой вверх
- **↓** - переместить слой вниз
- Кликните на слой в списке для выбора

### Работа с анимацией
- **+** - добавить новый кадр
- **-** - удалить текущий кадр
- **Copy** - дублировать текущий кадр
- **▶** - воспроизвести/остановить анимацию
- Настройте скорость анимации с помощью FPS

### Импорт/Экспорт
- **File → Open PNG** - загрузить PNG изображение
- **File → Save PNG** - сохранить текущий кадр как PNG
- **File → New** - создать новый проект

## Структура проекта

```
edit-pix/
├── main.tscn              # Главная сцена с UI
├── scripts/
│   ├── main.gd            # Основная логика приложения
│   └── drawing_canvas.gd  # Логика рисования и управления слоями/кадрами
└── project.godot          # Конфигурация проекта Godot
```

## Технические детали

### Система слоев
Каждый кадр содержит набор слоев. Слой - это отдельное изображение с поддержкой прозрачности (RGBA8). При отрисовке все видимые слои композитятся сверху вниз.

### Система анимации
Анимация состоит из кадров (AnimationFrame). Каждый кадр содержит свой набор слоев. При воспроизведении кадры переключаются с заданной частотой FPS.

### Инструменты рисования
- **Карандаш/Ластик** - используют алгоритм Брезенхема для рисования плавных линий
- **Заливка** - использует алгоритм flood fill для заполнения замкнутых областей
- **Фигуры** - рисуются с предпросмотром и финализируются при отпускании кнопки мыши

---

## 🚀 Запланированные функции

### Версия 2.3 (Ближайшее будущее)
- **Tile Animation Preview** - просмотр анимированных тайлов
- **Isometric Grid** - изометрические тайлсеты
- **Custom Brushes** - создание пользовательских кистей
- **Dithering Patterns** - библиотека паттернов dithering
- **Dirty Rectangle Optimization** - частичные обновления (5-10x ускорение)

### Версия 2.4 (Среднесрочно)
- **Layer Groups** - организация слоёв в папки
- **Smart Selection** - polygon lasso, magnetic selection
- **Scaling Algorithms** - Scale2x, hqx, xBR для pixel art
- **AI Tools** - upscaling, auto-palette generation
- **Multithreading** - async rendering

### Версия 3.0 (Долгосрочно)
- **2D Rigging System** 🦴 - анимация с костями (IK, weight painting)
- **Plugin System** 🔌 - API для расширений и marketplace
- **Particle Editor** ✨ - визуальный редактор частиц
- **Game Engine Integration** 🎮 - Unity, Unreal, расширенная Godot
- **Retro Palettes** 🕹️ - NES, Game Boy, Genesis, SNES
- **3D Features** 🎲 - voxel conversion, normal maps

### Версия 3.5+ (Будущее)
- **Real-time Collaboration** 👥 - совместная работа как в Figma
- **Cloud & Sync** ☁️ - WebAssembly версия, mobile app
- **Advanced AI** 🧠 - art generation, style transfer
- **Professional Publishing** 📦 - Steam, itch.io integration

**[Полный ROADMAP с 104+ идеями](ROADMAP.md)** | **[Детальный анализ](ROADMAP_EXPANSION.md)**

---

## 📚 Документация

### 🚀 Начало работы
- **[QUICKSTART.md](QUICKSTART.md)** - Быстрый старт за 3 шага
- **[USAGE.md](USAGE.md)** - Подробное руководство пользователя
- **[TUTORIAL.md](TUTORIAL.md)** - Пошаговые туториалы

### 🎨 Функции и возможности
- **[COLOR_PALETTES.md](COLOR_PALETTES.md)** - 31 профессиональная палитра
- **[COMPARISON.md](COMPARISON.md)** - Сравнение с Aseprite (превосходим!)
- **[ADAPTIVE_DISPLAY.md](ADAPTIVE_DISPLAY.md)** - Адаптивность под любые разрешения

### 🏗️ Тайлсеты (v2.1-2.2)
- **[UPDATE_V2.1_TILESETS.md](UPDATE_V2.1_TILESETS.md)** - Полное руководство по тайлсетам
- **[UPDATE_AUTOTILE.md](UPDATE_AUTOTILE.md)** - Auto-Tile System (3×3 bitmask)
- **[UPDATE_COLLISION_EDITOR.md](UPDATE_COLLISION_EDITOR.md)** - Collision Shapes Editor
- **[COLLISION_QUICKREF.md](COLLISION_QUICKREF.md)** - Быстрый справочник по коллизиям

### ⚡ Производительность
- **[PERFORMANCE_OPTIMIZATIONS.md](PERFORMANCE_OPTIMIZATIONS.md)** - Техническая документация (300+ строк)
- **[PERFORMANCE_QUICKREF.md](PERFORMANCE_QUICKREF.md)** - Быстрый справочник по оптимизациям
- **[PERFORMANCE_IMPLEMENTATION.md](PERFORMANCE_IMPLEMENTATION.md)** - Отчёт о реализации

### 🔧 Разработка и архитектура
- **[CONFIGURATION.md](CONFIGURATION.md)** - Настройка и кастомизация
- **[PROJECT_STRUCTURE.md](PROJECT_STRUCTURE.md)** - Архитектура проекта (MVC)
- **[PROJECT_COMPLETE.md](PROJECT_COMPLETE.md)** - Полный обзор возможностей

### �️ Планирование
- **[ROADMAP.md](ROADMAP.md)** - План развития (v2.2 → v3.5+)
- **[ROADMAP_EXPANSION.md](ROADMAP_EXPANSION.md)** - Детальный анализ (104+ идеи)

### ⚖️ Лицензия и информация
- **[LICENSE](LICENSE)** - Проприетарная лицензия с защитой прав
- **[CREDITS.md](CREDITS.md)** - Информация о проекте
- **[BRANDING.md](BRANDING.md)** - История названия и брендинг

## Быстрый старт

```bash
1. Откройте проект в Godot Engine 4.5+
2. Нажмите F5 для запуска (открывается в полный экран)
3. Начните рисовать!
4. F11 - переключить оконный/полноэкранный режим
```

Подробнее см. [QUICKSTART.md](QUICKSTART.md)

## Автор и разработчик

**BitVit (mjojo GLK Dev)**  
Создано с 💙 для пиксель-арт сообщества

## Лицензия и Права

**© 2024-2025 BitVit (mjojo GLK Dev). Все права защищены.**

PIXO распространяется под проприетарной лицензией:
- ✅ **Разрешено**: Личное использование, обучение, создание артов
- ❌ **Запрещено**: Коммерческое использование, распространение, ребрендинг
- 💼 **Коммерческие лицензии**: Свяжитесь с автором

См. [LICENSE](LICENSE) для полных условий.

**ВАЖНО**: Использование PIXO подразумевает согласие с условиями лицензии.

## Благодарности

- **Godot Engine** - за отличный игровой движок
- **Aseprite** - за вдохновение
- Сообщество пиксель-артистов

## Дополнительная информация

- **[CREDITS.md](CREDITS.md)** - Информация о проекте
- **[BRANDING.md](BRANDING.md)** - История переименования

---

## 🎯 Почему PIXO?

### ✨ Превосходит конкурентов
- **vs Aseprite**: Более мощная работа с тайлсетами, auto-tiling, collision editor
- **vs GIMP**: Специализация на pixel art, удобный UI, нет избыточных функций
- **vs Photoshop**: Легковесный, бесплатный, заточен под игровую графику

### 🎮 Для game developers
- ✅ Прямая интеграция с Godot Engine (экспорт .import, .tres)
- ✅ Collision shapes для тайлов (Rectangle, Circle, Polygon)
- ✅ Auto-tiling с bitmask (как в RPG Maker)
- ✅ Sprite sheets с метаданными
- ✅ Анимированные тайлы (v2.3)

### 🎨 Для pixel artists
- ✅ 31 профессиональная палитра (включая retro платформы)
- ✅ Симметричное рисование (Horizontal, Vertical, Quad, Radial)
- ✅ 10 фильтров и эффектов
- ✅ Blend modes для слоёв
- ✅ Onion skinning для анимации

### ⚡ Производительность
- ✅ Оптимизировано для больших холстов (512×512+)
- ✅ Кэширование рендеринга (~100x ускорение на idle)
- ✅ Dirty rectangle tracking (v2.3)
- ✅ GPU acceleration (планируется в v3.0)

### 🆓 Open Development
- ✅ Активная разработка (регулярные обновления)
- ✅ Подробная документация (20+ файлов)
- ✅ Публичный ROADMAP (104+ запланированных функции)
- ✅ Обратная связь с сообществом

---

## �️ Дорожная карта развития

### 🔄 В разработке

**v2.7 - Filter System Refactoring** (Oct-Dec 2025)
- Extract filters into FilterManager class
- Real-time filter preview
- New filters: Edge Detection, Emboss, Noise Reduction
- Target: -400 lines from drawing_canvas.gd

**v2.7.5 - Interactive Tutorial System** (Dec 2025) 🎓
- Interactive tutorial for first-time users
- 10 tutorial steps (Welcome, Tools, Colors, Layers, etc.)
- Highlighted UI elements with progress tracking
- Practice exercises and validation

### 📅 Запланировано (2026)

**v2.8 - Advanced Artistic Tools** (Jan-Mar 2026)
- Liquify & Warp brushes (deformation tools)
- Texture Scatter Brush & Stencil Tool
- FX Brushes (Blur, Sharpen, Dodge/Burn)
- Color Lock Painting

**v2.9 - Automation & AI** (Apr-May 2026)
- Layer Groups & Organization
- Smart Selection Tools (Polygon Lasso, Magnetic, Color Range)
- Pixel Art Scaling (Scale2x, hqx, xBR, Rotsprite)
- AI-Assisted Tools (upscaling, auto-palette, smart fill)

**v2.9.5 - Asset Creation & Marketplace Prep** (May-Jun 2026) 💰
- 📦 **Universal .pxr format** - package brushes, palettes, tilesets, tools
- 🛠️ **Asset Creator Tools:**
  - Asset Packager with validation
  - Brush Designer Pro (advanced parameters)
  - Palette Studio (harmony rules, extraction)
- 💼 **Seller Dashboard:**
  - Upload & publish assets
  - Sales analytics & revenue tracking
  - Payout management (Tokens → $)
- 📚 **Asset Management:**
  - Asset Browser & Collections
  - Auto-Update System
  - Licensing & Light DRM
- 🎨 **Create and sell:**
  - Custom Brushes
  - Color Palettes
  - Tilesets for games
  - Custom Tools & Effect Presets

**v2.10 - Advanced Procedural Tools** (Jul-Sep 2026)
- Color Cycling System (animated palettes)
- Noise Brushes (Perlin/Simplex/Cellular)
- Cellular Automata Generator
- Reference Moodboard Panel

**v2.11 - Generative Tiles & Pro Tools** (Oct-Dec 2026)
- Advanced Auto-Tile (Wang tiles, Corner tiles)
- Procedural Tile Generator
- Tile Atlas Optimizer
- Shader-based effects

### 🚀 Долгосрочные планы (2027+)

**v3.0 - Platform & Marketplace** (Q1-Q2 2027) 💰
- 🔌 **Plugin System** - GDScript plugin API
- 📦 **Universal .pxr Format** - package any asset type
- 🪙 **Token Economy** - buy/sell with PIXO Tokens
- 🛒 **PIXO Asset Store** - integrated marketplace
  - Browse & purchase assets (brushes, palettes, tilesets, tools)
  - Seller dashboard with analytics
  - Revenue sharing (70% creator, 30% PIXO)
  - Categories: Animated Tiles, Tilesets, Sprites, Brushes, Effects
- **Transform PIXO into a platform for creators to earn!**

**v3.5+ - Rigging & Integration** (Q3-Q4 2027)
- 2D Animation & Rigging System
- Mesh deformation & inverse kinematics
- Particle effects system
- Advanced export options

**v4.0+ - Cloud & Collaboration** (2028+)
- Cloud storage & sync
- Real-time collaboration
- Version control integration
- Mobile companion app

**Полная дорожная карта:** [ROADMAP.md](docs/development/roadmaps/ROADMAP.md) (160+ functions planned)

---

## �📊 Статистика проекта

- **Версий выпущено:** 2.6.1 ✅
- **Строк кода:** ~6500+ (GDScript)
- **Функций завершено:** 75+ (v1.0-v2.6.1)
- **Функций запланировано:** 85+ (v2.7-v4.0+)
- **Документации:** 25+ файлов, 6000+ строк
- **Палитр:** 31 профессиональная
- **Фильтров:** 10 эффектов
- **Инструментов:** 14 drawing/selection tools
- **Релизов в 2025:** 6 (v2.0, v2.1, v2.2, v2.3, v2.5, v2.6, v2.6.1)

---

## 🤝 Сообщество и поддержка

### 💬 Обратная связь
Есть идеи или предложения? Добавьте их в [ROADMAP.md](ROADMAP.md) в секцию "Запросы от сообщества"!

### 🐛 Нашли баг?
Сообщите разработчику через GitHub Issues или напрямую.

### 💼 Коммерческое использование?
Свяжитесь с автором для получения коммерческой лицензии.

### ⭐ Понравился PIXO?
- Поставьте звезду на GitHub
- Поделитесь с друзьями-пиксель-артистами
- Станьте создателем контента в v3.0 Marketplace! 💰

---

## 💰 Будущая бизнес-модель (v3.0+)

### Для художников (Creators):
- 🎨 **Создавайте и продавайте** кастомные кисти, палитры, тайлсеты
- 💼 **Зарабатывайте** 70% от продаж (30% комиссия платформы)
- 📊 **Отслеживайте** продажи через встроенную аналитику
- 💸 **Выводите** деньги через Tokens → $ (минимум $10)

### Для покупателей (Users):
- 🛒 **Покупайте** профессиональные ресурсы от сообщества
- ⚡ **Устанавливайте** в один клик
- 🔄 **Обновляйте** автоматически
- 🎨 **Ускоряйте** свой рабочий процесс

### Категории маркетплейса:
- 🌊 Animated Tiles (вода, трава, лава)
- 🗺️ Tilesets (RPG, platformer, dungeon)
- 🧙 Characters & Sprites
- 🎨 Palettes & Color Schemes
- 🖌️ Brushes & Tools
- 🎬 Effects & Shaders

**PIXO станет платформой для монетизации пиксель-арта!**
- Создайте artwork и отметьте #PIXO

---

## 🏆 Благодарности

- **Godot Engine** - за мощный и бесплатный движок
- **Aseprite** - за вдохновение и идеи
- **RPG Maker** - за концепцию auto-tiling
- **Пиксель-арт сообщество** - за поддержку и feedback

---

**PIXO v2.2** by **BitVit (mjojo GLK Dev)**  
© 2024-2025. Все права защищены.  
Создано с 💙 на Godot Engine 4.5

**Лицензия:** Proprietary (Personal Use) | [Детали](LICENSE)  
**Репозиторий:** [GitHub](https://github.com/mjojo/PIXO)  
**Статус:** ✅ v2.0/v2.1 Complete | 🔄 v2.2 In Progress (67%) | 🎯 v2.3-3.5+ Planned
