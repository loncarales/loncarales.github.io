# My JSON Resume

## What is my JSON Resume?

It is my personal resume writen in [JSON Resume](https://jsonresume.org/). The open source initiative to create a JSON-based standard for resumes.

## Usage

1. Download [JSON Resume CLI](https://jsonresume.org/)

```bash
npm install -g resume-cli
```

Simply run

```bash
resume serve --theme .
```

3. Use resume cli to build your resume

```
resume export index.html --theme .
```

### PDF output

Download a precompiled binary from [wkhtmltopdf](https://wkhtmltopdf.org) and run your HTML document through the tool.

For example, if I really like the treatment Google has done to their logo today and want to capture it forever as a PDF:

```bash
wkhtmltopdf http://google.com google.pdf
```
