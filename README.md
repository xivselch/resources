# xivselch/static

This repository serves as the authoritative source for **static content** within the X|VSelch ecosystem. It contains official guides, documentation, legal policies, and curated external resources intended to support contributors, developers, and community members. All content applies to the services hosted at [emetselch.xyz](https://emetselch.xyz) and the wider suite of tools provided by the X|VSelch organisation.

The repository is maintained under version control to ensure clarity, transparency, and efficient management across the X\|VSelch ecosystem.

## Structure

Each subdirectory within the `content/` folder must include a `meta.json` file. This file provides essential metadata and configuration details, allowing automated tools and scripts to process, filter, and present the relevant files within each directory effectively.

A standard `meta.json` file is structured as follows:

```json
{
  "glob": "**/*.{md,mdx}",
  "external": [
    {
      "url": "https://v2.xivapi.com/docs/welcome/",
      "description": "Official XIVAPI v2 documentation",
    },
  ]
}
```

### Key Fields

- **`glob`**:  
  Specifies the [glob pattern](https://code.visualstudio.com/docs/editor/glob-patterns) used to select which files are included as part of the directory’s content set.  
  For example, `"**/*.{md,mdx}"` includes all Markdown (`.md`) and MDX (`.mdx`) files in the folder and its subfolders, enabling the automatic discovery and processing of documentation.

- **`external`**:  
  Takes an array of external resources—including links, documents, or reference materials—relevant to the directory's content.  
  This field is currently left empty (`[]`), but may later reference official documentation, third-party guides, or authoritative sources as required. This extensibility enables seamless integration between internal and external resources.

Repository maintainers may update the `content/**/meta.json` files to control the visibility and indexing of files, as well as supplement documentation with curated links to additional reading or references from reputable external sources.
