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


## Remark template

Have a look at [Remark](https://github.com/gnab/remark) (it's great). I've added
[Font-awesome](http://fontawesome.io/icons/) to use some icon.

### How to use it

Open `index.html` with your favorite Web Browser, then:


- `F`: full screen mode
- `P`: toogle presenter mode
- `C`: open a new-synchronised windows
- `Number + enter`: go to Number slide
- `H` or `?`: toogle the help



## Slidify template

[Slidify](http://slidify.org/) is an R package that "helps you create and publish beautiful HTML5 presentations from RMarkdown". I have used it for some tutorials, very useful! Note however is author haven't updated the package since September 5th, 2015. Also note I put the presentation in a `docs` folder for publication on Github.



## Slidy Presentation

I use the [Rmarkdown integration](http://rmarkdown.rstudio.com/slidy_presentation_format.html).

### Display Modes

- 'C' Show table of contents
- 'F' Toggles the display of the footer
- 'A' Toggles display of current vs all slides (useful for printing handouts)
- 'S' Make fonts smaller
- 'B' Make fonts larger


## ioSlides Presentation

I use the [Rmarkdown integration](http://rmarkdown.rstudio.com/ioslides_presentation_format.html)
for ioSlides, they did a great job!


### Display Modes

- 'f' enable fullscreen mode
- 'w' toggle widescreen mode
- 'o' enable overview mode
- 'h' enable code highlight mode
- 'p' show presenter notes


## Make your life easier with R markdown integration

These integrations are fantastic! You can do even better by using a
simple bash function (very helpful if you aren't a Rstudio user and a shell
user).

```bash
rmdto() {
  Rscript --no-init-file -e "rmarkdown::render('$1', output_format = 'all')";
}
```



## Todo

- [ ] faire une simple page qui montre mes templates (on aurait un lien pour chaque, au moins les html)
- [ ] customize Slidy (so far I've used the example on the R markdown website)
- [ ] customize ioSlides (same comment as above)
- [ ] try [shower](https://shwr.me/#) and the [.Rmd integration](https://github.com/mangothecat/rmdshower)
by Gabor Csardi
