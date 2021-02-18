# HTML Images; CSS Color & Text

## Images

### What will we read?
* How to add images to pages
* hoosing the right format
* Optimizing images for the web

### There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart.

### Choosing Images for Your Site.
* A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one.

* Images can be used to set the tone for a site in less time than it takes to read a description.


### Storing Images on Your Site

* it is good practice to create a folder for all of the images the site uses.
* As a website grows, keeping images in a separate folder helps you understand how the site is organized.

### Adding Images
* To add an image into the page you need to use an **< img>** element.
* This is an empty element *(which means there is no closing tag)*.
* It must carry the following two attributes:
1. **src**
    * This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.
2. **alt**
    * This provides a text description of the image which describes the image if you cannot see it.
3. **title**
    * You can also use the title attribute with the **< img>** element to provide additional information about the image.

* The text used in the alt attribute is often referred to as **alt text**.
* It should give an accurate description of the image content so it can be understood by screen reader software and search engines.

[Insert-Image](images/insert-image.jpg)

### Height & Width of Images
* You will also often see an **< img>** element use two other attributes that specify its size:
1. **height**
This specifies the height of then image in pixels.
2. **width**
This specifies the width of the image in pixels.

* A good idea to specify the size of the image so that the browser can render the rest of the text on the page while leaving the right amount of space for the image that is still loading.

### Where to Place Images in Your Code
* Three Examples of image placement that produce different results:
1. before a paragraph.
    * The paragraph starts on a new line after the image.
2. inside the start of a paragraph.
    * The first row of text aligns with the bottom of the image.
3. In the middle of a paragraph.
    * The image is placed between the words of the paragraph that it appears in.

[Insert-Image-Code](images/insert-image-code.jpg)

[Insert-Image-Result](images/insert-image-result.jpg)

### Aligning Images Horizontally
* align
    * The align attribute was commonly used to indicate how the other parts of a page should flow around an image.

* The align attribute can take these horizontal values:
1. left
    This aligns the image to the left (allowing text to flow around its right-hand side).
2. right
    This aligns the image to the right (allowing text to flow around  its left-hand side).

[Image-Align-Code](images/image-align-code.jpg)

[Image-Align-Result](images/image-align-result.jpg)

### Aligning Images Vertically
* There are three values that the align attribute can take that control how the image should align vertically with the text that surrounds it:
1. top
    This aligns the first line of the surrounding text with the top of the image.
2. middle
    This aligns the first line of the surrounding text with the middle of the image.
3. bottom
    This aligns the first line of the surrounding text with the bottom of the image.

[Image-align-ver-code](images/image-align-ver-code.jpg)

[Image-align-ver-result](images/image-align-ver-code.jpg)

### Three Rules for Creating Images
1. Save images in the right format.
2. Save images at the right size.
3. Use the correct resolution.

### Tools to Edit & Save Images
* There are several tools you can use to edit and save images to ensure that they are the right size, format, and resolution.

* The most popular tool amongst web professionals is **Adobe Photoshop**.

### Image Formats:
1. JPEG

[Image-Type](images/image-type.jpg)

2. PNG

[Circle.PNG](images/circle.png)

### Image Dimensions

[Image-Dimension](images/image-dimension.jpg)

### Images Edits:
1. Cropping Images
    * When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.

2. Image Resolution
    * Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.
    * JPGs, GIFs, and PNGs belong to a type of image format known as **bitmap**.
    * Images appearing on computer screens are made of tiny squares called **pixels**.

### Vector Images
* Vector images are commonly created in programs such as **Adobe Illustrator**.

* The current method of using vector images for display on websites involves saving a bitmap version of the original vector image and using that.

* **Scalable Vector Graphics (SVG)** are a relatively new format used to display vector images directly on the web , however its use is not yet widespread.

* The advantage of creating line drawings in vector format is that you can *increase the dimensions* of the image without *affecting the quality* of it.

[Image-Vector](Images/iamge-vector.jpg)

### Animated GIFs

* Animated GIFs show several frames of an image in sequence and  therefore can be used to create simple animations.

* Each extra frame of the image increases the size of the file, and can therefore add to the time it takes for an image to download

3. Transparency
* Creating an image that is partially transparent for the web involves selecting one of two formats:
1. Transparent GIF
    * If the transparent part of the image has straight edges and it is 100% transparent (that is, not semi-opaque), you can save the image as a GIF (with the transparency option selected).
2. PNG
    * If the transparent part of the image has diagonal or rounded edges or if you want a semiopaque transparency or a dropshadow, then you will need to save it as a PNG.

### Examining Images on the Web

* Checking the Size of Images
    * If you are updating a website, you might need to check the size of an existing image before creating a new one to replace it.

[Image-Size](images/image-size.jpg)

* Downloading Images
If you want to download images from a website, you can do so by
accessing the same pop-up menu.

[Image-Download](images/image-download.jpg)

### how to download images in browsers : 

1. CHROME
    * Size: Open Image in New Tab
    * Size appears in new tab
    * Download: Save Image As
2. FIREFOX
    * Size: View Image Info
    * Size appears in pop-up window
    * Download: Save Image As*
3. Internet Explorer
    * Size: Properties
    * Size appears in pop-up window
    * Download: Save Image
4. SAFARI
    * Size: Open Image in New Tab
    * Size appears in title bar
    * Download: Save Image As

### HTML 5: Figure and Figure Caption
1. **< figure>**
    * Images often come with captions. HTML5 has introduced a new *< figure>* element to contain images and their caption so that the two are associated.
    * You can have more than one image inside the *< figure>* element as long as they all share the same caption.

2. **< figcaption>**
   * The *< figcaption>* element has been added to HTML5 in order to allow web page authors to add a caption to an image.
    * Before these elements were created there was no way to associate an *< img>* element with its caption. 

***
***

## Color

* Color can really bring your pages to life.

### What will we read? 
* How to specify colors
* Color terminology and contrast
* Background color

### Foreground Color
1. color
The color property allows you to specify the color of text inside an element.
You can specify any color in CSS in one of three ways:
   * rgb values
    These express colors in terms of how much red, green and blue are used to make it up.
    For example: rgb(100,100,90)
    * hex codes
    These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash #sign.
    For example: #ee3e80
    * color names
    There are 147 predefined color names that are recognized by browsers.
    For example: DarkCyan

### Background Color
1. background-color
You can specify your choice of background color in the same three ways you can specify foreground colors: **RGB values**, **hex codes**, and **color names**.

### Understanding Color
* Every color on a computer screen is created by mixing amounts of **red, green, and blue**. To find the color you want, you can use a **color picker**.

* Computer monitors are made up of thousands of tiny squares called **pixels**.

* Color picking tools are available in image editing programs like **Photoshop and GIMP**. You can see the **RGB values** specified next to the radio buttons that say **R, G, B**.

* The hex value is provided next to the pound or hash *#* symbol

[Image-Color-Picker](images/image-color-picker.jpg)


## Contrast

* When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be **Legible**.

* Low Contrast: Text is harder to read when there is low contrast between background and foreground colors.

* Medium Contrast: For long spans of text, reducing the contrast a little bit improves readability.

* High Contrast: Text is easier to read when there is higher contrast between background and foreground colors.

***

## Opacity & RGBA

**Opacity** 
* Allows you to specify the opacity of an element and any of its child elements.
* The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

**RGBA**
* allows you to specify a color, with adds a fourth value to indicate opacity.
* This value is known as an **Alpha value** and is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

***

## HSL Colors
* HUE: The colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360.

* Saturation: The amount of gray in a color.
Saturation is represented as a percentage.
100% is full saturation and 0% is a shade of gray.

* Lightness: The amount of white (lightness) or black (darkness) in a color. 
Lightness is represented as a percentage. 
0% lightness is black, 100% lightness is white, and 50% lightness is normal. 
Lightness is sometimes referred to as luminosity.

***

## HSL & HSLA

* **HSL** : a way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for:
1. HUE
2. Saturation
3. Lightness

* **HSLA** : Allows you to specify color properties using Hue, Saturation, and Lightness as above, and adds a fourth value which represents **Transparency**.

* This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.

[Color-Sample](images/color-sample.png)

***
***

## Text

* Size and typeface of text
* Bold, italics, capitals, underlines
* Spacing between lines, words, and letters

### Typeface Terminology

[Typeface-Terminology](image/typeface-terminology.jpg)

[Typeface-Terminology1](image/typeface-terminology1.jpg)

### Choosing a Typeface for your Website
* When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.

1. Serif
    Serif fonts have extra details on the end of the main strokes of the letters.
[Text-serif](images/text-serif.jpg)


2. Sans-Serif
    Sans-serif fonts have straight ends to letters and therefore have a much cleaner design.

[Text-sans-serif](images/text-sans-serif.jpg)

3. Monospace
    * Every letter in a monospace typeface is the same width. (Non-monospace fonts have different widths.)
[Text-monospace](images/text-monospace.jpg)


4. Cursive
    Cursive fonts either have joining strokes or other cursive characteristics, such as handwriting styles.
[Text-Cursive](images/text-cursive.jpg)

5. Fantasy
    Fantasy fonts are usually decorative fonts and are often used for titles. They're not designed for long bodies of text.
[Text-fantasy](images/text-fantasy.jpg)

### Techniques That Offer a Wider Choice ofTypefaces

* If you design on a Mac, it is important to check what the typefaces look like on a PC because PCs can render type less smoothly. But if you design on a PC, then it should look fine on a Mac.

### Specifying Typefaces
1. font-family
* The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.
* The value of this property is the name of the typeface you want to use.

* You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list.

[Font-Family-Code](images/font-family-code.jpg)

[Font-Family-Result](images/font-family-result.jpg)

### Size of Type
1. font-size
* The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:
    1. Pixels
    Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px.
    2. Percentages
    The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.
    3. EMS
    An em is equivalent to the width of a letter m.

### Type Scales

[Text-Scale](images/text-scale.jpg)

1. **Pixels**
* Setting font size in pixels is the best way to ensure that the type appears at the size you intended

* Pixels are relative to the resolution of the screen, so the same type size will look larger when a screen has a resolution of 800x600 than it would when it is 1280x800.

2. **Percentages**
* The default size of text in a web browser is 16 pixels. Using percentages of this amount, you can create a scale where the default text size is 12 pixels, and headings are sized in relation to this.

3. **EMS**
* Ems allow you to change the size of text relative to the size of the text in the parent element. Since the default size of text in web browsers is 16 pixels, you can use similar rules to those shown for percentages.

[Text-Scale1](images/text-scale1.jpg)


### **@font-face**
* **@font-face** allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.

* You add the font to your style sheet using the @font-face rule.

1. font-family
This specifies the name of the font. This name can then be used as a value of the font-family property in the rest of the style sheet.
2. src
This specifies the path to the font. In order for this technique to work in all browsers, you will probably need to specify paths to a few different versions of the font.
3. format
This specifies the format that the font is supplied in.

* there are open source fonts you can use freely.
You can find lists of them at:
1. ![fontsquirre](www.fontsquirrel.com)
2. ![fontex](www.fontex.org)
3. ![typekit](www.typekit.com)
![kernest](www.kernest.com)
![fontspring](www.fontspring.com)

### Font Formats
1. Bold (font-weight )
The font-weight property allows you to create bold text.
There are two values that this property commonly takes:
* normal
This causes text to appear at a normal weight.
* bold
This causes text to appear bold.

2. Italic ( font-style)
If you want to create italic text, you can use the font-style property. 
There are three values this property can take:
* normal
This causes text to appear in a normal style (as opposed to italic or oblique).
* italic
This causes text to appear italic.
* oblique
This causes text to appear oblique.

3. UpperCase & LowerCase ( text-transform)
The text-transform property is used to change the case of text giving it one of the following values:
* uppercase
This causes the text to appear uppercase.
* lowercase
This causes the text to appear lowercase.
* capitalize
This causes the first letter of each word to appear capitalized.

4. Underline & Strike( text-decoration)
The text-decoration property allows you to specify the following values:
* none
This removes any decoration already applied to the text.
* underline
This adds a line underneath the text.
* overline
This adds a line over the top of the text.
* line-through
This adds a line through words.
* blink
This animates the text to make it flash on and off.

5. Leading( line-height)
* Leading (pronounced ledding) is a term typographers use for the vertical space between lines of text. In a typeface, the part of a letter that drops beneath the baseline is called a **descender**, while the highest point of a letter is called the **ascender**. Leading is measured from the bottom of the descender on one line to the top of the ascender on the next.

6. Lett er & Word Spacing( letter-spacing, word-spacing)

[Text-leter](images/text-leter.jpg)


7. Alignment (text-align)

* The text-align property allows you to control the alignment of text. The property can take one of four values:
1. left
    This indicates that the text should be left-aligned.
2. right
    This indicates that the text should be right-aligned.
3. center
    This allows you to center text.
4. justify
    This indicates that every line in a paragraph, except the last line, should be set to take up the full width of the containing box.

8. Vertical Alignment (vertical-align)
* The vertical-align property is a common source of confusion. It is not intended to allow you to vertically align text in the middle of block level elements
* The values it can take are:
    * baseline
    * sub
    * super
    * top
    * text-top
    * middle
    * bottom
    * text-bottom

9. Indenting Text (text-indent)
* allows you to indent the first line of text within an element.

10. Drop Shadow (text-shadow)

* The text-shadow property has become commonly used despite lacking support in all browsers. It is used to create a drop shadow, which is a dark version of the word just behind it and slightly offset. It can also be used to create an embossed effect by adding a shadow that is slightly lighter than the text.

[Text-shadow](images/text-shadow.jpg)

11. First Lett er or Line (:first-letter, :first-line)
* You can specify different value for the first letter or first line of text inside an element using **:first-letter** and **:first-line**.
Technically these are not properties. They are known as **pseudo-elements**

12. Styling Links (:link, :visited)
* there are two **pseudo-classes** that allow you to set different styles for links that have and have not yet been visited.
    1. **:link**
    This allows you to set styles for links that have not yet been
visited.
    2. **:visited**
    This allows you to set styles for links that have been clicked on.

13. Responding to Users (:hover, :active, :focus)
* There are three pseudo-classes that allow you to change the appearance of elements when a user is interacting with them.
    1. **:hover**
    This is applied when a user hovers over an element with a pointing device such as a mouse.

    2. **:active**
    This is applied when an element is being activated by a user.
    3. **:focus**
    This is applied when an element has focus. Any element that you can interact with, such as a link you can click on or any form control can have focus.

[Text-responding](images/text-responding.jpg)


### Attribute Selectors

[Attribute-Selector](images/att-selector.jpg)














