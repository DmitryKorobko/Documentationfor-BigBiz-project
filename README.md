# REST API для мобильного приложения

## API v1
* Модуль "Authorization"
    * Методы
        * [Регистрация пользователя](api/v1/authorization/registration.POST.md)
        * [Авторизация пользователя(логин)](api/v1/authorization/login.POST.md)
        * [Авторизация пользователя как гость(логин)](api/v1/authorization/login-guest.POST.md)
        * [Logout](api/v1/authorization/logout.GET.md)
        * [Восстановление пароля](api/v1/authorization/password-recovery.POST.md)
        * [Отправка уникального кода для восстановления пароля](api/v1/authorization/send-security-code.POST.md)
        * [Метод генерации нового access_token на основе refresh_token](api/v1/authorization/generation-access-token.POST.md)
      
* Модуль "User"
    * Методы
        * [Получить профиль пользователя](api/v1/user/profile/profile.GET.md)
        * [Обновить профиль](api/v1/user/profile/profile.PUT.md)
        * [Удалить профиль](api/v1/user/profile/profile.DELETE.md) 
        * [Общий список избранных тем и товаров](api/v1/user/common-list-favorites.GET.md)        
        * [Регистрация девайса в системе](api/v1/user/device/device.POST.md)
        * [Метод бокового меню пользователя](api/v1/user/profile/side-menu.GET.md)
        * [Список ответов для пользователя](api/v1/user/profile/answers.GET.md)
        * [Список собственных тем пользователя](api/v1/user/theme/list.GET.md)
        * [Метод добавления собственной темы пользователем](api/v1/user/theme/add.POST.md)
        * [Метод изменения собственной темы пользователем](api/v1/user/theme/edit.PUT.md)
        * [Метод удаления собственной темы](api/v1/user/theme/delete.DELETE.md)
        * [Метод получения настроек профиля пользователя](api/v1/user/profile/settings.GET.md)
        * [Метод удаления собственного профиля пользователя](api/v1/user/profile/profile.DELETE.md)
        * [Метод изменения собственной аватарки пользователем](api/v1/user/profile/avatar.PUT.md)  
        * [Метод добавление репутации пользователю](api/v1/user/add-user-reputation.POST.md)  
        * [Изменение пароля](api/v1/user/profile/change-password.POST.md)
        * [Изменение онлайн статуса пользователя](api/v1/user/change-status-online.GET.md)

* Модуль "Shop"
    * Методы
        * [Список магазинов](api/v1/shop/shops.GET.md)
        * [Детальная информация о своём магазине](api/v1/shop/profile.GET.md)
        * [Краткая информация о магазине с темами и товарами](api/v1/shop/preview.GET.md)
        * [Подробная информация рейтинга магазина](api/v1/shop/rating.GET.md)
        * [Список отзывов о магазине](api/v1/shop/reviews.GET.md)
        * [Метод добавления отзыва о магазине](api/v1/shop/add-shop-review.POST.md)
        * [Метод изменения отзыва о магазине](api/v1/shop/update-shop-review.PUT.md)
        * [Детальная информация об отзыве конкретного пользователя](api/v1/shop/review-detail.GET.md)
        * [Список ответов для магазина](api/v1/shop/answers.GET.md)
        * [Метод бокового меню магазина](api/v1/shop/side-menu.GET.md)
        * [Детальная информация о магазине](api/v1/shop/detail.GET.md)
           
* Модуль "Product"
    * Методы
        * [Список продуктов в избранном](api/v1/product/list-favorites.GET.md)
        * [Детальная информация о продукте](api/v1/product/detail.GET.md) 
        * [Добавление продукта в избранное](api/v1/product/add-favorite.POST.md)
        * [Удаление продукта из избранного](api/v1/product/delete-favorite.DELETE.md) 
        * [Список отзывов о товаре](api/v1/product/list-feedbacks.GET.md)
        * [Метод добавления отзыва о товаре](api/v1/product/add-review.POST.md)
        * [Метод обновления отзыва о товаре](api/v1/product/update-review.PUT.md)
        * [Лайк товара](api/v1/product/like.POST.md) 
        * [Список товаров магазина](api/v1/product/shop-products.GET.md) 
        
* Модуль "Theme"
    * Методы
        * [Список тем категорий второго уровня](api/v1/theme/list.GET.md)  
        * [Детальная информация о теме](api/v1/theme/detail.GET.md) 
        * [Like или Dislike темы](api/v1/theme/like-dislike.POST.md)  
        * [Список тем магазина](api/v1/theme/shop-themes.GET.md)  
        * [Добавление темы в избранное](api/v1/theme/add-theme-in-favorites.POST.md)
        * [Удаление темы из избранного](api/v1/theme/delete-theme-from-favorites.DELETE.md) 
        * [Список тем в избранном](api/v1/theme/list-favorites.GET.md) 
        
* Модуль "Content"
    * Методы
        * [Список категорий первого уровня](api/v1/content/category/main.GET.md)
        * [Список категорий второго уровня](api/v1/content/category/child.GET.md)
        * [Список городов](api/v1/content/city.GET.md) 
        * [Список активных баннеров](api/v1/content/banner/list.GET.md)
 
* AWS
    * Методы
        * [Формирования ссылки для загрузки картинки на AWS S3](api/v1/aws/generate-presigned-url.POST.md)
        
* Модуль "Comment"
    * Методы
        * [Обновление комментария](api/v1/comment/update.PUT.md)
		* [Удаление комментария](api/v1/comment/delete.DELETE.md)
		* [Добавление комментария](api/v1/comment/create.POST.md) 
        * [Список комментариев темы](api/v1/comment/list.GET.md)
        * [Like комментария](api/v1/comment/like.POST.md)

* Модуль "Support"
    * Методы
        * [Отправка письма в поддержку](api/v1/support/send-support-email.POST.md)

* Модуль "Message"
    * Методы
        * [Список чатов](api/v1/message/list-chats.GET.md)
        * [Отправление личного сообщения](api/v1/message/create.POST.md)
        * [Изменение сообщения](api/v1/message/update.PUT.md)
        * [Удаление сообщения](api/v1/message/delete.DELETE.md)
        * [История конкретного чата](api/v1/message/chat-history.GET.md)
        * [Настройка таймера очищения истории](api/v1/message/cleaning-chat.POST.md)
        * [Удаление истории сообщений с конкретным пользователем](api/v1/message/delete-chat.DELETE.md)



                
