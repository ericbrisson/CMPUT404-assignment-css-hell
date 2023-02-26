# CMPUT 404 - Assignment 3 - Part 1)
## Eric Brisson - ebrisson - 1615620
### Books chosen:
- [A Room with a View](https://www.gutenberg.org/ebooks/2641)
- [Middlemarch](https://www.gutenberg.org/ebooks/145)
- [Romeo and Juliet](https://www.gutenberg.org/ebooks/1513)
---
### CSS applied:
- paragraphs are themed with a Times New Roman font, 1.2em font size, normal font weight, and a black font color
- divs are also themed the same way as paragraphs, as some of the book `.html` files had text inside of divs with no `<p>` tags
- all headers (`h1` through `h6`) are themed with a Times New Roman font, a bold font weight, and a teal font color
- the HTML body has a background color of #f0e0c6 (yellow-ish), a repeating old paper background, a margin of 30% on the left and right, and has everything centered (using text-align)
- an additional class had a CSS rule written, `fig` because all the book `.html` files had their cover image sitting inside a `div` with the class name `fig`. I wanted to center the book cover along with all the other content on the page, so I gave some margin, text-align, and display rules to this class.

---
### Changes made to the `.html` files
- to all three book's `.html` files, I removed all `<style>` tags to give myself a clean slate, and then added the following right before the closing `</head> tag, to import my CSS file:
```
<!-- import book.css -->
<link rel="stylesheet" href="book.css" type="text/css" />
```

- additionally, `middlemarch.html` for some reason was missing the inline styling that my other `.html` book files used for the table of contents, so that was added inline just to keep things consistent:
```
...
<h2>Contents</h2>
    <table style="margin-left: auto; margin-right: auto">
        <tbody>
...
```

- furthermore, all image book cover's `href` attributes were modified just to point to the correct file name in the root of this folder in each book's `.html` file, to `<BOOK_TITLE>_cover.jpg`.

---
### Screenshots
__A Room with a View:__
![A Room with a View Screenshot](a_room_with_a_view_screenshot.png)

__Middlemarch:__
![Middlemarch Screenshot](middlemarch_screenshot.png)

__Romeo and Juliet:__
![Romeo and Juliet Screenshot](romeo_and_juliet_screenshot.png)