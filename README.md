`k8env` is a simple way to manage your different Kubernetes contexts.


Installation
------------

    $ pip install k8env

It's recommended to remove your default Kubernetes context, so you don't
accidentially invoke it:

    $ kubectl config unset current-context

You may also want to export your shell prompt:

    $ echo 'export PS1' >> ~/.bash_profile


Usage
-----

To start using a Kubernetes context:

    $ k8env <context>

Now any calls to `kubectl` will use that context.

To stop using that context, simply exit the subshell.

To list available contexts:

    $ k8env --list


License
-------

Copyright (c) 2016 Shotwell Labs, Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
