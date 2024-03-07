# Техническое задание

## Продуктовый помощник "Hell chicken".

---

## Сводное HTTP API

Система должна представлять следующие HTTP-хендлеры:

- `GET /api/users` - список пользователей
- `POST /api/users` - регистрация пользователя
- `GET /api/users/{user_id}` - профиль пользователя
- `GET /api/users/me` - текущий пользователь
- `POST /api/users/set_password` - изменение пароля
- `POST /api/token/login` - получить токен авторизации
- `POST /api/token/logout` - удаление токена авторизации

- `GET /api/tags` - список тегов
- `GET /api/tags/{tag_id}` - получение тега
- `POST /api/tags` - создание тега
- `PATCH /api/tags/{tag_id}` - изменение тега
- `DELETE /api/tags/{tag_id}` - удаление тега

- `GET /api/recipes` - список рецептов
- `POST /api/recipes` - создание рецепта
- `GET /api/recipes/{recipe_id}` - получение рецепта
- `PATCH /api/recipes/{recipe_id}` - обновление рецепта
- `DELETE /api/recipes/{recipe_id}` - удаление рецепта

- `GET /api/recipes/download_shopping_cart` - скачать список покупок
- `POST /api/recipes/{recipe_id}/favorite` - добавить рецепт в избранное
- `POST /api/recipes/{recipe_id}/shopping_cart` - добавить рецепт в список покупок
- `DELETE /api/recipes/{recipe_id}/favorite` - удалить рецепт из избранного
- `DELETE /api/recipes/{recipe_id}/shopping_cart` - удалить рецепт из списка покупок

- `GET /api/users/subscriptions` - мои подписки
- `POST /api/users/{user_id}/subscribe` - подписаться на пользователя
- `DELETE /api/users/{user_id}/subscribe` - отписаться от пользователя

- `GET /api/ingredients` - список ингредиентов
- `POST /api/ingredients` - создание ингредиента
- `GET /api/ingredients/{ingredient_id}` - получение ингредиента
- `PATCH /api/ingredients/{ingredient_id}` - обновление ингредиента
- `DELETE /api/ingredients/{ingredients_id}` - удаление ингредиента
