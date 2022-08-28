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
resume export resume.html --theme .
```

### PDF output

Probably you want a PDF version of your resume...

JSONResume CLI should be able to make a PDF out of your JSON but I always struggled to get it to work,
so I switched to a more direct and effective approach.

I use Puppeteer-CLI to make a PDF from my HTML resume.

```
npm install -g puppeteer-cli
puppeteer --margin-top 0 --margin-right 0 --margin-bottom 0 --margin-left 0 --format A4 print resume.html resume.pdf
```

Obviously you could write a very simple Node script to use the real Puppeteer and the `render` function to make a PDF without first exporting the HTML version.

### PDF output alternative

Download a precompiled binary from [wkhtmltopdf](https://wkhtmltopdf.org) and run your HTML document through the tool.

For example, if I really like the treatment Google has done to their logo today and want to capture it forever as a PDF:

```bash
wkhtmltopdf http://google.com google.pdf
```

Also checkout [HackMyResume](), a powerful tool to build and analyze your JSON Resume.
