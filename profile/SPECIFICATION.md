# Техническое задание

## Продуктовый помощник "Hell chicken".

---

## Сводное HTTP API

Система должна представлять следующие HTTP-хендлеры:

- `GET /api/users` - [список пользователей](#список-пользователей)
- `POST /api/users` - [регистрация пользователя](#регистрация-пользователя)
- `GET /api/users/{user_id}` - [профиль пользователя](#профиль-пользователя)
- `GET /api/users/me` - [текущий пользователь](#текущий-пользователь)
- `POST /api/users/set_password` - [изменение пароля](#изменение-пароля)
- `POST /api/token/login` - [получить токен авторизации](#получить-токен-авторизации)
- `POST /api/token/logout` - [удаление токена авторизации](#удаление-токена-авторизации)

- `GET /api/tags` - [список тегов](#список-тегов)
- `GET /api/tags/{tag_id}` - [получение тега](#получение-тега)
- `POST /api/tags` - [создание тега](#создание-тега)
- `PATCH /api/tags/{tag_id}` - [изменение тега](#изменение-тега)
- `DELETE /api/tags/{tag_id}` - [удаление тега](#удаление-тега)

- `GET /api/recipes` - [список рецептов](#список-рецептов)
- `POST /api/recipes` - [создание рецепта](#создание-рецепта)
- `GET /api/recipes/{recipe_id}` - [получение рецепта](#получение-рецепта)
- `PATCH /api/recipes/{recipe_id}` - [обновление рецепта](#обновление-рецепта)
- `DELETE /api/recipes/{recipe_id}` - [удаление рецепта](#удаление-рецепта)

- `GET /api/recipes/download_shopping_cart` - [скачать список покупок](#скачать-список-покупок)
- `POST /api/recipes/{recipe_id}/favorite` - [добавить рецепт в избранное](#добавить-рецепт-в-избранное)
- `POST /api/recipes/{recipe_id}/shopping_cart` - [добавить рецепт в список покупок](#добавить-рецепт-в-список-покупок)
- `DELETE /api/recipes/{recipe_id}/favorite` - [удалить рецепт из избранного](#удалить-рецепт-из-избранного)
- `DELETE /api/recipes/{recipe_id}/shopping_cart` - [удалить рецепт из списка покупок](#удалить-рецепт-из-списка-покупок)

- `GET /api/users/subscriptions` - [мои подписки](#мои-подписки)
- `POST /api/users/{user_id}/subscribe` - [подписаться на пользователя](#подписаться-на-пользователя)
- `DELETE /api/users/{user_id}/subscribe` - [отписаться от пользователя](#отписаться-от-пользователя)

- `GET /api/ingredients` - [список ингредиентов](#список-ингредиентов)
- `POST /api/ingredients` - [создание ингредиента](#создание-ингредиента)
- `GET /api/ingredients/{ingredient_id}` - [получение ингредиента](#получение-ингредиента)
- `PATCH /api/ingredients/{ingredient_id}` - [обновление ингредиента](#обновление-ингредиента)
- `DELETE /api/ingredients/{ingredients_id}` - [удаление ингредиента](#удаление-ингредиента)

### Список пользователей

Хендлер: `GET /api/users`

### Регистрация пользователя

Хендлер: `POST /api/users`

### Профиль пользователя

Хендлер: `GET /api/users/{user_id}`

### Текущий пользователь

Хендлер: `GET /api/users/me`

### Изменение пароля

Хендлер: `POST /api/users/set_password`

### Получить токен авторизации

Хендлер: `POST /api/token/login`

### Удаление токена авторизации

Хендлер: `POST /api/token/logout`

### Список тегов

Хендлер: `GET /api/tags`

### Получение тега

Хендлер: `GET /api/tags/{tag_id}`

### Создание тега

Хендлер: `POST /api/tags`

### Изменение тега

Хендлер: `PATCH /api/tags/{tag_id}`

### Удаление тега

Хендлер: `DELETE /api/tags/{tag_id}`

### Список рецептов

Хендлер: `GET /api/recipes`

### Создание рецепта

Хендлер: `POST /api/recipes`

### Получение рецепта

Хендлер: `GET /api/recipes/{recipe_id}`

### Обновление рецепта

Хендлер: `PATCH /api/recipes/{recipe_id}`

### Удаление рецепта

Хендлер: `DELETE /api/recipes/{recipe_id}`

### Скачать список покупок

Хендлер: `GET /api/recipes/download_shopping_cart`

### Добавить рецепт в избранное

Хендлер: `POST /api/recipes/{recipe_id}/favorite`

### Добавить рецепт в список покупок

Хендлер: `POST /api/recipes/{recipe_id}/shopping_cart`

### Удалить рецепт из избранного

Хендлер: `DELETE /api/recipes/{recipe_id}/favorite`

### Удалить рецепт из списка покупок

Хендлер: `DELETE /api/recipes/{recipe_id}/shopping_cart`

### Мои подписки

Хендлер: `GET /api/users/subscriptions`

### Подписаться на пользователя

Хендлер: `POST /api/users/{user_id}/subscribe`

### Отписаться от пользователя

Хендлер: `DELETE /api/users/{user_id}/subscribe`

### Список ингредиентов

Хендлер: `GET /api/ingredients`

### Создание ингредиента

Хендлер: `POST /api/ingredients`

### Получение ингредиента

Хендлер: `GET /api/ingredients/{ingredient_id}`

### Обновление ингредиента

Хендлер: `PATCH /api/ingredients/{ingredient_id}`

### Удаление ингредиента

Хендлер: `DELETE /api/ingredients/{ingredients_id}`