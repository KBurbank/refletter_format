# Refletter Format

## Installing



```bash
quarto use template kburbank/refletter
```

This will install the extension and create an example qmd file that you can use as a starting place for your letter.

## Using

Write your letter in a qmd file, and render it to pdf using the `refletter-pdf` format.

## Format Options



Some important fields need to be set either in the `_metadata.yml` file, or inline in the qmd file itself:

* `author_info`: Information about the author of the letter.
* `closing`: The closing of the letter.
* `logo-path`: The path to the logo of the letter.
* `signature-path`: The path to the signature of the letter.

For example,

```yaml
format:
  refletter-pdf: default
date: last-modified
logo-path: "logo.png"
signature-path: "signature.pdf"
closing: "Sincerely,"
author_info:
  name: "Your name"
  degree: "Your degree (e.g., PhD, MS, etc.)"
  position: "Your position (e.g., Assistant Professor, etc.)"
  department: "Your department"
  address: "Your address"
  cityzip: "Your city, zip code, country, etc"
  email: "Your email address"
  phone: "Your phone number"
```

