# PDF from Scratch

This repository has some pdf files created from zero using the VIM text editor. There are some links from PDF Specification and tutorials.

## Videos tutorial

- [Tutorial 1 by Axolotlic](https://youtu.be/ZQpTTdkIZbs)
- [Intro to PDF by Rosenthol](https://youtu.be/KmP7pbcAl-8)

## Tools

- [PDF Validation Toool](https://pdf-online.com/osa/validate.aspx)

## Uncompress zlib data

Using shell script:

```sh
sudo apt install qpdf
zlib-flate -uncompress < FILE
```

Using python:
```python
import zlib

f = open("FILE","r")
print(
   zlib.decompress(f.read())
)
```

## Uncompress all streams of PDF file

```sh
qpdf \
--compress-streams=n \
--decode-level=all \
old.pdf new.pdf
```

## Documents

 - [Document management - Portable document format - Part1: PDF 1.7](https://www.adobe.com/content/dam/acom/en/devnet/pdf/pdfs/PDF32000_2008.pdf)
 - [PDF Reference 3ed Adobe Portable Document Format](https://www.adobe.com/content/dam/acom/en/devnet/pdf/pdfs/pdf_reference_archives/PDFReference.pdf)
 - [QPDF Manual by Jay Berkenbilt](http://qpdf.sourceforge.net/files/qpdf-manual.pdf)