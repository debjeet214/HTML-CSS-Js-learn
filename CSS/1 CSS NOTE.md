CSS = Cascading Style sheets . (markup = html)
css basically helps in the styling of the webpage. and it makes the webpage looks good and interactive.

CSS TYPE
1. inline CSS   = written inside the indivisual tags using stylew attribute
2. internal CSS = written in a sepage section inside the html code in head section with Style tag
3. External CSS = written in a separate .css file outside html code & link the file with link tag in head
*****************************************************************************************************************************************************
CSS code always apply the style which is written at the last......
like you written the same styling properties with different value through inline , internal & external way
it gives preference to the 1. inline , whichever written last it will be implemented.

* if you add !important tag after a styleing property then it will always get most presidence & can't be overwrite 
 <style>
        p{
            width: 60%;
            background-color: aqua;
            color:rgb(52, 97, 180) !important; **
        }
*****************************************************************************************************************************************************

SELECTORS : those which help to tell the css which targeted html tag to style
1. element selector : p{}  telling p tag to style 

2. universal selector : *{}  means, you want to style all the tags in a 
same way ex. you want the font to be same and change so it is a easy way.

3. id selector : #xlx {}  to target specific tag id to change, there can be mitiple p tag, now if you use element selector it will change all the p tags, but to specifically target one p tag, just give it a id and use id selector to change it's styling only 

4. class selector : .xlx{} this is class selector, it can be applied to all the P tags with the class xlx to change it's style. 

***the ID selector is applied only to one element in a page, whereas the class selector can be applied to several elements on a single page.***
*****************************************************************************************************************************************************

Type of Font in CSS
1. web safe fornt : This fonts that are pre downloaded in the machine 
2.  web font : those that need to take from web and link it in the cose. <link href = >

there is many things to not study at first but you will know about it later while coding more in the future in the projects.
*****************************************************************************************************************************************************

CSS POSITIONING:
1. Static : by default
2. Relative: change the position from it's original position if it is under any other parent div, consider change it's position from that beginning position adding top, bottom, left, right etc.
3. Stickey: to stick the point inside another div.
4. Fixed: to fix the div at a set position even you scroll.
5. Absolute: you can precisely position the div at the position you want respect to the main page position. 
*****************************************************************************************************************************************************
FONT-SIZE ::
Here Size in Words refers to:    larger   smaller    xx-small    x-small    small   medium    large    x-large    xx-larger

Another widely used unit is em. Let's try to understand this, with the help of an example: If we set the font-size of the text in the body as 1em and set the font-size of the h1 heading text as 3em. Then no matter which device, the browser will make sure that the heading text is always 3 times the size of the body text
*****************************************************************************************************************************************************
FONT-WEIGHT ::
number between 100-900, which is divisible by 100, that means the allowed values are 100, 200, 300, 400, 500, 600, 700, 800, and 900. If you keep the value as 400, then the text will be displayed like normal text,
*****************************************************************************************************************************************************

WORD & LETTER SPACING :: type of spacing : normal || initial || inherited || length
The default value for this property is normal. The value inherit means, that this property's value will be inherited from the parent HTML element's style.The length here is because we can also specify a numeric value. Don't get confused by the value that we have to provide for the letter-spacing property, it is just a numeric value, can be negative or positive, with a unit - px or em or inch, etc. For example, letter-spacing: 2px;, will make the letters appear 2px away from each other in the text.
*****************************************************************************************************************************************************

TEXT DIRECTION : in usual the line starts from left to right b. but we can convert in to nright to left by,   direction : rtl ; (rtl = right to left.)
TEXT DECORATION : giving some line decoration to the line . ( text-decoration : none ) m= to remove all deco.
*****************************************************************************************************************************************************

TEXT OVERFLOW ::
     In CSS, the text-overflow property deals with the text that is overflowed or extra. Suppose we created a box and added some text to it, but the text does not fit in the box and runs out of the borderline of the box. This situation is called text overflow. To manage this type of situation, CSS offers the text-overflow property. With the help of this property, we can manage the overflowed text in many ways such as you can clip that text, add a scroll bar, etc.
Example of text-overflow: clip | ellipsis | string | initial | inherit;
*****************************************************************************************************************************************************
Height & Weight options :    width: auto | length | percentage | initial | inherit
*****************************************************************************************************************************************************
  *MARGIN & PADDING :
Margin is the space given between two element of the html outside of the border.
Padding is the space between border and the copntent ....inner space
** margin & padding:  10px ; = all side will get 10px of padding or margin .
   margin & padding:  10px 20px;  = top & bottom will get 10px and right & left get 320 px padding or margin.
   margin & padding:  10px  10px  25px   15px; 
                      top   right bottom left   (configeration)
*****************************************************************************************************************************************************
FILTERS FOR IMAGES IN CSS :::
filter:  blur(spread in px)| brightness() | contrast()| drop-shadow() | grayscale() | hue-rotate()| invert()| opacity()| saturate()| sepia();
*****************************************************************************************************************************************************
CSS offers the transition property which is used to change the state of an element smoothly.
The CSS transition-property is used to specify on which CSS property we want to apply the transition. The properties specified as the value of the transition-property are animated during the transition. like,,   transition-property: none | all | property | initial | inherit; example ::   transition-proprty : width;
we can add multiple transition properties too.
  It is necessary to specify the transition duration because the default value of the transition-duration property is 0s (zero second), and 0 sec means the change happens immediately. otherwise using a value will actually signify for how much time it should change itself.

*****************************************************************************************************************************************************
to do it all together we can simply do it by ,  transition: width 1s ease-in-out, height 1s ease-in-out; 
  as the syntex here is, transition: [property] [duration] [timing-function] [delay];
*****************************************************************************************************************************************************
The transition-delay is used to determine how long we need to wait before the transition effect is applied to the element. The value of this property can be defined in seconds (s) and milliseconds (ms).
