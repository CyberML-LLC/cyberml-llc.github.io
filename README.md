# cyberml.ai

Website for CyberML — applied AI consulting (Generative AI, LLMs, RAG, multi-agent systems and evaluation).

A single static page (`index.html`) served by GitHub Pages. No build step.

## Structure

```
index.html        the site
assets/logo.jpg   logo, favicon and social preview image
.nojekyll         serve files as-is (skip Jekyll)
```

## Contact form

The form posts to [FormSubmit](https://formsubmit.co), which forwards each message to the CyberML inbox. The first submission sends a one-time activation email to that inbox; click the link in it to start receiving messages. After activation, FormSubmit gives you a random alias string you can put in the form's `action` URL in place of the email address, so the address no longer appears in the page source.

## Custom domain

To serve the site at `cyberml.ai`:

1. In the repo, go to **Settings → Pages → Custom domain** and enter `cyberml.ai`. (This adds a `CNAME` file.)
2. At your DNS provider, point the apex domain at GitHub Pages with four `A` records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`. Add a `CNAME` record for `www` pointing to `cyberml-llc.github.io`.
3. Once DNS resolves, tick **Enforce HTTPS**.
