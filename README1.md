##12. TEXT

The properties that allow you to control the appearance of text can be split into two groups:

* Those that directly affect the font and its appearance (including the typeface, whether it is regular, bold or italic, and the size of the text)
* Those that would have the same effect on text no matter what font you were using (including the color of text and the spacing between words and letters)

###TYPEFACE TERMINOLOGY

####SERIF
Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.

In print, serif fonts were traditionally used for long passages of text because they were considered easier to read.

![](imgs/ch12 - serif.jpg)

####SANS-SERIF
Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

Screens have a lower resolution than print. So, if the text is small, sans-serif fonts can be clearer to read.

![](imgs/ch12 - sans-serif.jpg)

####MONOSPACE
Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

![](imgs/ch12 - monospace.jpg)

Monospace fonts are commonly used for code because they align nicely, making the text easier to follow.

![](imgs/ch12 - specifications.jpg)

####WEIGHT
The font weight not only adds **emphasis** but can also affect the amount of **white space** and **contrast** on a page.

![](imgs/ch12 - weight.jpg)

####STYLE
**Italic** fonts have a cursive aspect to some of the lettering. **Oblique** font styles take the normal style and put it on an angle.

![](imgs/ch12 - style.jpg)

####STRETCH
In condensed (or narrow) versions of the font, letters are thinner and closer together. In expanded versions they are thicker and further apart.

![](imgs/ch12 - stretch.jpg)

###CHOOSING A TYPEFACE FOR YOUR WEBSITE

####SERIF
Serif fonts have extra details on the end of the main strokes of the letters.

EXAMPLES:
* Georgia
* Times
* Times New Roman

####SANS-SERIF
Sans-serif fonts have straight ends to letters and therefore have a much cleaner design.

EXAMPLES:
* Arial
* Verdana
* Helvetica

It is possible to specify more than one typeface and create an order of preference (in case the user does not have your first choice of typeface installed). This is sometimes referred to as a font stack.

####MONOSPACE
Every letter in a monospace typeface is the same width. (Non-monospace fonts have different widths.)

EXAMPLES:

![](imgs/ch12 - monospace examples.jpg)

####CURSIVE
Cursive fonts either have joining strokes or other cursive characteristics, such as handwriting styles.

EXAMPLES:

![](imgs/ch12 - cursive examples.jpg)

####FANTASY
Fantasy fonts are usually decorative fonts and are often used for titles. They're not designed for long bodies of text.

EXAMPLES:

![](imgs/ch12 - fantasy examples.jpg)

Browsers are supposed to support at least one typeface from each of the groups above. For this reason, it is common to add the generic font name after your preferred choice of typefaces.

For example, if you wanted serif type, you could write the following:

```font-family: Georgia, Times, serif;```

###TECHNIQUES THAT OFFER A WIDER CHOICE OF TYPEFACES

There are several ways to use fonts other than those listed on the previous page. However, typefaces are subject to copyright, so the techniques you can choose from are limited by their respective licenses.

![](imgs/ch12 - choice of typefaces.jpg)

---

![](imgs/ch12 - choice of typefaces1.jpg)

###SPECIFYING TYPEFACES

**```font-family```**

The ```font-family``` property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

The people who are visiting your site need the typeface you have specified installed on their computer in order for it to be displayed.

You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list.

It is also common to end with a generic font name for that type of font.

If a font name is made up of **more than one word**, it should be put in **double quotes**.

Designers suggest pages usually look better if they **use no more than three typefaces on a page**.

![](imgs/ch12 - font family.jpg)
![](imgs/ch12 - font family result.jpg)

###SIZE OF TYPE

**```font-size```**

![](imgs/ch12 - font size.jpg)
![](imgs/ch12 - font size result.jpg)

The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:

**PIXELS**

Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px.

**PERCENTAGES**

The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.
If you create a rule to make all text inside the ```<body>``` element to be 75% of the default size (to make it 12px), and then specify another rule that indicates the content of an element inside the ```<body>``` element should be 75% size, it will be 9px (75% of the 12px font size).

**EMS**

An em is equivalent to the width of a letter **```m```**.

####TYPE SCALES

You may have noticed that programs such as Word, Photoshop and InDesign offer the same sizes of text.

This is because they are set according to a scale or ratio that was developed by European typographers in the sixteenth century.
It is considered that this scale for type is pleasing to the eye and it has therefore changed little in the last 400 years.

For this reason, when you are designing pages, using sizes from this scale will help them look more attractive.

On the next page, you can see how to achieve this scale using pixels, percentages, and ems.

Print designers often refer to the size of text in terms of points rather than pixels (hence the use of pt in the scale on the right). A pixel roughly equates to a point because a point corresponds to 1/72 of an inch, and most computer displays have a resolution of 72 dots per inch.

The default size of text in a browser is 16 pixels. So if you use percentages or ems, you calculate the size of text you want based on the default size of the text used in browsers. For example, you could scale down to 12 pixels for body copy and scale up to 24 pixels for headings.

Recently, some web designers have started to leave the body text at the default size of 16 pixels and adjust the other font sizes using a scale that keeps the relative proportions of this one.

When you first see body text at 16 pixels, it might seem quite large. Once you get used to the larger type, however, most people find it far easier to read; and going back to a page where main type is 12 pixels will often then look quite small.

![](imgs/ch12 - type scales.jpg)

###UNITS OF TYPE SIZE

![](imgs/ch12 - units of type size.jpg)

Setting font size in pixels is the best way to ensure that the type appears at the size you intended (because percentages and ems are more likely to vary if a user has changed the default size of text in their browser).

Pixels are relative to the resolution of the screen, so the same type size will look larger when a screen has a resolution of 800×600 than it would when it is 1280×800.

You can also use **pt for point** sizes instead of px for pixels, but you should only do this when creating style sheets for **printer-friendly** versions of pages.

The **default size** of text in a web browser is **16 pixels**. Using percentages of this amount, you can create a scale where the default text size is 12 pixels, and headings are sized in relation to this.

It is possible for users to change the default size of text in their web browsers. If they have done this, the fonts will be displayed at the same scale that the designer intended, but at a larger size.

**```Ems```** allow you to change the size of text relative to the size of the text in the parent element. Since the default size of text in web browsers is 16 pixels, you can use similar rules to those shown for percentages.

Because users can change the default size of text in their browser, the fonts could all appear larger (or smaller) than the designer intended.

###MORE FONT CHOICE

**```@font-face```**

```@font-face``` allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.

**```font-family```**

This specifies the name of the font. This name can then be used as a value of the font-family property in the rest of the style sheet (as shown in the rule for the ```<h1>``` and ```<h2>``` elements).

**```src```**

This specifies the path to the font. In order for this technique to work in all browsers, you will probably need to specify paths to a few different versions of the font.

**```format```**

This specifies the format that the font is supplied in.

![](imgs/ch12 - font-face.jpg)
![](imgs/ch12 - font-face result.jpg)

Many typeface makers do not allow you to use their fonts in this way, but there are open source fonts you can use freely. You can find lists of them at:
* http://www.fontsquirrel.com
* http://www.fontex.org
* http://www.openfontlibrary.org

When looking at fonts on these sites, it is still important to check the font's license agreement because some fonts are only free for personal use (that is, not for use on commercial websites).

There are some sites that give you access to use commercial fonts, because they negotiated permission to let their customers use these fonts for a fee:
* http://www.typekit.com
* http://www.kernest.com
* http://www.fontspring.com

**Google** also provides **open source fonts**. Rather than adding the ```font-face``` rule to your own style sheet, you link to a CSS file and font files on their servers: http://fonts.google.com

###UNDERSTANDING FONT FORMATS

![](imgs/ch12 - understanding font formats.jpg)
![](imgs/ch12 - understanding font formats result.jpg)

Because the browser needs to download the font file in order to show it, users might see something known as a Flash of Unstyled Content (FOUC) or Flash of Unstyled Text (FOUT). Two things you can do to try to minimize this behavior are to delete any unneccesary glyphs from the font and/or host the font on a Content Delivery Network (a special type of web hosting that offers faster delivery of files).

Different browsers support different formats for fonts (in the same way that they support different audio and video formats), so you will need to supply the font in several variations to reach all browsers.

If you do not have all of these formats for your font, you can upload the font to a website called FontSquirrel where they will convert it for you:
http://www.fontsquirrel.com/fontface/generator

Font Squirrel also provides you with the CSS code for the @font-face rule. This is very helpful because, when you are dealing with multiple font formats, the src and format properties of the ```@font-face``` rule can get rather complicated.

The various font formats should appear in your code in this order:
1. eot
2. woff
3. ttf/otf
4. svg

###BOLD

![](imgs/ch12 - font weight.jpg)
![](imgs/ch12 - font weight result.jpg)

####```font-weight```
The font-weight property allows you to create bold text. There are two values that this property commonly takes:

**```normal```**

This causes text to appear at a normal weight.

**```bold```**

This causes text to appear bold.
In this example, you can see that the element whose class attribute has a value of credits has been bolded.

You might wonder why there is a normal weight. This is because if, for example, you created a rule for the ```<body>``` element indicating that all text inside the body should appear bold, you might need an option that allows the text in certain instances to appear normal weight. So it is essentially used as an “off switch.”

###ITALIC
![](imgs/ch12 - font style.jpg)
![](imgs/ch12 - font style result.jpg)

####```font-style```
If you want to create italic text, you can use the ```font-style``` property. There are three values this property can take:

**```normal```**

This causes text to appear in a normal style (as opposed to italic or oblique).

**```italic```**

This causes text to appear italic.

**```oblique```**

This causes text to appear oblique.

Italic fonts were traditionally stylized versions of the font based on calligraphy, whereas an oblique version would take the normal version and put it on an angle.

It is not unusual for the browser to fail to find an italic version of a typeface, in which case it will use an algorithm to place the normal version of the type on a slant, which means that a lot of italic text online is actually oblique.

###UPPERCASE & LOWERCASE

![](imgs/ch12 - text transform.jpg)
![](imgs/ch12 - text transform result.jpg)

####```text-transform```
The ```text-transform``` property is used to change the case of text giving it one of the following values:

**```uppercase```** - This causes the text to appear uppercase.

**```lowercase```** - This causes the text to appear lowercase.

**```capitalize```** - This causes the first letter of each word to appear capitalized.

In this example, the ```<h1>``` element is uppercase, the ```<h2>``` element is lowercase, and the credits are capitalized. In the HTML, the word by in the credits had a lowercase b.

If you do utilize the uppercase option, it is worth looking at the letter-spacing property to increase the gap between each letter as shown on page 284. This will help improve readability.

###UNDERLINE & STRIKE

![](imgs/ch12 - text decoration.jpg)
![](imgs/ch12 - text decoration result.jpg)

####```text-decoration```
The ```text-decoration``` property allows you to specify the following values:

**```none```** - This removes any decoration already applied to the text.

**```underline```** - This adds a line underneath the text.

**```overline```** - This adds a line over the top of the text.

**```line-through```** - This adds a line through words.

**```blink```** - This animates the text to make it flash on and off (however this is generally frowned upon, as it is considered rather annoying).

In this example, the credits have been underlined. Also, the name of the breed (which is a link) is not underlined, which it would be by default because it is a link. This property is commonly used by designers to remove the underlines that browsers place under links. 

###LEADING

Leading (pronounced *ledding*) is a term typographers use for the vertical space between lines of text. In a typeface, the part of a letter that drops beneath the baseline is called a **descender**, while the highest point of a letter is called the **ascender**. Leading is measured from the bottom of the descender on one line to the top of the ascender on the next.

![](imgs/ch12 - leading.jpg)

####```line-height```
In CSS, the ```line-height``` property sets the height of an entire line of text, so the difference between the font-size and the line-height is equivalent to the leading (as shown in the diagram above).

Increasing the line-height makes the vertical gap between lines of text larger.

![](imgs/ch12 - line-height.jpg)
![](imgs/ch12 - line-height result.jpg)
![](imgs/ch12 - line-height result minus css.jpg)

Increasing the default amount of leading can make text easier to read. **The vertical space between lines should be larger than the space between each word as this helps the eye move along the line instead of down them**. 

A good starter setting is around 1.4 to 1.5em. Because users can adjust the default size of text in their browser, the value of the ```line-height``` property is best given in ```ems```, not pixels, so that the gap between lines is relative to the size of text the user has selected.

###LETTER & WORD SPACING

![](imgs/ch12 - letter and word spacing.jpg)
![](imgs/ch12 - letter and word spacing result.jpg)
![](imgs/ch12 - letter and word spacing result minus css.jpg)

####```letter-spacing```, ```word-spacing```

**Kerning** is the term typographers use for the space between each letter. You can control the space between each letter with the ```letter-spacing``` property.

**It is particularly helpful to increase the kerning when your heading or sentence is all in uppercase. If your text is in sentence (or normal) case, increasing or decreasing the kerning can make it harder to read.**

You can also control the gap between words using the ```word-spacing``` property.

When you specify a value for these properties, it should be given in ems, and it will be added on top of the default value specified by the font.

The default gap between words is set by the typeface (often around 0.25em), and it is unlikely that you would need to change this property regularly. If the typeface is bold or you have increased the space between letters, then a larger gap between words can increase readability.

###ALIGNMENT

![](imgs/ch12 - text align.jpg)
![](imgs/ch12 - text align result.jpg)

####```text-align```
The text-align property allows you to control the alignment of text. The property can take one of four values:

**```left```** - This indicates that the text should be left-aligned.

**```right```** - This indicates that the text should be right-aligned.

**```center```** - This allows you to center text.

**```justify```** - This indicates that every line in a paragraph, except the last line, should be set to take up the full width of the containing box.

When you have several paragraphs of text, it is considered easiest to read if the text is left-aligned.

Justified text looks at the words on each individual line and creates an equal gap between those words. It can look odd if you end up with large gaps between some words and smaller gaps between others. This often happens when your lines are not very wide or when your text contains long words.

###VERTICAL ALIGNMENT

![](imgs/ch12 - vertical align.jpg)
![](imgs/ch12 - vertical align result.jpg)

####```vertical-align```

The ```vertical-align``` property is a common source of confusion. It is not intended to allow you to vertically align text in the middle of block level elements such as ```<p>``` and ```<div>```, although it does have this effect when used with table cells (the ```<td>``` and ```<th>``` elements).

It is more commonly used with inline elements such as ```<img>```, ```<em>```, or ```<strong>``` elements. When used with these elements, it performs a task very similar to the HTML ali gn attribute used on the ```<img>``` element, which you met on pages 103-106. The values it can take are:
* baseline
* sub
* super
* top
* text-top
* middle
* bottom
* text-bottom

It can also take a **length** (usually specified in pixels or ems) or a **percentage** of the line height.

###INDENTING TEXT

![](imgs/ch12 - text ident.jpg)
![](imgs/ch12 - text ident result.jpg)

####```text-ident```

The ```text-indent``` property allows you to indent the first line of text within an element. The amount you want the line indented by can be specified in a number of ways but is usually given in pixels or ems.

It can take a negative value, which means it can be used to push text off the browser window. You can see this technique used in this example, where the ```<h1>``` element uses a background image to represent the heading. The text has been moved far to the left, off the screen.

We still want the heading text to be on the page (for search engines and those who cannot see the image), but we cannot have it displayed on top of the logo or it will be unreadable. By pushing it 9,999 pixels to the left, it is way out of sight but still in the HTML code.

The second rule in this example indents the credits 20 pixels to the right.

###CSS3: DROP SHADOW

![](imgs/ch12 - text shadow.jpg)
![](imgs/ch12 - text shadow result.jpg)

####```text-shadow```

It is used to create a drop shadow, which is a dark version of the word just behind it and slightly offset. It can also be used to create an embossed effect by adding a shadow that is slightlylighter than the text.

The value of this property is quite complicated because it can take three lengths and a color for the drop shadow:

* The first length indicates how far to the left or right the shadow should fall.
* The second value indicates the distance to the top or bottom that the shadow should fall.
* The third value is optional and specifies the amount of blur that should be applied to the drop shadow.
* The fourth value is the color of the drop shadow.

###FIRST LETTER OR LINE

![](imgs/ch12 - first letter or line.jpg)
![](imgs/ch12 - first letter or line result.jpg)

####```:first-letter```, ```:first-line```

Technically these are not properties. They are known as **pseudo-elements**.

You specify the pseudo-element at the end of the selector, and then specify the declarations as you would normally for any other element.

CSS introduces both **pseudo-elements** and **pseudo-classes**. A pseudo-element acts like an extra element is in the code. In the case of the ```:first-letter``` and ```:first-line``` **pseudo elements**, it is as if there is an extra element around the first letter or the first line which can have its own styles applied.

A **pseudo-class** acts like an extra value for a class attribute. In the case of the ```:visited``` **pseudo-class** it allows you to have different styles for links that have been visited. Similarly, the ```:hover``` **pseudo-class** allows you to style elements differently when a user hovers over them.

###STYLING LINKS

![](imgs/ch12 - link visited.jpg)
![](imgs/ch12 - link visited result.jpg)

####```:link```, ```:visited```

Browsers tend to show links in blue with an underline by default, and they will change the color of links that have been visited to help users know which pages they have been to.

In CSS, there are two **pseudo-classes** that allow you to set different styles for links that have and have not yet been visited.

**```:link```** - This allows you to set styles for links that have not yet been visited.

**```:visited```** - This allows you to set styles for links that have been clicked on.

###RESPONDING TO USERS

![](imgs/ch12 - link hover active focus.jpg)
![](imgs/ch12 - link hover active focus result.jpg)

####```:hover```, ```:active```, ```:focus```

There are three pseudo-classes that allow you to change the appearance of elements when a user is interacting with them.

**```:hover```** - This is applied when a user hovers over an element with a pointing device such as a mouse. This has commonly been used to change the appearance of links and buttons when a user places their cursor over them. It is worth noting that such events do not work on devices that use touch screens (such as the iPad) because the screen is not able to tell when someone is hovering their finger over an element.

**```:active```** - This is applied when an element is being activated by a user; for example, when a button is being pressed or a link being clicked. Sometimes this is used to make a button or link feel more like it is being pressed by changing the style or position of the element slightly.

**```:focus```** - This is applied when an element has focus. Any element that you can interact with, such as a link you can click on or any form control can have focus.

Focus occurs when a browser discovers that you are ready to interact with an element on the page. For example, when your cursor is in a form input ready to accept typing, that element is said to have focus. It is also possible to use the tab key on your keyboard to move through the interactive items on a page. 

When pseudo-classes are used, they should appear in this order: 
1. ```:link``` 
2. ```:visited```
3. ```:hover```
4. ```:focus```
5. ```:active```

###ATTRIBUTE SELECTORS

There are also a set of attribute selectors that allow you to create rules that apply to elements that have an attribute with a specific value.

###SUMMARY TEXT
* There are properties to control the choice of font, size, weight, style, and spacing.
* There is a limited choice of fonts that you can assume most people will have installed.
* If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
* You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.
* You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

## 13. BOXES

