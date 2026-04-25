# 🐳 Ура 12: Анализ логов в Docker
> «У меня работает» → «Работает везде»

## 🎯 Цель
Упаковать скрипт `analysis.py` в контейнер, чтобы он запускался одной командой на любом компьютере (Ubuntu, Windows, Mac).

## 📦 Что внутри
- `Dockerfile` – рецепт образа
- `docker-compose.yml` – кнопка «запустить всё»
- `analysis.py` – ваш код анализа
- `verify.sh` – самопроверка

## 🛠 Подготовка (1 раз)
1. Установите Docker:
   - Ubuntu: `sudo apt update && sudo apt install docker.io docker-compose-plugin`
   - Windows/Mac: [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Проверьте установку:
   ```bash
   docker --version
   docker compose version
