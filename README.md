Git Submodule based template repository for the [Ananke theme](https://github.com/gohugo-ananke/ananke) for [GoHugo](https://gohugo.io/).

## Versions

- [Install Ananke as Hugo Module](https://github.com/gohugo-ananke/template-hugo-mod)
- **[Install Ananke as Git Submodule](https://github.com/gohugo-ananke/template-git-submod) - this repository**

## Requirements

1. [Install Hugo](https://gohugo.io/installation/linux/) (extended or extended/deploy edition, 0.128.0 or later)
2. [Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Use this repo as a template

- Click the "Use this template" button at the top of this page to create a new repository based on this template.
- Clone this new repository to your local machine:

  ```bash
  git clone --recurse-submodules https://github.com/username/reponame.git # <-- replace username and reponame with your repository path
  ```
    
Or follow the instructions below to install Ananke as a Git submodule in an existing Hugo site.

## Installation of Ananke as a Git submodule

To install or create a Hugo website from scratch with the Ananke theme using the submodule method, follow these steps:

Verify that you have installed Hugo 0.128.0 or later.

```bash
hugo version
```

Create the project structure `quickstart` directory:

```bash
hugo new site quickstart
```

Change into the newly created directory:

```bash
cd quickstart
```

Initialize Git in the current directory:

```bash
git init
```

Clone the theme into the `themes` directory, adding it to your project as a [Git submodule].

```bash
git submodule add https://github.com/gohugo-ananke/ananke.git themes/ananke
```

Append a line to the site configuration file, indicating the current theme.

```bash
echo "theme = 'ananke'" >> hugo.toml
```

Start Hugo's development server to view the site.

```bash
hugo server
```

Running this command will start the development server and you can see your website at <http://localhost:1313/>. To stop the development server press `Ctrl + C`.

So set up details like comment system follow the steps in the [Ananke theme's getting started guide](https://github.com/gohugo-ananke/ananke#getting-started).
