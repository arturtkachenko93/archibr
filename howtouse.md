<!-- !С правами администратора! -->

1) npm i
2) npm install webp-converter@2.2.3 --save-dev
3) gulp

Переустановка node-sass
npm rebuild node-sass

Проблема с pyton
npm install --global windows-build-tools

<!-- !Работа с ТАБАМИ -->

@@include("_tabs-block.html")
_tabs - задать контейнеру
_tabs-item - для добавления на каждый ТАБ
_tabs-block - для добавления на каждый блок ТАБА

<!-- !Работа со SPOLLERS -->

@@include("_spollers.html")
_spollers - задать контейнеру
_spoller - задать кнопке
_one - для добавления эффекта "аккордеона" (все спойлеры будут закрыты, кроме одного)

<!-- !Работа с FORM -->

@@include("_form.html")
_req - задать inputу для валидации формы
_email - задать inputy для валидации email
Для подключения масок необходимо в js/vendors.js подключить libs/inputmask.min.js
 - для input добавить _digital - ввод только цифр;
 - для input добавить _phone - валидация ввода телефона;
 - для input добавить _date - появление календарика (предварительно подключить js/vendor.js --> datepicker-full.min.js)

data-ajax="true" - для отправки формы (задать самой forme)
js/vendors.js подключить libs/nouislider.js, wNumb.min.js - для ползунка RANGE

<!-- !Работа со SLIDER -->

_swiper - задать контейнеру для построения структуры слайдера
js/vendors.js --> @@include('libs/swiper.min.js', {}) - для подключения js
js/app.js @@include('files/sliders.js', {}) подключать по-выше
js/files/slider.js - настройки слайдера.

<!-- !Работа с POPUP -->

_popup-link - задать нужной ссылке
href="#callback" - любой POPUP
href="#video" - для видео (only YOUTUBE!)

<!-- !Работа с GALLERY -->

js/vendors.js --> @@include('libs/lightgallery.min.js', {}) - для подключения js
_gallery - задать контейнеру для построения структуры gallery

<!-- !Работа со SCROLL -->

_src-item - добавить любому блоку для активации анимации при скролле
scroll - добавить анимацию при скролле. Теперь при появлении блок плавно отображается

для ссылки добавить _goto и href="#название_блока" - плавная прокрутка страницы к нужному блоку

_goto-block - добавляется класс .active ссылке в навигации, когда находимся в данном блоке href="#название_блока".

для подсказок при наведении - добавить js/vendors.js --> @@include('libs/tippy.js', {}) ==> добавить .tippy нужному элементу для появления подсказки
