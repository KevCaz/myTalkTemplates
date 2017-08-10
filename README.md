# myTalksTemplate
Collection of templates for my talks



## Beamer templates

Beamer template and its Rmarkdown integration, it is based on https://github.com/SteveViss/Rimouski.
To use the dark version, comment out the line below in `beamerKevCaz.tex` or
in the same line in `header.tex` file if you use the Rmarkdown integration.


```
% \usecolortheme{KevCazDark}
```

### Compile

For the beamer Latex, use `pdflatex` like so:

```
pdflatex beamerKevCa.tex
```

To use and `.Rmd` files instead, use the following command (or click in the right
place if you are a Rstudio user):

```
Rscript --no-init-file  -e 'rmarkdown::render("DemoRmarkdown.Rmd", "all")'
```

<br/>


## remark template

Have a look at [Remark](https://github.com/gnab/remark) (it's great). I've added
[Font-awesome](http://fontawesome.io/icons/) to use some icon.

### How to use it

Open `index.html` with your favorite Web Browser, then:


- `F`: full screen mode
- `P`: toogle presenter mode
- `C`: open a new-synchronised windows
- `Number + enter`: go to Number slide
- `H` or `?`: toogle the help
