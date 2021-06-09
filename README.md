# Study Workspace

_Здесь публикуется всё, что связано с изучением frontend_

# [Яндекс](https://yandex-five.vercel.app/)

## Оглавление

1. **HTML**

- [Таблицы](#table)
- [Списки](#lists)
- [Группировка содержимого](#grouping)
  - [\<p\>](#parag)
  - [\<blockquote\>](#blockquote)
  - [\<ol\>](#ol)
  - [\<ul\>](#ul)
  - [\<dl\>](#dl)
  - [\<figure\>](#figure)
  - [\<main\>](#main)
  - [\<div\>](#div)
- [Семантика инлайновых элементов](#seo-inline)
  - [\<a\>](#a)
  - [\<cite\>](#cite)
  - [\<abbr\>](#abbr)
  - [\<time\>](#time)
  - [\<code\>](#code)
  - [\<span\>](#span)
  - [\<br\>](#br)
- [Формы](#forms)
  - [\<form\>](#form)
  - [\<input\>](#input)
  - [\<textarea\>](#textarea)
  - [\<select\>](#select)
  - [\<label\>](#label)
  - [\<button\>](#button)
2. **CSS**
  - [Схлопывание margin](#collapse-margin)
  - [Выпадение вертикальных отступов](#dropping-out-margin)
  - [Блочные и строчные элементы](#blocks-inlines)
  - [Единицы измерения](#units)
    - [px](#px)
    - [em](#em)
    - [%](#percents)
    - [rem](#rem)
---

### &#9776; HTML

#### <a name="table"></a> &#9745; Таблицы

HTML-таблицы (тег `<table></table>`) упорядочивают и выводят на экран данные с помощью строк или столбцов. Таблицы состоят из ячеек, образующихся при пересечении строк и столбцов.

Ячейки таблиц могут содержать любые HTML-элементы, такие как заголовки, списки, текст, изображения, элементы форм, а также другие таблицы. Каждой таблице можно добавить связанный с ней заголовок, расположив его перед таблицей или после неё.

**_Пример:_**

```html
<table>
  <caption>
    Описание
  </caption>
  <tr>
    <th rowspan="3">Молоко</th>
    <th>Производитель</th>
    <th>Цена, руб.</th>
    <th>Объем, мл</th>
  </tr>
  <tr>
    <td>Простоквашино</td>
    <td>50</td>
    <td>950</td>
  </tr>
  <tr>
    <td>Вкуснотеево</td>
    <td>45</td>
    <td>900</td>
  </tr>
</table>
```

**_Результат:_**

<table>
  <caption>Подпись</caption>
  <tr>
    <th rowspan="3">Молоко</th>
    <th>Производитель</th>
    <th>Цена, руб.</th>
    <th>Объем, мл</th>
  </tr>
  <tr>
    <td>Простоквашино</td>
    <td>50</td>
    <td>950</td>
  </tr>
  <tr>
    <td>Вкуснотеево</td>
    <td>45</td>
    <td>900</td>
  </tr>
</table>

---

#### <a name="lists"></a> &#9745; Списки

HTML-списки (теги `<ul></ul>`, `<ol></ol>`, `<dl></dl>`) используются для группировки связанных между собой фрагментов информации.
Каждый список представляет собой контейнер, внутри которого располагаются элементы списка или пары термин-определение.

Элементы списка ведут себя как блочные элементы, располагаясь друг под другом и занимая всю ширину блока-контейнера. Каждый элемент списка имеет дополнительный блок, расположенный сбоку, который не участвует в компоновке.

**_Пример:_**

```html
<ul>
  <li>Машина</li>
  <li>Велосипед</li>
  <li>Самокат</li>
  <li>Самолет</li>
</ul>
```

**_Результат:_**

<ul>
  <li>Машина</li>
  <li>Велосипед</li>
  <li>Самокат</li>
  <li>Самолет</li>
</ul>

---

#### <a name="grouping"></a> &#9745; Групировка содержимого

#### <a name="parag"></a> &#10102; \<p\>

Элемент `<p>` представляет абзац. Абзацы — это блоки текста, физически отделенные от смежных блоков пустыми строками.
Элемент `<p>` не должен использоваться, когда уместен более конкретный элемент.

**_Пример:_**

```html
<p>Это параграф</p>
```

**_Результат:_**

<p>Это параграф</p>

#### <a name="blockquote"></a> &#10103; \<blockquote\>

Элемент `<blockquote>` представляет содержимое, цитируемое из другого источника, необязательно со ссылкой на источник цитирования, которая указывается в элементе `<footer>` или `<cite>`, и, необязательно, с изменениями по тексту, такими как аннотации и сокращения.

**_Пример:_**

```html
<blockquote>
  <p>Легко вставать, когда ты не ложился.</p>
  <cite><i>Джейсон Стейтем</i></cite>
</blockquote>
```

**_Результат:_**

<blockquote>
  <p>Легко вставать, когда ты не ложился.</p>
  <cite><i>Джейсон Стейтем</i></cite>
</blockquote>

#### <a name="ol"></a> &#10104; \<ol\>

Элемент `<ol>` представляет собой список элементов, где элементы были изначально упорядочены таким образом, что изменение порядка изменило бы смысл документа. Элементами списка являются элементы `<li>`.

**_Пример:_**

```html
<ol>
  <li>Первый пункт</li>
  <li>Второй пункт</li>
  <li>Третий пункт</li>
</ol>
```

**_Результат:_**

<ol>
  <li>Первый пункт</li>
  <li>Второй пункт</li>
  <li>Третий пункт</li>
</ol>

#### <a name="ul"></a> &#10105; \<ul\>

Элемент `<ul>` представляет собой список элементов, где порядок элементов не важен, то есть когда изменение порядка не приведет к существенному изменению смысла документа.

**_Пример:_**

```html
<ul>
  <li>Первый пункт</li>
  <li>Второй пункт</li>
  <li>Третий пункт</li>
</ul>
```

**_Результат:_**

<ul>
  <li>Первый пункт</li>
  <li>Второй пункт</li>
  <li>Третий пункт</li>
</ul>

#### <a name="dl"></a> &#10106; \<dl\>

Элемент `<dl>` представляет список описаний, состоящий из нуля или более групп термин-описание. Термин представлен элементом `<dt>`, описание — элементом `<dd>`.

Группы термин-описание могут быть терминами и определениями, вопросами и ответами, категориями и темами и т.п.

**_Пример:_**

```html
<dl>
  <dt>Дисперсия:</dt>
  <dd>
    Мера разброса значений случайной величины относительно её математического
    ожидания
  </dd>
  <dt>Ковариация:</dt>
  <dd>Мера линейной зависимости двух случайных величин</dd>
</dl>
```

**_Результат:_**

<dl>
  <dt>Дисперсия:</dt>
  <dd>Мера разброса значений случайной величины относительно её математического ожидания</dd>
  <dt>Ковариация:</dt>
  <dd>Мера линейной зависимости двух случайных величин</dd>
</dl>

#### <a name="figure"></a> &#10107; \<figure\>

Элемент `<figure>` представляет автономное содержимое (необязательно с подписью), являющееся самостоятельным элементом основного потока. С помощью элемента `<figure>` можно добавлять краткие характеристики к иллюстрациям, фотографиям, диаграммам, фрагментам кода и т.д.

**_Пример:_**

```html
<figure>
  <img src="https://clck.ru/V83Aa" alt="Кот" />
  <figcaption>Вроде кот</figcaption>
</figure>
```

**_Результат:_**

<figure>
  <img src="https://clck.ru/V83DR" alt="Кот"/>
  <figcaption>Вроде кот</figcaption>
</figure>

#### <a name="main"></a> &#10108; \<main\>

Элемент `<main>` включает основное содержимое элемента `<body>` документа или приложения и исключает содержимое, которое повторяется на страницах сайта/приложения, таких как ссылки для навигации по сайту, информация об авторских правах, логотипы сайта и баннеры, а также поисковые формы (за исключением случаев, когда основной функцией документа или приложения является поисковая форма).

Не является секционным содержимым, поэтому не оказывает никакого влияния на структуру документа.

В документе должно быть не более одного элемента `<main>`.

**_Пример:_**

```html
<body>
  <header>
    <nav>
      <ul>
        <li><a href="#">Главная</a></li>
        <li><a href="#">Не главная</a></li>
      </ul>
    </nav>
    <h1>Это моя страничка!</h1>
  </header>
  <main>
    <header>...</header>
    <section>...</section>
    <footer>...</footer>
  </main>
  <footer>
    <adress>Москва, Красная площадь</adress>
  </footer>
</body>
```

#### <a name="div"></a> &#10109; \<div\>

Элемент `<div>` сам по себе ничего не значит. Он представляет свои дочерние элементы. Может использоваться с атрибутами class, lang и title для разметки семантики, общей для группы последовательных элементов.

Рекомендуется использовать элемент `<div>` в случаях, когда другой элемент не подходит. Использование более подходящих элементов вместо элемента `<div>` обеспечивает лучшую доступность для читателей и облегчает обслуживание кода.

**_Пример:_**

```html
<div>
  <p>Первый параграф</p>
  <p>Второй параграф</p>
</div>
```

**_Результат:_**

<div>
  <p>Первый параграф</p>
  <p>Второй параграф</p>
</div>

---

#### <a name="seo-inline"></a> &#9745; Семантика инлайновых элементов

#### <a name="a"></a> &#10102; \<a\>
Если элемент `<a>` имеет атрибут `href`, то он представляет собой гиперссылку (ссылку на другой ресурс, к которому можно перейти или скачать) или якорь (ссылку на идентификатор фрагмента, который является значением в атрибуте `id` элемента в связанном документе).

Элемент `<a>` может быть обернут вокруг целых абзацев, списков, таблиц и т. д., даже целых разделов, при условии, что внутри отсутствует интерактивный контент (например, кнопки или другие ссылки).

___Пример:___

```html
<a href="https://google.com">
    <div>
        <p>Перейти</p>
    </div>
</a>
```

___Результат:___

<a href="https://google.com">
    <div>
        <p>Перейти</p>
    </div>
</a>

#### <a name="cite"></a> &#10103; \<cite\>
Элемент `<cite>` представляет собой ссылку на творческое произведение. Он должен включать название работы или имя автора (человека, людей или организации) или ссылку на URL, или ссылку в сокращенной форме в соответствии с соглашениями, используемыми для добавления метаданных цитирования.

___Пример:___

```html
<blockquote>
    <p>Программирование — это как бить себя по лицу, рано или поздно ваш нос будет кровоточить.</p>
    —<cite>Kyle Woodbury</cite>
</blockquote>
```

___Результат:___

<blockquote>
    <p>Программирование — это как бить себя по лицу, рано или поздно ваш нос будет кровоточить.</p>
    —<cite>Kyle Woodbury</cite>
</blockquote>

#### <a name="abbr"></a> &#10104; \<abbr\>
Элемент `<abbr>` представляет аббревиатуру, необязательно с расшифровкой (в браузере обычно подчеркивается пунктирной линией). Расшифровка аббревиатуры осуществляется с помощью атрибута `title`, она появляется при наведении курсора мыши на текст.

___Пример:___

```html
<abbr title="HyperText Markup Language">HTML</abbr>
```

___Результат:___

<abbr title="HyperText Markup Language">HTML</abbr>


#### <a name="time"></a> &#10105; \<time\>
Элемент `<time>` представляет свое содержимое вместе с машиночитаемой формой этого содержимого в атрибуте `datetime`. Тип содержимого ограничен различными типами дат, времени, смещений часовых поясов и продолжительности. Содержимое элемента `<time>` должно быть валидным значением атрибута `datetime`.
    
___Пример:___

```html
<time>2021-05-27 11:34</time>
```
___Результат:___

<time>2021-05-27 11:34</time>

Если атрибут `datetime` присутствует, то содержимым элемента `<time>` может быть произвольный текст.

___Пример:___

```html
<time datatime="2021-05-27">27 мая 2021 года</time>
```
___Результат:___

<time datatime="2021-05-27">27 мая 2021 года</time>

#### <a name="code"></a> &#10106; \<code\>
Элемент `<code>` представляет собой фрагмент компьютерного кода, содержимое элемента отображается в браузере моноширинным шрифтом.

Не существует формального способа указать язык разметки компьютерного кода. Для подсветки синтаксиса с помощью скрипта можно добавить элементу класс с префиксом `language-`.

___Пример:___

```html
<code>const item = {prop1: 1, prop2: 2}</code>
```

___Результат:___

<code>const item = {prop1: 1, prop2: 2}</code>

#### <a name="span"></a> &#10107; \<span\>
Элемент `<span>` сам по себе ничего не значит, но может быть полезен при использовании вместе с глобальными атрибутами, например, `class`, `lang` или `dir`. Он представляет свои дочерние элементы.

___Пример:___

```html
<span class="some-style">Текст с определенными стилями</span>
```
___Результат:___

<span class="some-style">Текст с определенными стилями</span>

#### <a name="br"></a> &#10108; \<br\>
Элемент `<br>` представляет разрыв строки. Элементы `<br>` должны использоваться только для разрывов строк, которые фактически являются частью содержимого, как в стихах или адресах.

Элементы `<br>` не должны использоваться для разделения тематических групп в абзаце.

___Пример:___

```html
<p>Мои мечты стремятся вдаль,<br>
Где слышны вопли и рыданья,<br>
Чужую разделить печаль<br>
И муки тяжкого страданья.<br>

Я там могу найти себе<br>
Отраду в жизни, упоенье,<br>
И там, наперекор судьбе,<br>
Искать я буду вдохновенья.<br>
</p>
<p>— <cite>Сергей Есенин</cite></p>
```

___Результат:___

<p>Мои мечты стремятся вдаль,<br>
Где слышны вопли и рыданья,<br>
Чужую разделить печаль<br>
И муки тяжкого страданья.<br>

Я там могу найти себе<br>
Отраду в жизни, упоенье,<br>
И там, наперекор судьбе,<br>
Искать я буду вдохновенья.<br>
</p>
<p>— <cite>Сергей Есенин</cite></p>

---

#### <a name="forms"></a> &#9745; Формы

#### <a name="form"></a> &#10102; \<form\>
Основу любой формы составляет элемент `<form>...</form>`. Он не предусматривает ввод данных, так как является контейнером, удерживая вместе все элементы управления формы – поля. Атрибуты этого элемента содержат информацию, общую для всех полей формы, поэтому в одну форму нужно включать поля, объединенные логически.

___Пример:___
```html
<form action="#">
  <label for="enter">Введите что-нибудь</label>
  <input type="text" placeholder="Ввод" name="enter">
  <input type="submit" value="Отправить">
</form>
```

#### <a name="input"></a> &#10103; \<input\>
Элемент `<input>` создает большинство полей формы. Атрибуты элемента отличаются в зависимости от типа поля, для создания которого используется этот элемент.

С помощью css-стилей можно изменить размер шрифта, тип шрифта, цвет и другие свойства текста, а также добавить границы, цвет фона и фоновое изображение. Ширина поля задается свойством `width`.

___Пример:___
```html
<form action="#">
  <input type="text" placeholder="Имя">
  <input type="text" placeholder="Фамилия">
  <input type="tel" placeholder="Телефон">
  <input type="email" placeholder="Телефон">
  <input type="password" placeholder="Телефон">
  <p>Ваш пол:</p>
  <label for="male">Мужской</label>
  <input type="radio" value="мужской" name="male">
  <label for="female">Женский</label>
  <input type="radio" value="женский" name="female">
  <p>День рождения</p>
  <input type="date" name="birthday>
</form>
```

#### <a name="textarea"></a> &#10104; \<textarea\>
Элемент `<textarea>...</textarea>` используется вместо элемента `<input type="text">`, когда нужно создать большие текстовые поля. Текст, отображаемый как исходное значение, помещается внутрь.

Размеры поля устанавливаются при помощи атрибутов `cols` – размеры по горизонтали, `rows` – размеры по вертикали. Высоту поля можно задать свойством `height`. Все размеры считаются исходя из размера одного символа моноширинного шрифта.

___Пример:___
```html
<textarea placeholder="Расскажите немного о себе" cols="20" rows"20"><textarea>
```

#### <a name="select"></a> &#10105; \<select\>
Списки дают возможность расположить большое количество пунктов компактно. Раскрывающиеся списки создаются при помощи элемента `<select>...</select>`. Они позволяют выбрать одно или несколько значений из предложенного множества. По умолчанию в поле списка отображается его первый элемент.

Для добавления в список пунктов используются элементы `<option>...</option>`, которые располагаются внутри `<select>`.

Для систематизации списков применяется элемент `<optgroup>...</optgroup>`, который создает заголовки в списках.

___Пример:___
```html
<select>
  <optgroup label="Цифра">
    <option value="one">Один</option>
    <option value="two">Два</option>
    <option value="three">Три</option>
  </optgroup>
  <optgroup label="Цвет">
    <option value="white">Белый</option>
    <option value="blue">Синий</option>
    <option value="red">Красный</option>
  </optgroup>
</select>
```

#### <a name="label"></a> &#10106; \<label\>
Надписи к элементам формы создаются с помощью элемента `<label>...</label>`. Существует два способа группировки надписи и поля. Если поле находится внутри элемента `<label>`, то атрибут `for` указывать не нужно.

___Пример:___
```html
<label for="field">Имя</label>
<input type="text" name="field" placeholder="Введите имя" />

<label>Имя<input type="text" placeholder="Введите имя" /></label>
```

#### <a name="button"></a> &#10107; \<button\>
Элемент `<button>...</button>` создает кликабельные кнопки. В отличие от кнопок, созданных `<input>`, внутрь элемента `<button>` можно поместить контент — текст или изображение.

Для корректного отображения элемента `<button>` разными браузерами нужно указывать атрибут `type`, например, `<button type="submit"></button>`.
  
___Пример:___
```html
<button type="submit">Отправить заявку<button>
```

---

### &#9776; CSS

#### <a name="collapse-margin"></a> &#9745; Схлопывание margin
Смежные вертикальные отступы двух или более элементов уровня блока `margin` объединяются (перекрываются). При этом ширина общего отступа равна ширине большего из исходных. Исключение составляют отступы корневого элемента, которые не схлопываются.

___Пример:___
```html
<div class="block1">margin-bottom 30px</div>
<div class="block2">margin-top 30px</div>
```
```css
.block1 {
  width: 150px;
  height: 150px;
  background-color: red;
  margin-bottom: 30px;
}

.block2 {
  width: 150px;
  height: 150px;
  background-color: green;
  margin-top: 30px;
}
```

___Результат:___
[Схлопывание вертикальных margin](https://codepen.io/g0dez/pen/QWpaQNK)

---

#### <a name="dropping-out-margin"></a> &#9745; Выпадение вертикальных отступов
Если внутри одного блока расположить другой блок и задать ему `margin-top`, то внутренний блок прижмется к верхнему краю родительского, а у родительского элемента появится отступ сверху, т.е. внутренний блок «выпадет» из родительского блока. Если у родительского элемента также был задан верхний отступ, то выберется наибольшее из значений.

Чтобы избавиться от эффекта выпадения, можно задать родительскому элементу `padding-top` или добавить `border-top: 1px solid transparent`.

___Пример:___
```html
<div class="block1">
  <div class="block2"></div>
</div>

```
```css
.block1 {
  border-top: 1px solid transparent;
  width: 150px;
  height: 150px;
  background-color: red;
}

.block2 {
  margin-top: 20px;
  width: 100px;
  height: 100px;
  background-color: green;
}
```

___Результат:___
[Выпадение вертикальных отступов](https://codepen.io/g0dez/pen/xxqpYZz)

---

#### <a name="blocks-inlines"></a> &#9745; Строчные и блочные элементы

___Пример:___
```html
<body>
  <header class="header">
    <nav>
      <ul>
        <li>1</li>
        <li>2</li>
        <li>3</li>
      </ul>
     </nav>
  </header>
  
  <main class="main">
    <article class="article">
      <header><h2>TItle</h2></header>
      <p><span class="red">T</span>ext</p>
      <footer><time datatime="2021-05-27">27 мая 2021 года</time></footer>
    </article>
  </main>
  
  <footer class="footer"><adress>Moscow, Pushkino</adress></footer>
</body>
```

```css
ul {
  list-style: none;
  margin: 0;
}

h2 {
  margin: 0;  
}

.header {
  background-color: green;
}

.main {
  background-color: yellow;
}

.article {
  text-align: center;
  margin: 0 auto;
  width: 500px;
  background-color: blue;
  color: #fff;
}

.footer {
  background-color: red;
  text-align: center;
}

.red {
  color: red;
}
```

___Результат:___
[Блочные и строчные элементы](https://codepen.io/g0dez/pen/VwpyQjR)

---

#### <a name="units"></a> &#9745; Единицы измерения

#### <a name="px"></a> &#10102; Пиксели: px
Пиксель `px` – это самая базовая, абсолютная и окончательная единица измерения.

Количество пикселей задаётся в настройках разрешения экрана, один `px` – это как раз один такой пиксель на экране. Все значения браузер в итоге пересчитает в пиксели.

___Пример:___
```html
<p style="font-size: 20px;">
  <a style="font-size: 20px">Ссылка</a>
</p>
```

#### <a name="em"></a> &#10103; Относительно шрифта: em
`1em` – текущий размер шрифта.

Можно брать любые пропорции от текущего шрифта: `2em`, `0.5em` и т.п.

Размеры в `em` – относительные, они определяются по текущему контексту.

___Пример:___
```html
<p style="font-size: 1.5em;">
  <a style="font-size: 1.5em">Ссылка</a>
</p>
```

#### <a name="percents"></a> &#10104; Проценты: %
Проценты `%`, как и `em` – относительные единицы.

Когда мы говорим «процент», то возникает вопрос – «Процент от чего?»

Как правило, процент будет от значения свойства родителя с тем же названием, но не всегда.

___Пример:___
```html
<p style="font-size: 250%;">
  <a style="font-size: 250%">Ссылка</a>
</p>
```

#### <a name="rem"></a> &#10105; Единица rem: смесь px и em
Единица rem задаёт размер относительно размера шрифта элемента `<html>`.

Как правило, браузеры ставят этому элементу некоторый «разумный» (reasonable) размер по умолчанию, который мы, конечно, можем переопределить и использовать `rem` для задания шрифтов внутри относительно него.

Элементы, размер которых задан в `rem`, не зависят друг от друга и от контекста – и этим похожи на `px`, а с другой стороны они все заданы относительно размера шрифта `<html>`.

___Пример:___
```html
<p style="font-size: 1rem;>
  <a style="font-size: 1.5rem">Ссылка</a>
</p>
```
```css
html {
  font-size: 14px;
}
```

