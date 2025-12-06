# xivselch/resources

This repository collects **community resources** for the X|VSelch project, to help all FFXIV players find useful links and materials. It is not meant for technical documentation. Resources here support contributors, developers, and the wider FFXIV community using services at [emetselch.xyz](https://emetselch.xyz) and across Eorzea.

All resources are kept under version control for transparency and easy collaboration.

## Structure

Community resources are organised in subfolders. Each one contains a `meta.json` file with basic information so scripts and tools can use the links in a standard way.

A sample `meta.json` file looks like this:

```json
{
  "glob": "**/*.{md,mdx}",
  "external": [
    {
      "url": "https://v2.xivapi.com/docs/welcome/",
      "description": "Official XIVAPI v2 documentation"
    }
  ]
}
```

### Key Fields

- **`glob`**:  
  A [glob pattern](https://code.visualstudio.com/docs/editor/glob-patterns) that selects which files in the folder (for example, `.md` and `.mdx` guides or event posts) are included. These are community resources, not technical documents.

- **`external`**:  
  A list of useful links and short descriptions for external resources — such as official sites, community projects, or recommended FFXIV links — to help players further. This helps connect X|VSelch to the broader FFXIV community.

Repository maintainers may update or add `resources/**/meta.json` files to keep the list of resources helpful, easy to find, and current. The focus is always on supporting the FFXIV community and sharing useful resources, not maintaining official documentation.
