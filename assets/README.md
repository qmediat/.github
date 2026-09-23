# Brand assets

The Quantum Media Technologies wordmark used in the README of every published qmediat package, cropped from the
official 2024 brand kit (full company name, web variants), untouched apart from the viewBox and an accessible label.

| file | for |
|---|---|
| `qmediat-wordmark-dark.svg` | light backgrounds (the `<img>` fallback: npm, PyPI, GitHub light mode) |
| `qmediat-wordmark-light.svg` | dark backgrounds (`<source media="(prefers-color-scheme: dark)">` on GitHub) |

Markup every package README uses:

```html
<p align="left">
  <a href="https://www.qmediat.io/open-source?utm_source=oss-readme&utm_medium=<package>&utm_campaign=open-source">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/qmediat/.github/main/assets/qmediat-wordmark-light.svg">
      <img src="https://raw.githubusercontent.com/qmediat/.github/main/assets/qmediat-wordmark-dark.svg" alt="Quantum Media Technologies" height="40">
    </picture>
  </a>
</p>
```

The files are referenced by absolute URL because npm and PyPI do not resolve relative image paths. The brand colours are
`#e73735` (mark) and `#2e2e2d` (wordmark on light backgrounds).
