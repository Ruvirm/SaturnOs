### <img src="/icon/logOs.png" alt="icon" width="256">



## Содержание
1. [Введение](#введение)  
2. [Планы](#Планы)  
3. [Цели](#Цели)
4. [Структура](#Структура)
5. [Контакты](#Контакты) 


## Введение:
### logOs

Простая операционная система с собственным ядром. 

---

### **Планы:**
- [ ] Создать первую версию ядра.
- [ ] Реализовать простую оболочку.
- [ ] Разработать API для работы с системой.
- [ ] Подготовить документацию для пользователей.

### **Цели:**
- Максимальная простота использования.
- Изменение принципов программирования.
- Классический дизайн в стиле Windows 95.
- Поддержка приложений Windows NT.
- Гибкая и удобная настройка системы.
- Наличие драйверов "из коробки".
- Богатый набор стандартных приложений.

---
## **Структура:**
### Это структура, к которой стремится ядро.
```
project/
├── boot/                   # Загрузчик (bootloader)
│   ├── boot.s              # Ассемблерный код для запуска ядра
│   └── loader.c            # Инициализация начальных структур
├── kernel/                 # Основное ядро
│   ├── arch/               # Аппаратно-зависимый код
│   │   ├── x86/
│   │   │   ├── idt.c       # Таблица прерываний
│   │   │   ├── gdt.c       # Таблица сегментов
│   │   │   ├── io.c        # Ввод/вывод
│   │   │   └── isr.c       # Обработчики прерываний
│   ├── memory/             # Управление памятью
│   │   ├── paging.c        # Страницы памяти
│   │   ├── heap.c          # Менеджер кучи
│   │   └── memmap.c        # Карта памяти
│   ├── scheduler/          # Управление процессами
│   │   ├── task.c          # Задачи и потоки
│   │   ├── timer.c         # Таймеры
│   │   └── context.c       # Сохранение/восстановление контекста
│   ├── drivers/            # Драйверы
│   │   ├── keyboard.c      # Драйвер клавиатуры
│   │   ├── screen.c        # Драйвер экрана
│   │   ├── disk.c          # Драйвер диска
│   │   └── pci.c           # Работа с PCI
│   ├── fs/                 # Файловая система
│   │   ├── vfs.c           # Виртуальная файловая система
│   │   └── fat.c           # Пример реализации FAT
│   ├── net/                # Сетевой стек
│   │   ├── tcp.c           # TCP протокол
│   │   ├── udp.c           # UDP протокол
│   │   └── ip.c            # IP протокол
│   ├── syscall/            # Системные вызовы
│   │   ├── syscall.c       # Реализация вызовов
│   │   └── table.c         # Таблица вызовов
│   └── main.c              # Основная точка входа
├── modules/                # Модули ядра
│   ├── module_loader.c     # Загрузчик модулей
│   └── example_module.c    # Пример модуля
├── lib/                    # Утилиты и вспомогательные функции
│   ├── string.c            # Работа со строками
│   ├── math.c              # Математические операции
│   └── list.c              # Реализация связного списка
└── include/                # Заголовочные файлы
    ├── kernel.h            # Основные объявления ядра
    ├── memory.h            # Интерфейсы памяти
    ├── scheduler.h         # Интерфейсы процессов
    ├── drivers.h           # Интерфейсы драйверов
    └── syscall.h           # Системные вызовы
```    
---
## Контакты
Если у вас есть вопросы свяжитесь с нами по адресу: [ссылка](https://t.me/YaroPe1).
