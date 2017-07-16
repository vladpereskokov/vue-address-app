##  Приложение поиска адреса с автодополнением

## Приложение развернуто на Heroku (настроен автодеплой из Travis CI)
Работающее приложение на [Heroku](https://vue-address-app.herokuapp.com)

#### Технологии
- TypeScript для написания логики,
- Sass для стилей,
- Webpack для сборки,
- [Vuejs](http://vuejs.org/v2/guide/) фреймворк для компонентной разработки
- [vue-class-component](https://github.com/vuejs/vue-class-component) для наилучшей интеграции vuejs и typescript.

#### Разработка и запуск
- `npm install`,
- `npm start` - запуск сервера разработки, результат будет доступен по адресу [http://localhost:3200](http://localhost:3200)

#### Компоненты
Приложение имеет компонентную структуру, входной точкой является `src/app/components/app.component`, он содержит в себе дочерние компоненты и запускается в файле `src/main.ts`.

#### Библиотека (сервис) адресов
В файле `app/lib/index.ts`, есть сервис `addresses`, которому можно передать введенный пользователем токен и получить промис адреса.


### Задача
- ~~Отслеживать пользовательский ввод в инпут и выводить адрес полученный на основе токена в компоненте результатов поиска~~,
- ~~Отправлять запрос в сервис адресов, если пользовательский ввод (токен) больше 3х символов~~,
- ~~Между отправкой токена в сервис адресов и получением результата показывать индикатор загрузки в компоненте индикатора загрузки~~,
- ~~Отправлять запрос в сервис адресов, только после 1380 милисекунд бездействия пользователя~~,
- ~~Отправлять запрос, только если токен изменился относительно предыдущего токена~~.

