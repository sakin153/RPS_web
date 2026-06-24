# ✊ Камень-Ножницы-Бумага

> Игра с компьютером через веб-камеру на основе ONNX-модели

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen?style=for-the-badge)](https://sakin153.github.io/RPS_web/)
---

## 📦 Структура проекта

```
.
├── index.html          # Основной файл — веб-интерфейс игры
├── train.ipynb         # Jupyter Notebook — обучение модели
├── best.onnx           # Экспортированная ONNX-модель
└── README.md           # Этот файл
```

---

## 🚀 Быстрый старт

1. Откройте `index.html` в современном браузере
2. Разрешите доступ к камере
3. Нажмите **«Начать игру»** и покажите жест ✊🖐️✌️

**Или попробуйте онлайн:**  
👉 [https://sakin153.github.io/RPS_web/](https://sakin153.github.io/RPS_web/)

---

## 🧠 Обучение модели

- Файл: `train.ipynb`
- Датасет: [Rock-Paper-Scissors Images](https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors)
- Архитектура: **YOLOv8n** (Nano)
- Экспорт: → `best.onnx` (оптимизирована для веба)
- Размер входа: `640×640` пикселей

---

## 🎮 Как играть

| Жест | Эмодзи | Побеждает |
|------|--------|-----------|
| Камень | ✊ | Ножницы |
| Ножницы | ✌️ | Бумагу |
| Бумага | 🖐️ | Камень |

1. Встаньте перед камерой
2. Покажите жест — модель распознаёт его в реальном времени
3. За 5 кадров определяется ваш выбор
4. Компьютер делает случайный ход — результат мгновенно!

---

## 🛠️ Технологии

| Компонент | Технология |
|-----------|------------|
| Модель | YOLOv8 → ONNX |
| Инференс | ONNX Runtime Web |
| Интерфейс | Vanilla JS + Tailwind CSS |
| Камера | WebRTC `getUserMedia` |
| Звук | Web Audio API |

---

**Автор:** [@sakin153](https://github.com/sakin153)  
**Проект:** [github.com/sakin153/RPS_web](https://github.com/sakin153/RPS_web)
