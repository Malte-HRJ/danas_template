## 🚀 Project Structure

```text
/
├── public/
│   └── favicon.svg
├── src
│   ├── assets
│   │   └── astro.svg
│   ├── components
│   │   └── Welcome.astro
│   ├── layouts
│   │   └── Layout.astro
│   └── pages
│       └── index.astro
└── package.json
```

## NOTE til Dana

- components og layouts skal starte med stort bogstav
- pages starter med et lille bogstav
- et astro component/page/layout er bygget sådan her op:

```astro
/
---
//frontmatter, her skriver du den kode der skal køre når siden bliver bygget
// for eksempel hvis du importere components eller hente data
import MitSuperSejeComponent from "../components/MitSuperSejeComponent"
//eksempel
const listeAfData = ["Malte", "er", "Sej"]
---

<DIT_HTML_KODE class="whatever">
...
<MitSuperSejeComponent></MitSuperSejeComponent>
// du kan bruge curly braces til at køre "bygge kode". eks:
{listeAfData}
</DIT_HTML_KODE>

<style>
//din css kode / styling her.
.whatever{
    *styling*
}
// styling er scoped, så det css skrevet her gælder kun for ".whatever" i dette component
</style>

<script>
//her kan du skrive javascript kode
</script>
```

## 🧞 Commands

| `npm install` | Installs dependencies |
| `npm run dev` | Starter en lokal server (din hjemmeside) på urlen `localhost:4321` |
| `npm run build` | Build your production site to `./dist/` |
| `npm run astro -- --help` | Get help using the Astro CLI (CLI = command line interface) |

[Astros dokumentation](https://docs.astro.build)
