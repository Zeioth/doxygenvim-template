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
Doxygen themes will normally use the next DoxyFile parameters.
Make sure they are correct when installing, or creating a theme.

```
# This is just an example, values may difer.

HTML_HEADER            = ./theme/header.html
HTML_FOOTER            = ./theme/footer.html
HTML_STYLESHEET        = ./theme/css.html
HTML_EXTRA_FILES       = ./theme/any-extra-file-you-want-to-include.html \
                         ./theme/should-look-like-this.png \
DOXYGEN_LAYOUT         = ./DoxygenLayout.xml
```

* **Changing the page structure**: Use
DoxygenLayout.xml if you want to alter the page
structure. It is a good idea to look for examples and start from there.

For more info, check the [official doxygen documentation](https://doxygen.nl/manual/customize.html).
