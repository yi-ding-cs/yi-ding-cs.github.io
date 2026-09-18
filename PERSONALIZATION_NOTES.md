# Yi Ding academic website — setup notes

This repository has been personalized from the Academic Pages template using the supplied LaTeX CV.

## Already configured

- Site identity: Dr. Yi Ding
- GitHub Pages URL: `https://yi-ding-cs.github.io`
- GitHub account/repository assumption: `yi-ding-cs/yi-ding-cs.github.io`
- Google Scholar: configured from the CV
- Email: configured from the CV
- Main sections: Research, Publications, Teaching & Mentoring, Talks, Service, CV
- LaTeX CV source: `files/Yi_Ding_CV.tex`

## Recommended final touches

1. Add a professional headshot under `images/profile.jpg` and set `author.avatar: "profile.jpg"` in `_config.yml`.
2. Add your LinkedIn username to `author.linkedin` if desired.
3. Add ORCID / ResearchGate / Semantic Scholar identifiers if desired.
4. For each publication, optionally add DOI / paper / code links. The current publication list mirrors the supplied CV and links to Google Scholar for the live record.
5. If your GitHub Pages repository is not `yi-ding-cs/yi-ding-cs.github.io`, change `url` and `repository` in `_config.yml`.

## Deploy

Push the repository contents to the GitHub repository named `yi-ding-cs.github.io`. GitHub Pages should build the site through the repository's configured Pages workflow/settings.

## Local preview

The template uses Jekyll. With Ruby/Bundler installed, run:

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open the local address printed by Jekyll.
