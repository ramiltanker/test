# Научиться учиться
Проект даёт возможность узнать современные и эффективные способы обучения такие как:
1. Техники обучения.
2. Видео нa TED.
3. Метод Фейнмана.
4. Цифры и факты.
5. Книга.
6. Принципы обучения.
7. Полезные ресурсы.

## Технологи, которые использовались в проекте
В проекте использован flex-box, чтобы разместить блоки так как нужно.
```css
//css
.table {
  margin: auto;
  width: 1100px;
  min-height: 200px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding-left: 0;
}
```
В проете использованы заголовки разных уровней
```html
<h1 class="header__title">Научиться учиться</h1>
<h2 class="section-title">Техники обучения</h2>
<h3 class="cards__title">Два вида внимания</h3>
```
Также присутствуют изображения фоновые(background-image) и с тегом <img>
```html
<img src="./images/cards-recall.png" alt="Рикол" class="cards__image">
```
```css
.kaufman__triangle {
  position: absolute;
  width: 877px;
  height: 877px;
  z-index: -5;
  background-image: url("../../../images/kaufman-triangle.svg");
  background-size: contain;
  top: 0;
  right: -210px;
}
```
Использована анимация
```css
@keyframes square {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

.rotation {
  animation: square 20s linear infinite;
}
```
На страницу вставленны два видео благодаре iframe
```html
<iframe class="video__iframe" src="https://www.youtube.com/embed/5MgBikgcWnY" ></iframe>
<iframe class="video__iframe" src="https://www.youtube.com/embed/arj7oStGLkU" ></iframe>
```
Были использованы плавные переходы для ссылок
```css
.header__link {
  text-decoration: none;
  opacity: 1;
  color: #2f80ed;
}

.header__link:hover {
  text-decoration: underline;
  opacity: 0.5;
  transition-property: opacity;
  transition-duration: 1s;
  transition-timing-function: linear;
  transition-delay: 0.5;
}
```
### Планы по доработке проекта
Дабавить анимацию к другим элементам с помощью animation, transition, transform, keyframes.
Добавить форму в проект используя imput. 
