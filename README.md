# Joy Akinleye — Cloud & DevOps Portfolio

A responsive personal portfolio built with HTML, CSS and vanilla JavaScript.

## Project structure

```text
joy-devops-portfolio/
├── index.html
├── styles.css
├── script.js
├── assets/
│   └── Joy_Oluwafunmiso_Akinleye_DevOps_CV.pdf
└── README.md
```

## Add the CV PDF

Copy the public-safe CV PDF into the `assets/` folder and name it exactly:

`Joy_Oluwafunmiso_Akinleye_DevOps_CV.pdf`

The CV link in `index.html` points to that path. If you choose a different filename, update the link too.

## Run locally

No build tools or package installation are required.

From this directory, run:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser. Stop the local server with `Ctrl+C`.

You can also open `index.html` directly, but using a local HTTP server is a better test of links and browser behaviour.

## Check before publishing

- Test the navigation on desktop and phone widths.
- Open both GitHub and LinkedIn links.
- Test the email link.
- Add the CV PDF and test View / Download CV.
- Check that all project descriptions reflect work you actually completed.
- Do not add private keys, passwords, AWS credentials or `.env` files to this repository.

## Current scope

This is the first website milestone: homepage, About, Skills, Projects, experience, CV link and Contact. Docker, EC2 deployment and GitHub Actions CI/CD will be added in later stages.
