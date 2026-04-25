# 🐳 Ура 12: Анализ логов в Docker
> «У меня работает» → «Работает везде»

## 🎯 Цель
Упаковать скрипт `analysis.py` в контейнер, чтобы он запускался одной командой на любом компьютере (Ubuntu, Windows, Mac).

## 📦 Что внутри
- `Dockerfile` – рецепт образа
- `docker-compose.yml` – кнопка «запустить всё»
- `analysis.py` – ваш код анализа
- `verify.sh` – самопроверка

У нас теперь всё в одном месте: и игра, и анализ.

### Шаг 1: Получаем данные (Локально)
Сначала нужно поиграть, чтобы получить лог. Запускайте игру на своем компьютере (не в Docker!):
```bash
python3 game.py

## 🛠 Подготовка (1 раз)
1. Установите Docker:
   - Ubuntu: `sudo apt update && sudo apt install docker.io docker-compose-plugin`
   - Windows/Mac: [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Проверьте установку:
   ```bash
   docker --version
   docker compose version
