BXtexversion Package
====================

TeX: To get strings of engine names and versions

### System requirement

  * TeX format: LaTeX, plain TeX and iniTeX.
      - It will work as long as `\`, `%`, alphabets and numerals have
        normal (plain-compatible) category codes.
  * TeX engine: (Knuthian) TeX, e-TeX, pdfTeX, LuaTeX, XeTeX, pTeX, upTeX,
    e-pTeX, e-upTeX, ApTeX (pTeX-ng), NTT-jTeX, Omega, Aleph.
      - The engine version string is unavailable on some engines.
  * Dependent packages: None.

### Installation

  - `*.sty` → $TEXMF/tex/latex/bxtexversion

### License

This package is distributed under the MIT License.


The bxtexversion Package ― main
--------------------------------

### Package Loading

In LaTeX: (no options available)

    \usepackage{bxtexversion)

In plain TeX or iniTeX:

    \input bxtexversion.sty

### Usage

  * `\TeXenginename`: The string of the engine name.
  * `\TeXengineversion`: The string of the engine version.
  * `\TeXenginenamefull`: The string of the engine name with version, in
    the form `\TeXenginename-\TeXengineversion`; if `\TeXengineversion`
    is empty then it equals to `\TeXenginename`.

The strings for each engine (of the latest version around 2018/10/04)
is shown below:

    Engine    \TeXenginename \TeXengineversion
    ------    -------------- -----------------
    TeX       TeX            (empty)
    e-TeX     e-TeX          2.6
    pdfTeX    pdfTeX         1.40.19
    LuaTeX    LuaTeX         1.07.0
    XeTeX     XeTeX          0.99999
    pTeX      pTeX           3.8.1
    upTeX,    upTeX,         1.23
    e-pTeX    e-pTeX         3.8.1-180518
    e-upTeX   e-upTeX        1.23-180518
    ApTeX     Asiatic pTeX   (empty)
    NTT-jTeX  JTeX           (empty)
    Omega     Omega          1.15
    Aleph     Aleph          0.0

### Notices for TeX programmers

  * `\TeXenginename` is a non-long macro which once-expands to strings
    of character tokens. Each character has its normal (plain-compatible)
    category code.
  * `\TeXengineversion` is a non-long macro which once-expands to strings
    of character tokens with category code 12.
  * `\TeXenginenamefull` is fully expandable.


Revision History
----------------

  * Version 0.2  〈2018/10/04〉
      - The first public version.

--------------------
Takayuki YATO (aka. "ZR")  
https://github.com/zr-tex8r
