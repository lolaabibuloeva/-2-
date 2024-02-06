<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="utf-8" />
<title>Код блочного сайта</title>

/* Стилевое оформление */
<style> body{   background:#c0c0c0; /* Меняется фон экрана, выбирается здесь */ }
#wrapper{ /* Оболочка страницы сайта */   width: 900px; /* Меняется ширина страницы */   margin: 0 auto;   background:#f2e8c9; /* Меняется задний фон страницы */ }
/* Шапка сайта */
#header{ position:relative; /* Задаём блоку относительное позиционирование для того, чтобы затем размещать, в нём другие элементы и позиционировать относительно его границ поверх фоновой картинки и заголовка */   height: 250px; /* Высота шапки */   background-color: #ffffff; /* Фон шапки */    margin-bottom: 5px; /* Нижний отступ шапки от остального контента */   border-radius: 5px; /* Закругляются углы блока */   box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Тень. Визуально приподнимает блок над оболочкой */ } img{ /* Фоновая картинка в шапке */ float: left; /* Разрешаем наплывание других элементов на картинку */   margin: -40px 0 0 0;} /* Размещаем картинку в блоке header. 1-я и 3-я цифры - двигаем вверх-вниз, 2-я и 4-я цифры - двигаем вправо-влево */ h1{ /* Заголовок сайта */   margin:0 0 10px 40px; /* Заголовок двигается верх-вправо-вниз-влево. */   color:#464451; /* Цвет заголовка */ } .nomer{ /*Подзаголовок (номер телефона)*/   position:absolute; /* Позиционируем абсолютно подзаголовок, относительно границ блока header. Также можно разместить в шапке сайта ещё другие картинки и абзацы поверх фоновой картинки и заголовка */   top:5px; /* Двигается вверх-вниз */   left:680px; /* Двигается вправо-влево */   font-size: 25px; /* Размер букв подзаголовка */   font-style:italic; /* Курсив */   font-weight:bold; /* Жирный */   color:#464451; /* Цвет букв подзаголовка */ }
/* Сайдбар (колонка справа) */
#sidebar{ /* Блок сайдбара */   background-color: #ffffff; /* Фон блока */   width: 180px; /* Ширина блока */   padding: 10px; /* Отступ текста от краёв */   float: right; /* Размещаем блок справа от других элементов, наплывание или обтекание справа). Если делать сайдбар слева, то значение right меняем на left */   border-radius: 5px; /* Закругляем углы блока */   box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Задаём блоку тень */ } .marcer{ /* Галочки маркеры меню */   float: left; /* Размещаем слева от текста */   margin: 5px 5px 0 0; /* Двигаются вверх-вправо-вниз-влево */ }
/* Контент (статья) */
#content{ /* Блок контента */   margin-bottom: 5px; /* Отступ блока статьи от блока подвала */   width: 676px; /* Ширина статьи */   padding: 10px; /* Отступ текста от краёв блока */   background: #ffffff; /* Фон статьи */   border-radius: 5px;   box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; } .left{ /* Картинка в тексте слева */   float: left;   margin: 30px 7px 7px 7px; } .right{ /* Картинка в тексте справа */   float: right;   margin: 7px 0 7px 7px; } /* Подвал */
#footer{ /* Блок подвала */   height:80px; /* Высота блока подвала */   background-color: #ffffff; /* Фон блока подвала */   margin-bottom: 10px; /* Отступ снизу */   border-radius: 5px; /* Закруглённые углы */   box-shadow: rgba(0,0,0,0.5) 0px 1px 3px; /* Тень блока */ } .clear{ /* Запрет наплывания. Устанавливается для того, чтобы блок контента, при заполнении текстом и изображениями не наплывал на подвал */   clear: both; }   .fon{ /* Номер телефона */   float:left; /* Разрешаем другим элементам обтекать абзац справа */   margin:20px 0 0 20px; } .fax{ /* Номер факса */   float:left;   margin:20px 0 0 60px; } .mail{ /* Адрес E-mail */   float:left;  margin:20px 0 0 60px; } </style> </head> <body>   <div id="wrapper"> <!--Оболочка страницы--> <!--Шапка сайта-->     <div id="header"> <!--Заголовок сайта-->       <h1>Грузоперевозки</h1> <!--Описание (телефон)-->         <p class="nomer">234-49-50 <br> +7 900 650 33 45</p> <!--Фоновая картинка в шапке сайта-->       <img src="http://trueimages.ru/img/cf/26/9116df15.png">     </div> <!--Сайдбар-->     <div id="sidebar"> <!--меню-->       <h3>На нашем сайте</h3> <!--Картинки маркеров меню (галочки)-->         <p><img class="marcer" src="http://trueimages.ru/img/99/91/dea39f15.png" width="10" height="10">Наши сотрудники</p>         <p><img class="marcer" src="http://trueimages.ru/img/99/91/dea39f15.png" width="10" height="10">Наша техника</p>         <p><img class="marcer" src="http://trueimages.ru/img/99/91/dea39f15.png" width="10" height="10">Прайс</p> <!--Прямая синяя линия-->           <hr width="50" color="#037FFC" size="5"> <!--Общая информация в сайдбаре-->       <h3>Другая информация</h3>     </div> <!--Основной контент (статья)-->     <div id="content"> <!--Картинка слева-->       <img class="left" src="http://trueimages.ru/img/81/90/b1718f15.png"> <!--Заголовок статьи-->         <h3>Наша работа</h3> <!--Текст статьи--> <p>Здравствуйте уважаемые будущие веб-мастера!</p> <p>Мне 55 лет и я рад приветствовать Вас на своём сайте. Этот сайт первый, который я разработал самостоятельно, а до этого умел только входить в интернет. Почему я решил его сделать?</p> <p>За те 3 месяца, пока разбирался в сайтостроении и создавал этот ресурс обнаружилось, что авторы руководств по созданию сайтов считают многие нюансы само собой разумеющимися и не обращают на них внимание.</p> <p>А мне, учитывая возраст и «опыт», было не просто понять как раз эти нюансы, они отнимали больше всего времени. И я решил написать свой материал, так что-бы другим было легче сориентироваться в потоке новой информации.</p> <!--Картинка справа-->       <img class="right" src="http://trueimages.ru/img/0d/64/07a18f15.png">
<p>Здесь «разжеваны» все мелочи сопровождающие создание сайта, мимо которых обычно проскакивают другие авторы. Если вам что-то будет непонятно, спрашивайте, для меня нет «глупых» вопросов. Читайе и создавайте свой сайт самостоятельно, каким бы ни был Ваш возраст и стаж работы на компьютере.</p> <p>Уверен, у Вас получится еще лучше и уж точно, в несколько раз быстрее, чем у меня.</p>     </div> <!--Запрет наплывания-->   <div class="clear"></div> <!--Подвал-->     <div id="footer">       <p class="fon"><strong>Телефон:<br> 265-48-76</strong> </p>       <p class="fax"><strong>Факс:<br> 265-85-97</strong></p>       <p class="mail"><strong>E-mail<br>ctoto@mail.ru</strong></p>
    </div>   </div> </body> </html>
