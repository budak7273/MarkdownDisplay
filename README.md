# MarkdownDisplay

A static page that loads and markdown-formats a webpage supplied as a URL parameter as the contents of the current page. Can also scroll to headings in the linked markdown file with standard `#id` syntax.

Usage example: `.../MarkdownDisplay.html?page=https://raw.githubusercontent.com/markedjs/marked/master/README.md#docs`

Uses [Marked](https://github.com/markedjs/marked) to turn the raw Markdown into HTML for display, uses [DOMPurify](https://github.com/cure53/DOMPurify) to clean the supplied url of any possible dangerous HTML, and formats the markdown with [github-markdown-css](https://github.com/sindresorhus/github-markdown-css) for display.

Dangerous HTML is likely not a concern for anything that would use this page, but it's good practice to clean it regardless.
