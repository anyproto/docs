# Руководство по пользовательским CSS

Оригинал предоставлен [LavaC](https://community.anytype.io/u/LavaC) на нашем форуме сообщества:

{% embed url="https://community.anytype.io/t/tutorial-of-custom-css/14234" %}

Если вам понадобится помощь по этому руководству CSS или по CSS в целом, вы можете оставить комментарий в оригинальной теме.
### Где <a href="#where-1" id="where-1"></a>

Чтобы использовать пользовательский CSS, вам нужно сначала перейти в рабочую директорию Anytype.

<figure><img src="https://community-static.anytype.io/original/2X/c/cefa762c4537031b75bc43f2bc387e35fe36911b.jpeg" alt=""><figcaption></figcaption></figure>

Затем создайте файл под названием custom.css в этой директории.

<figure><img src="https://community-static.anytype.io/optimized/2X/c/cbe263ff498e9700dca9f07e4c730f667042b556_2_690x401.jpeg" alt=""><figcaption></figcaption></figure>
### Как <a href="#how-2" id="how-2"></a>

Чтобы учесть новичков, многие методы в этой статье не являются лучшими практиками. Если вы понимаете CSS, можете пропустить большую часть содержимого.

#### Цветовая тема <a href="#theme-color-3" id="theme-color-3"></a>

При разработке программного обеспечения стили обычно задаются через переменные, установленные в качестве базовых. В Anytype это так же. Если вы хотите изменить стили под себя, начните с этого.

Эти переменные обычно находятся под селектором `:root`, их можно увидеть в Dev Tools.

<figure><img src="https://community-static.anytype.io/optimized/2X/8/8c798a22e6bddd7bd190043a2ec7c226fcf5cf24_2_690x408.png" alt=""><figcaption></figcaption></figure>

Например, `--color-text-primary` кажется переменной для самого тёмного чёрного текста, поэтому мы можем написать его в файле custom.css следующим образом:

<figure><img src="https://community-static.anytype.io/original/2X/b/bbefbe5a417032384cde12b1e80e4b2f480ded68.png" alt=""><figcaption></figcaption></figure>

После сохранения вы можете обновить Anytype, нажав `(Command/Ctrl) + r`.

> Конечно, вы также можете напрямую изменить и просмотреть эффекты в Dev Tools.

На этом этапе мы можем увидеть, что красный цвет, который я только что написал, переопределил значение по умолчанию, поэтому весь мой текст стал красным.

<figure><img src="https://community-static.anytype.io/optimized/2X/0/0e16feda708cfeee241bc7128caa3f802a09c66d_2_690x384.png" alt=""><figcaption></figcaption></figure>

Ниже приведена часть custom.css, которую я изменил, ссылаясь на [Solarized 18](https://en.wikipedia.org/wiki/Solarized). Это похоже на игру с изменением слов: меняйте переменные, чтобы увидеть, где они вступают в силу, и затем вы узнаете, что изменить дальше.

<figure><img src="https://community-static.anytype.io/optimized/2X/0/0a67ca485d41ba2d1e72dd5b30b5cae7f489f82e_2_690x394.jpeg" alt=""><figcaption></figcaption></figure>

```css
:root {
    --color-text-primary: #002b36;
    --color-text-secondary:	#586e75;
    --color-text-tertiary: 	#839496;
    --color-text-inversion: #eee8d5;
    --color-shape-primary: 	#586e75;
    --color-shape-secondary: 	#eee8d5;
    --color-shape-tertiary: 	#eee8d5;
    --color-shape-highlight-medium: rgba(79, 79, 79, 0.08);
    --color-shape-highlight-light: rgba(79, 79, 79, 0.04);
    --color-control-accent: #252525;
    --color-control-active: #b6b6b6;
    --color-control-inactive: #dcdcdc;
    --color-control-bg: #fff;
    --color-bg-primary: #fdf6e3;
    --color-bg-loader: rgba(255,255,255,0.7);
    --color-system-accent-100: #ffb522;
    --color-system-accent-50: #ffd15b;
    --color-system-accent-25: #ffee94;
    --color-system-selection: rgba(24, 163, 241, 0.15);
    --color-system-drop-zone: rgba(255, 187, 44, 0.25);
    --color-yellow: #ecd91b;
    --color-orange: #ffb522;
    --color-red: #f55522;
    --color-pink: #e51ca0;
    --color-purple: #ab50cc;
    --color-blue: #3e58eb;
    --color-ice: #2aa7ee;
    --color-teal: #0fc8ba;
    --color-lime: #5dd400;
    --color-green: #66B395;
}
```

#### Шрифты <a href="#fonts-4" id="fonts-4"></a>

Атрибут, связанный со шрифтами в CSS, называется [font-family](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family). Чтобы все тексты отображались с одним шрифтом, мы обычно применяем стили к тегу `body`.

```css
body {
    font-family: "霞鹜文楷", "jetBrainsMono";
}
```

Конечно, для того чтобы это сработало, шрифт должен быть установлен на вашем компьютере. Если его нет, вы можете установить его или импортировать шрифт из интернета.

{% hint style="info" %}

{% endhint %}

<details>

<summary>Импортировать шрифт онлайн</summary>

[<img src="https://community-static.anytype.io/optimized/2X/d/d1348ecf28fafeb4c079d5cd9ba343b30ee6f9d2_2_690x494.png" alt="image" data-size="original">](https://community-static.anytype.io/original/2X/d/d1348ecf28fafeb4c079d5cd9ba343b30ee6f9d2.png)\
[![image](https://community-static.anytype.io/optimized/2X/a/aaf23f71f95b30839021c2489a9153cc46f2b8be\_2\_690x271.png)](https://community-static.anytype.io/original/2X/a/aaf23f71f95b30839021c2489a9153cc46f2b8be.png)\
[![image](https://community-static.anytype.io/optimized/2X/d/d29da78fce6ac4d052c0b030fd322fab4fef2a1a\_2\_690x458.png)](https://community-static.anytype.io/original/2X/d/d29da78fce6ac4d052c0b030fd322fab4fef2a1a.png)\
[![image](https://community-static.anytype.io/optimized/2X/8/87c8c15932c29ee8bd91d58928d2958209db39e3\_2\_690x107.png)](https://community-static.anytype.io/original/2X/8/87c8c15932c29ee8bd91d58928d2958209db39e3.png)\
[![image](https://community-static.anytype.io/optimized/2X/6/690391b23293397bb0844789dee9d500300a3028\_2\_690x435.png)](https://community-static.anytype.io/original/2X/6/690391b23293397bb0844789dee9d500300a3028.png)

</details>

#### Тёмный режим <a href="#dark-mode-5" id="dark-mode-5"></a>

Стили для тёмного режима нужно обернуть в `html.themeDark`.

```css
/* Default applies to light mode */
.blocks {
    .block.blockText.textCallout>.wrapContent{
        border-radius: 30px;
    }
}

html.themeDark {
    /* Applies to Dark mode */
    --color-text-primary: red;
    .blocks {
        .block.blockText.textCallout>.wrapContent{
            border-radius: 2px;
        }
    }
}

```

#### Другие элементы <a href="#other-elements-6" id="other-elements-6"></a>

Если вы хотите изменить определённый элемент, вы можете использовать функцию Dev Tools в верхнем левом углу, затем выбрать элемент, который хотите изменить, и увидеть связанные с ним стили в колонке **Styles**.

<figure><img src="https://community-static.anytype.io/optimized/2X/3/3d111c1232f10345c8584f5a2cf15ec36cba8864_2_690x460.png" alt=""><figcaption></figcaption></figure>

Вы можете попробовать изменить значения прямо там, чтобы увидеть, какие эффекты это вызовет.

<figure><img src="https://community-static.anytype.io/optimized/2X/6/6ec5d48153fd5abfd34274a2c9cfb736de865a14_2_690x283.png" alt=""><figcaption></figcaption></figure>

Если эффекты вам понравились, вы можете скопировать всё это содержимое в свой файл custom.css, чтобы сохранить изменения.

<figure><img src="https://community-static.anytype.io/original/2X/8/8c83f1c7406a1a651cac26da10c6429bd59f2dcb.png" alt=""><figcaption></figcaption></figure>

#### Замена иконок <a href="#change-icons-7" id="change-icons-7"></a>

Иконки в Anytype реализованы с помощью SVG.

<details>

<summary>Например, иконки отношений</summary>

[<img src="https://community-static.anytype.io/optimized/2X/6/6d596177b0b332db51cd793630c415891538f8f7_2_672x500.png" alt="image" data-size="original">](https://community-static.anytype.io/original/2X/6/6d596177b0b332db51cd793630c415891538f8f7.png)

Текст, начинающийся с `data:image/svg...`, — это данные Base64, преобразованные из SVG.\
Вы можете расшифровать эти данные на специальном [веб-сайте](https://base64.guru/converter/decode/image/svg), чтобы получить SVG изображение.

</details>

Если вы хотите настроить собственную иконку, вы можете преобразовать SVG в формат Base64, что можно сделать на специальном [веб-сайте](https://base64.guru/converter/encode/image/svg).

Что касается источников SVG-иконок, я рекомендую использовать этот [веб-сайт](https://pictogrammers.com/libraries/).

> Лучше не выбирать слишком сложные SVG, иначе текст Base64 будет слишком длинным.

После получения соответствующего текста Base64 и его замены, мы успешно изменили иконку.

```css
.header .icon.relation {
  background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvb......);
}
```

![image](https://community-static.anytype.io/original/2X/3/30b788e54c7daa2db54352ca4ff721ecc6d2e027.png)

**Если вам нравится оригинальная иконка, но вы хотите просто изменить её цвет, это также возможно, хотя и немного сложно.**

```css
.header .icon.relation {
  // The content of the url in the next line is the content of the `background-image` attribute of this icon. 
  mask-image: url(data:image/svg+xml;base64,.......);
  mask-repeat: no-repeat;
  background: red; // the color you want
}
```

Если вы использовали Photoshop, вы, вероятно, догадаетесь, что это аналогичная функция маски. Однако, к сожалению, конечный результат не будет очень гладким.

<figure><img src="https://community-static.anytype.io/original/2X/7/72dbdcf71ef643f5873aa7ea1ea814bf282dfec5.png" alt=""><figcaption></figcaption></figure>

### Примеры

{% embed url="https://community.anytype.io/t/anytype-mist-light-dark-a-brand-new-anytype-theme/16329" %}
