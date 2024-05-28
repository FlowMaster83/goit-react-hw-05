Навігація в додатку

У застосунку обов'язково повинні бути наступні маршрути.

'/' – компонент HomePage, домашня сторінка із списком популярних кінофільмів.
'/movies' – компонент MoviesPage, сторінка пошуку кінофільмів за ключовим словом.
'/movies/:movieId' – компонент MovieDetailsPage, сторінка із детальною інформацією про кінофільм.
/movies/:movieId/cast – компонент MovieCast, інформація про акторський склад. Рендериться в нижній частині на сторінці MovieDetailsPage.
/movies/:movieId/reviews – компонент MovieReviews, інформація про огляди. Рендериться в нижній частині на сторінці MovieDetailsPage.
Якщо користувач зайшов за неіснуючим маршрутом, потрібно показувати компонент NotFoundPage, в якому є посилання Link на домашню сторінку.

Файли компонентів сторінок, таких як HomePage, MoviesPage, MovieDetailsPage, NotFoundPage, повинні бути в папці src/pages.
Компоненти MovieCast і MovieReviews не є окремими сторінками, вони є лише частинами сторінки MovieDetailsPage, тому файли цих компонентів зберігаємо в src/components.
Меню з навігаційними посиланнями перенесіть в компонент Navigation. Він складається з двох компонентів NavLink, які вказують на маршрути / і /movies.
Для відображення списку фільмів створіть компонент MovieList. Використовуйте його на сторінках HomePage і MoviesPage.



API key: 5475dbe28db4c8eaecd1f756d8383814

Access: eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiI1NDc1ZGJlMjhkYjRjOGVhZWNkMWY3NTZkODM4MzgxNCIsInN1YiI6IjY2NTYxNDhiNTJiMzNhOTNmYWEzZTZmMiIsInNjb3BlcyI6WyJhcGlfcmVhZCJdLCJ2ZXJzaW9uIjoxfQ.hxMkPjIMt6HUgE5WFgTgr_o4yZ5AOUL4rqSA4L0B5gE