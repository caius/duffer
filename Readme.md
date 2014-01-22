# Duffer

Adds lines numbers to each line in a unified diff. Probably not robust yet, but works for `diff -U0` at least so far.

## Usage

Pipe `diff -U0 file1 fil2` into `duffer` and revel in the numbered output

    $ diff -U0 tmp/{one,two} | ./bin/duffer
    --- tmp/one	2014-01-21 23:19:24.000000000 +0000
    +++ tmp/two	2014-01-21 23:30:06.000000000 +0000
    @@ -5,2 +5,2 @@
    5	-amet,
    6	-consectetur
    5	+amet
    6	+fred
    @@ -8 +8 @@
    8	-elit,
    8	+elit
    @@ -19 +19,2 @@
    19	-aliqua.
    19	+aliqua
    20	+GEORGE
    @@ -24 +25 @@
    24	-veniam,
    25	+veniam
    @@ -36,2 +37 @@
    36	-consequat.
    37	-Duis
    37	+consequat
    @@ -41 +40,0 @@
    41	-in
    @@ -52 +51 @@
    52	-pariatur.
    51	+pariatur
    @@ -58 +57 @@
    58	-proident,
    57	+proident
    @@ -69 +68 @@
    69	-laborum.
    68	+laborum

## License

The MIT License (MIT)
Copyright © 2014 Caius Durling <dev@caius.name>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
