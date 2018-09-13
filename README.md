# modest
Modest is a theme for Hugo static site generator. It is built with CSS grid and a little bit vanilla Javascript.
## Design approaches
- Progressive enhancement. This theme works well enough with javascript turned off. 
- Content first.
- Accessibility.
- Readability.
## Pictures
This theme works well with Cloudinary. You have to specify you cloudinary address base in your Hugo configuration file:
``` toml
cloudinary_base_url = "https://res.cloudinary.com/geri-darbai/image/upload/"
```
And then you can use this shortcode to insert link to picture into markdown with link to specific picture:
``` HTML
{{<cloudinary src="cloudinary-folder/name-of-picture.jpg" max-width="30em" alt="Alternative text" title="Picture title" attrlink="https://example.com">}}
```
Cloudinary automaticaly makes picture manipulations and serve the size you need.
## Rough edges
- Scrollspy works only with latin characters in anchor headings. Workaround for this is to assign headers id's manually directly in markdown:
``` Markdown
## Švenčiausiąjį {#svenciausiaji}
```
- scrollspy is a little bit "drunk". If you have small sections, it will probably miss.
- CSS and Javascript is put directly into html for the better pagespeed scores (no external css/javascript files. In order to make changes you have to edit critical-theme.less and footer.html files.
## TODO
- i18n.
## Credits
- To Steve Francia (spf13), Bjørn Erik Pedersen (bep) and all [Hugo](https://gohugo.io/) team
- To Vimux for Hugo [blank theme](https://themes.gohugo.io/blank/) which was used as a starter of modest theme. 
- To Leonardo Santos for [menuspy.js](https://github.com/lcdsantos/menuspy) which was used to implement scrollspy functionality.
- To Julian Knight for a snippet how to [add anchors next to headers](https://discourse.gohugo.io/t/adding-anchor-next-to-headers/1726/13). 
## Contributions ...
... and feedback are very much welcome.




