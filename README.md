# test_log_pass_classificator
Файлы приложения находятся в папке app.
Controller - flask приложение , запускает веб-сервер с страницей авторизации (localhost:5000). Записывает полученные временные данные в файл data.
Classificator_app - использует данные из файла data для обучения и использования классификатора пары логин/пароль на поведение, свойственное хозяину пары.
Использует для классификации логистическую регрессию. Для обучения используются первые 15 семплов , для теста следующие 3 (можно откорретировать в коде)

У Classificator app есть GUI. Для того чтобы посмотроить графики - кнока build graphs, после этого можно возспользоваться классификатором при помощи кнопки check. Данные для графиков и классификации беруться из файла data. Чтобы использовать новые значения необходимо удалить все значения в файле data.
