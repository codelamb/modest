# modest
Modest is a port of niu-x2-sidebar theme from Pelican to Hugo. Hugo blank theme was used as a starter.
Goals of this project are:
[] Perfect pagesspeed scores
[] Perfect lighthouse scores
--Progressive webapp
--Performance
--Accessibility
--Best practices
[] Multilingual
[] Progressive enhancement
[] Content first approach

Built using HUGO, LESS, CSS grid.

###How to insert image into markdown
To reach perfect pagespeed scores images are inserted as background images inside div element. Example:
<div style="background-image: url('../images/image.jpg');padding-top: 45%;" class="bkimg"></div>
This approach reduces quality of a picture and does not allow directly download image file.



