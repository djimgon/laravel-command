# sql удаление пользователей кроме админа
DELETE FROM users WHERE id <> 1;

# запуск php кода в консоли
php artisan tinker

# создания моделей, но без их сохранения в базе данных используя tinker
$users = User::factory()->count(3)->make();

# Генерация фабрик
php artisan make:factory PostFactory --model=Post

# автоматическое добавление данных в таблицы Laravel
