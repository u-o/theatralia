[![Build Status](https://travis-ci.org/rmoehn/theatralia.svg?branch=master)](https://travis-ci.org/rmoehn/theatralia)

# theatralia

The project uses [Midje](https://github.com/marick/Midje/).

## How to run the tests

`lein midje` will run all tests.

`lein midje namespace.*` will run only tests beginning with "namespace.".

`lein midje :autotest` will run all the tests indefinitely. It sets up a
watcher on the code files. If they change, only the relevant tests will be
run again.

## Notes from the start

I looked at current ways to set up a Clojure web application. The most
prominent thing applicable to this application (mainly server-side
stuff) appeared [Luminus](http://www.luminusweb.net/). It claims to be
minimal, but when I look at the Leiningen template, it still sets up a
lot of stuff that I'd like to set up step by step. Additionally it talks
about some things I wouldn't use in my project, most prominently Selmer
for templating and non-Datomic databases. It doesn't talk about Datomic
anywhere, which makes me suspicious. However, Luminus looks like a good
orientation for some things, so you'll probably see comments like
»stolen from Luminus«.

A second thing you should know is Stuart Sierra's
[component](https://github.com/stuartsierra/component) framework.
Consume these:

 - [Stuart Sierra: Components. Just Enough Structure](http://youtu.be/13cmHf_kt-Q) 
 - http://thinkrelevance.com/blog/2013/06/04/clojure-workflow-reloaded 

## Credits

The previous section already named some resources I used for my work. Most of
the source files will also contain a Credits section referencing places on the
web (mainly), where I found snippets or hints about how to write a particular
piece of code.

## License

The MIT License (MIT)

Copyright (c) 2014 Richard Möhn

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
