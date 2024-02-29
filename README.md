      _____                        _______ ____   _____ 
     |  __ \                      |__   __/ __ \ / ____|
     | |  | | ___   ___ ___ ___      | | | |  | | |     
     | |  | |/ _ \ / __/ __/ _ \     | | | |  | | |     
     | |__| | (_) | (_| (_| (_) |    | | | |__| | |____ 
     |_____/ \___/ \___\___\___/     |_|  \____/ \_____|
                                                        

Docco TOC is a fork of Docco that adds a simple table-of-contents
to generated documentation.

-------------------------------------------------------------------------------

Docco is a quick-and-dirty, hundred-line-long, literate-programming-style
documentation generator. For more information, see:

http://jashkenas.github.com/docco/

Installation:

    sudo npm install -g docco-toc

Usage:

    docco-toc [options] FILES

      Options:

        -h, --help             output usage information
        -V, --version          output the version number
        -l, --layout [layout]  choose a built-in layouts (parallel, linear)
        -c, --css [file]       use a custom css file
        -o, --output [path]    use a custom output path
        -t, --template [file]  use a custom .jst template
        -e, --extension [ext]  use the given file extension for all inputs
        -L, --languages [file] use a custom languages.json
        -m, --marked [file]    use custom marked options
