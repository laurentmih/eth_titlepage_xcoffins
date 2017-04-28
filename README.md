# LaTeX coffins design: hands-on
The `xcoffins` package of LaTeX3 allows for some interesting designs, especially for title pages. However, I found documentation lacking. Here, using the example of a report for my school, I show how you can use the `xcoffins` package to attain a relatively simple design. For a walk-through, see my [[blog post]]().

## Image resolution
I have ripped the used images off the public websites of the respective institutions. They provide high-resolution `.eps` files, but those are behind a login-wall, so I'm not clear on the permission to provide them publicly. You can use the package `epstopdf` to deal with `.eps` files in LaTeX.

## Font
The font I'm using here, `DIN Pro`, is a proprietary font. It needs to be installed on the system in order for this to work. If that's not possible for you, just replace the references in `main.tex` to another font that you do have installed.

## XeLaTeX
In order to include fonts in a non-ridiculously complicated fashion, I used the `fontspec` package, but the usual, standard engine, `pdflatex` doesn't support that, so you'll have to use/install `XeLaTeX` (or alternatively `LuaLaTeX` I think).