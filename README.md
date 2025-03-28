A single-page, one-column resume for software developers. It uses the base latex templates and fonts to provide ease of use and installation when trying to update the resume. The different sections are clearly documented and custom commands are used to provide consistent formatting. The three main sections in the resume are education, experience, and projects.

### Motivation

I created this template as managing a resume on Google Docs was hard and changing any formatting was too difficult since it had to be applied in multiple places.

Most currently available templates either focus on two columns, or are multiple pages long that didn't work well for career fairs or online applications.

### Quick start

Get started quickly using [Overleaf](https://www.overleaf.com/latex/templates/software-engineer-resume/gqxmqsvsbdjf) template.

### Build using Docker

```sh
docker build -t latex .
docker run --rm -i -v "$PWD":/data latex pdflatex nguyen_hoan_thien_resume.tex
```

### Preview
Generate PNG file for preview

```sh
docker run --rm -i -v "$PWD":/data dpokidov/imagemagick convert -density 300 /data/nguyen_hoan_thien_resume.pdf -quality 90 -background white -alpha remove -alpha off /data/HoanThien-Nguyen-CV.png
```

![Resume Screenshot](/HoanThien-Nguyen-CV-0.png)

### License

Format is MIT but all the data is owned by Sourabh Bajaj.
