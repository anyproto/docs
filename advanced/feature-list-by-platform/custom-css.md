# Custom CSS

Original shared by [LavaC](https://community.anytype.io/u/LavaC) on our community forum:

{% embed url="https://community.anytype.io/t/tutorial-of-custom-css/14234" %}

For assistance with this CSS guide or CSS in general, please comment in the original topic linked above.

### Where <a href="#where-1" id="where-1"></a>

To enable the Custom CSS style sheet, go to `Menu > File > Apply Custom CSS`.

<figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

To edit the custom CSS file, go to `Menu > File > Open > Custom CSS`.

<figure><img src="../../.gitbook/assets/image (4) (1).png" alt="" width="375"><figcaption></figcaption></figure>

### How <a href="#how-2" id="how-2"></a>

In order to take into beginners, many methods in this article are not best practices. If you understand CSS, you can likely skip most of the contents.

#### Theme color <a href="#theme-color-3" id="theme-color-3"></a>

When developing software, styles variables are usually set first as a baseline. Anytype is the same. If you want to change to your own style, generally start from here.

These variables are usually under the `:root` selector, we can see these in Dev tools.

<figure><img src="https://community-static.anytype.io/optimized/2X/8/8c798a22e6bddd7bd190043a2ec7c226fcf5cf24_2_690x408.png" alt=""><figcaption></figcaption></figure>

For example, `--color-text-primary` seems to be the color variable for the darkest black text, so we can write it this way in the custom.css file:

<figure><img src="https://community-static.anytype.io/original/2X/b/bbefbe5a417032384cde12b1e80e4b2f480ded68.png" alt=""><figcaption></figcaption></figure>

After saving, you can refresh Anytype by pressing `(Command/Ctrl) + r`.

> Of course, you can also directly modify and view the effects in Dev tools.

At this point, we can see that the red I just wrote overrode the default value, so my text has all turned red.

<figure><img src="https://community-static.anytype.io/optimized/2X/0/0e16feda708cfeee241bc7128caa3f802a09c66d_2_690x384.png" alt=""><figcaption></figcaption></figure>

Below is part of the custom.css I modified referring to [Solarized 18](https://en.wikipedia.org/wiki/Solarized), which is actually like a word filling game, change these variables more to see where they take effect, and then you’ll know what to modify next.

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

#### Fonts <a href="#fonts-4" id="fonts-4"></a>

The attribute related to fonts in CSS is called [font-family 3](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family). In order to ensure that all text applies the same font, we generally put the styles on the `body` tag.

```css
body {
    font-family: "霞鹜文楷", "jetBrainsMono";
}
```

Of course, the premise for it to take effect is that you have this font on your computer, if not, you can install this font on your computer or choose to import the font online.

{% hint style="info" %}

{% endhint %}

<details>

<summary>Import font online</summary>

[<img src="https://community-static.anytype.io/optimized/2X/d/d1348ecf28fafeb4c079d5cd9ba343b30ee6f9d2_2_690x494.png" alt="image" data-size="original">](https://community-static.anytype.io/original/2X/d/d1348ecf28fafeb4c079d5cd9ba343b30ee6f9d2.png)\
[![image](https://community-static.anytype.io/optimized/2X/a/aaf23f71f95b30839021c2489a9153cc46f2b8be_2_690x271.png)](https://community-static.anytype.io/original/2X/a/aaf23f71f95b30839021c2489a9153cc46f2b8be.png)\
[![image](https://community-static.anytype.io/optimized/2X/d/d29da78fce6ac4d052c0b030fd322fab4fef2a1a_2_690x458.png)](https://community-static.anytype.io/original/2X/d/d29da78fce6ac4d052c0b030fd322fab4fef2a1a.png)\
[![image](https://community-static.anytype.io/optimized/2X/8/87c8c15932c29ee8bd91d58928d2958209db39e3_2_690x107.png)](https://community-static.anytype.io/original/2X/8/87c8c15932c29ee8bd91d58928d2958209db39e3.png)\
[![image](https://community-static.anytype.io/optimized/2X/6/690391b23293397bb0844789dee9d500300a3028_2_690x435.png)](https://community-static.anytype.io/original/2X/6/690391b23293397bb0844789dee9d500300a3028.png)

</details>

#### Dark Mode <a href="#dark-mode-5" id="dark-mode-5"></a>

The styles in dark mode need to be wrapped within the `html.themeDark`.

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

#### Other elements <a href="#other-elements-6" id="other-elements-6"></a>

If you want to modify a particular element, you can use the Dev tools function in the upper left corner, and then select the element you want to modify, at which time you can see the styles related to it in the **Styles** column.

<figure><img src="https://community-static.anytype.io/optimized/2X/3/3d111c1232f10345c8584f5a2cf15ec36cba8864_2_690x460.png" alt=""><figcaption></figcaption></figure>

You can try directly modifying the values inside to see what effects it would produce.

<figure><img src="https://community-static.anytype.io/optimized/2X/6/6ec5d48153fd5abfd34274a2c9cfb736de865a14_2_690x283.png" alt=""><figcaption></figcaption></figure>

If you think the effects are not bad, you can copy all this content to your custom.css stylesheet to save.

<figure><img src="https://community-static.anytype.io/original/2X/8/8c83f1c7406a1a651cac26da10c6429bd59f2dcb.png" alt=""><figcaption></figcaption></figure>

#### Change Icons <a href="#change-icons-7" id="change-icons-7"></a>

The icons in Anytype are implemented using SVG.

<details>

<summary>For example the relation icons</summary>

[<img src="https://community-static.anytype.io/optimized/2X/6/6d596177b0b332db51cd793630c415891538f8f7_2_672x500.png" alt="image" data-size="original">](https://community-static.anytype.io/original/2X/6/6d596177b0b332db51cd793630c415891538f8f7.png)

The text starting with `data:image/svg...` is the Base64 data converted from SVG.\
You can decrypt this data on a dedicated [website 1](https://base64.guru/converter/decode/image/svg) to get the SVG image.

</details>

If you want to customize your own icon, you can convert SVG to Base64 format, which can be achieved on a dedicated [website](https://base64.guru/converter/encode/image/svg).

As for the source of SVG icons, I recommend using this [website 4](https://pictogrammers.com/libraries/).

> It is best not to choose SVG that is too complicated, otherwise the resulting Base64 text will be too long.

After obtaining the corresponding Base64 text and replacing it, we have successfully replaced it.

```css
.header .icon.relation {
  background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvb......);
}
```

![image](https://community-static.anytype.io/original/2X/3/30b788e54c7daa2db54352ca4ff721ecc6d2e027.png)

**If you think the original icon is very good and just want to change the color, there is also a way to achieve it, but it will be a bit complicated.**

```css
.header .icon.relation {
  // The content of the url in the next line is the content of the `background-image` attribute of this icon. 
  mask-image: url(data:image/svg+xml;base64,.......);
  mask-repeat: no-repeat;
  background: red; // the color you want
}
```

If you have used PS, you should be able to guess that this is a similar mask function, but unfortunately the final result is not very smooth.\


<figure><img src="https://community-static.anytype.io/original/2X/7/72dbdcf71ef643f5873aa7ea1ea814bf282dfec5.png" alt=""><figcaption></figcaption></figure>

### Examples

{% embed url="https://community.anytype.io/t/anytype-mist-light-dark-a-brand-new-anytype-theme/16329" %}
