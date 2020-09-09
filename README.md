# vk hatakon hotfix.web

## Доступно по ссылкам:

[https://codesandbox.io/s/priceless-franklin-v6h44](https://codesandbox.io/s/priceless-franklin-v6h44)

[https://v6h44.csb.app/](https://v6h44.csb.app/)

Выполнение третьего задания. Что было сделано:

## 1. Можно создать заказ, не выбрав ни одного блюда.

1. Кнопка оформления заказа на странице ресторана становится активной только после добавления блюда в корзину
2. Если все-так пользователь перешел на страницу корзины, но ничего в корзине нет, то показываем сообщение вместо кнопки оплаты и предлагаем перейти к изменению корзины по кнопке "изменить"
3. Если и после этого пользователю удалось перейти на страницу оплаты, то сообщаем что это невозможно, нужно добавить товары в корзину и предлагаем вернуться на страницу ресторана.

## 2. При указании времени доставки можно ввести всё что угодно.

1. У поля для времени установлен тип "time" таким образом можно ввести только правильное время.

## 3. Цена картофеля фри отличается в меню и при оформлении заказа (правильная цена — 50 рублей).

1. Для данного товара в конфиге задано уникальное имя

## 4. После отмены заказа в консоли приходит статус DONE вместо CANCELED.

1. Название статуса заказа изменено с DONE на CANCELED
2. Для отмены заказа используется функционал "setFinishedOrder". И этот функционал нужен для успешного завершения заказа, его хорошо бы отделить и сделать 3 функции - для изменения статуса на Активный, Отмененный и Завершенный. Но задача именно изменить статус для отмены - я это сделал. Дополнительное изменение кода не стал делать, т.к. это может поломать тесты, если они проверяют результат работы функции setFinishedOrder.

## 5. При изменении состава заказа сбрасываются параметры заказа — время, место и тип («С собой / На месте»).

1. При изменении полей формы я записываю их в localStorage
2. При загрузке страницы записываю сохраненные данные в поля формы.

Контакты: https://telegram.me/jusandi