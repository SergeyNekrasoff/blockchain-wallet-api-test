# Тестовое задание — Blockchain Wallet API

> **Кратко:** нужно заполнить методы в одном файле — [`src/wallet/wallet.service.ts`](src/wallet/wallet.service.ts).
> Весь каркас уже готов: маршруты, провайдеры, Redis, валидация, Swagger — всё подключено и работает.
> Выбираешь любую знакомую тебе сеть, пишешь логику, сдаёшь. Вот и всё.

---

## Быстрый старт

```bash
yarn/pnpm i
cp .env.example .env        # выбрать сеть и вставить ключи (ниже — где их взять)
docker-compose up -d        # поднять Redis
npm run start:dev           # запустить приложение
```

Swagger с документацией всех эндпоинтов: **http://localhost:3000/api**

---

## Готовы

```bash
добавить приватный ключ в .env для ETHERSCAN_API_KEY и выбрать NETWORK=ethereum
Тест: wallet.service.spec.ts -> getBalance метод
```

**GET /wallet/:address/balance**  
**GET /wallet/:address/transactions?limit=5**  
**POST /wallets/watch**  
**GET /wallets/watched**  
**GET /wallets/alerts**  

---

## Сдача

Публичный репозиторий (GitHub / GitLab)