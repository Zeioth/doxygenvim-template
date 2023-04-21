# Welcome to vim-doxygen

## How to: Edit this page

This is an example main page. You can edit it on:

> ./doxygen/mainpage.md

## How to: Download and use a theme


You can download a
[theme from the community](https://github.com/topics/doxygen-theme) and copy
it inside of your doxygen directory. Normally, this will override the default
DoxyFile. It's fine.

## Make the changes permanent
Once you have installed a theme, and customized your own DoxyFile, it is a
good idea to upload them to a repository. Make sure your repo look exactly
like the file and directory structure of
[vim-doxygen-template](https://github.com/Zeioth/vim-doxygen-template).

```
 " After that, you can tell vim-doxygem to use your template like:
 let g:doxygen_clone_config_repo = 'https://github.com/Zeioth/vim-doxygen-template.git'
```

## Advanced: How to customize an existing theme
The most relevant DoxyFile settings to tweak when customizing or
creating a theme are:

```
# This is just an example, values may difer.

HTML_HEADER            = ./header.html
HTML_FOOTER            = ./footer.html
HTML_STYLESHEET        = ./css-to-replace-doxygen-styles.css
HTML_EXTRA_STYLESHEET  = ./css-to-extend-doxygen-styles.css
HTML_EXTRA_FILES       = ./any-extra-file-you-want-to-include.html \
                         ./should-look-like-this.png \
DOXYGEN_LAYOUT         = ./DoxygenLayout.xml
```

* **Changing the page structure**: Use
DoxygenLayout.xml if you want to alter the page
structure. It is a good idea to look for examples and start from there.

For more info, check the [official doxygen documentation](https://doxygen.nl/manual/customize.html).
