Это сайт рецептов на Django.

Сайт доступен по ссылке https://cookbook-gb.onrender.com/

Сайт задеплоин на render.com. Если вы перейдете по ссылку, то не увидите картинок рецептов. Но если вы добавите свой рецепт, его картитнка отобразится. Как я понял, это происходит, потому что render не поддерживает постоянный доступ, а начинает каждый раз заного деплоить сайт из их образа, когда кто-то переходит по ссылке.

И каждый новый раз он это делает на другом компьютере, где нет старых медиа файлов, так как они сохраняются в базовою дерикторию на старом компьютере. Render предоставляет внешнее храниеще медеа-файлов, но оно платное. Как это сделать бесплатно, чтобы не пришлось писать собственный сервис, я не нашел.

Используя фреймворк Django создайн сайт, на котором пользователи смогут
добавлять свои рецепты блюд и просматривать рецепты других пользователей, оставлять комментарии и вступать в чат с создателем рецепта.


Модели
Для работы с пользователями использован встроенный в Django User`a.
Подготовлены нижеперечисленные модели:

● Рецепты:

  ○ Название

  ○ Описание

  ○ Шаги приготовления

  ○ Время приготовления

  ○ Изображение

  ○ Автор

  ○ ингредиенты

● Категории рецептов

○ Название

● Связующая таблица для связи Рецептов и Категории

Шаблоны

Подготовлены базовый шаблон проекта и нижеперечисленные дочерние шаблоны:

● Главная с 5 последними добавленными рецептами

● При на клике на рецепт открывается страница с подробным описанием рецептом

● Страницы регистрации, авторизации и выхода пользователя

● Страница добавления/редактирования рецепта

Формы

Созданы формы для ввода и редактирования рецептов и интегрированны в шаблоны.

Представления

Созданы представления, которые охватывают весь проект: модели, формы,
шаблоны.

Маршруты

Подключены маршруты.
