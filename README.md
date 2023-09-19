# Libxkbswitch-macosx for Apple Slicon macs

macOS library for [vim-xkbswitch](https://github.com/lyokha/vim-xkbswitch) plugin.
This repository is forked from [myshov/libxkbswitch-macosx](https://github.com/myshov/libxkbswitch-macosx) to support Apple Slicon macs.

## Usage 

- This library uses [xkbswitch-macosx (forked version)](https://github.com/xiehuc/xkbswitch-macosx) - console utility for keyboard layout switching. 
    - Check out README.md of that repository to install the utility.
    - You might not get expected results if you use [xkbswitch-macosx (original version)](https://github.com/myshov/xkbswitch-macosx), so do not use it.
- Put library `libxkbswitch.dylib` (you can find compiled version of it in `./bin`) to `/usr/local/lib`.
    - You can put the file in your preferred `lib`. A configuration change is needed for vim-xkbswitch (`let g:XkbSwitchLib = '/path/to/your/lib/file'`)

## Trouble Shooting

- If you got an error `incompatible architecture`, try to build this library again with `make` or try the original repository (the second link from above)

## License

The MIT License (MIT)

Copyright (c) 2015 Alexander Myshov | Beom, Junhwan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
