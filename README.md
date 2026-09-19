# Regcoffee LLC — website

Marketing site for Regcoffee LLC, which operates secure truck parking yards and
industrial outdoor storage near interstate corridors in Pennsylvania, New Jersey
and New York.

> ## Incomplete: this repository does not build
>
> It contains build configuration only. There is no `src/` directory, yet
> `index.html` loads `/src/main.tsx`, so `npm run build` fails at the TypeScript
> step. The application source was never committed.
>
> Two other things to resolve before publishing:
>
> - `index.html` sets both its canonical URL and `og:url` to
>   `https://www.regcoffe.com/`, spelled with one "e", while this repository is
>   named with two. Confirm which domain is live and make the two agree.
> - A repository named [`regcoffeenyc/www.regcoffe.com`](https://github.com/regcoffeenyc/Www.regcoffe.com)
>   exists but contains the GDSFF Media & Communications Bot, not Regcoffee
>   content. The similar names are easy to confuse.
>
> Last updated 4 September 2025.

## Stack

- React 18 with TypeScript
- Vite 5
- Tailwind CSS 3
- Deployed through Netlify, configured in `netlify.toml`

## Local development

```bash
npm install
npm run dev
```

The dev server will fail until `src/main.tsx` and the rest of the application
source are added.

## Notes

- `.github/workflows/jekyll-docker.yml` is a leftover GitHub starter workflow.
  This is a Vite project, not Jekyll, so that workflow does not apply.
