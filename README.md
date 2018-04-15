# LinuxIsBadass
Linux is Badass. The E-book.

This is to my knowledge the only free ePub of Bryan Lunduke's *Linux is Badass (Slightly More Badass Edition)* and best of all the CC-BY-NC-SA license means I can't sell it even if I wanted to. Also this e-book was solely developed on a Mac, partly for my amusement given the book's subject material.

Jokes aside, support Bryan Lunduke via Patreon: https://www.patreon.com/bryanlunduke

I don't agree with the guy on everything, but he's still a good example of a GNU/Linux community member.

## Featuring

* Better typesetting (than the PDF at least as I haven't seen the physical book or official e-book formats) with initial letters and non-indented starting paragraphs. I hope the typesetting is better when I inevitably grab a physical paperback.
* New better-res covers that use Red Hat's [Overpass](https://github.com/RedHatBrand/Overpass) typeface (and some [IBM Plex Mono](https://github.com/IBM/plex) too). There's a Fedora joke there somewhere.
* DID I MENTION IT'S **FREE**?! As in beer and price.

## Compiling

I do leave compilation instructions and there no proprietary programming languages or IDEs (*cough* Xojo *cough*). Nor fears of vendor lock-in here. My setup for generating an ePub merely uses Python, epubcheck and GNU Bash.

A new ePub file can be made by using the provided `CreateE-book.py` via installing [Python 3](https://www.python.org/downloads/) and then ~~running the script on IDLE, [Thonny](http://thonny.org/) or~~ the `python3 CreateE-book.py` command on GNU Bash (macOS and GNU/Linux Terminal). The script however **does not** work with Python 2 and I have no plans to backport.

XHTML, CSS and the `metadata.json` files can be edited using a text editor such as [Atom](https://atom.io/) and [Notepad++](https://notepad-plus-plus.org/).

The `toc.ncx` and `content.opf` are generated by the `CreateE-book.py` and shouldn't be edited as they would be overwritten.

If you need to check the e-book yourself run `java -jar epubcheck.jar LinuxIsBadass.epub` from on the GNU Bash terminal (macOS and GNU/Linux) after moving to the folder that the ePub file is placed in.

I personally combine the commands by running `python3 CreateE-book.py && java -jar epubcheck.jar LinuxIsBadass.epub` to streamline things.

## Licensing:

Book content such as text and images are licensed under the **Creative Commons Attribution-Noncommercial-ShareAlike 3.0**.

Book code such as the .xhtml, .css and .xml files are licensed under **Creative Commons Zero 1.0 Universal (CC0 1.0)**.

The IDPF's `epubcheck-4.0.2` tool is licensed under **Apache License 2.0**, **Mozilla Public License** and **BSD 3-clause License**.

![Cover](https://github.com/inferno986return/LinuxIsBadass/blob/master/e-book/OEBPS/images/cover.png)
