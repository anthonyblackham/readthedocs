### mkdocs.yml

This is a default mkdocs.yml:

```
site_name: My Docs
```

You can get a list of your pages

```
cd repo.wiki.git
ls > pages.txt
```

Final result:

```
# Project information
site_name: 'Read the Docs'
site_description: 'Documentation using MkDocs with the Read the Docs theme'
site_author: 'Anthony Blackham'
site_url: 'https://anthonyblackham.com/readthedocs'

# Repository
repo_name: 'readthedocs'
repo_url: 'https://github.com/anthonyblackham/readthedocs'
edit_uri: 'edit/main/docs/'

# Copyright
copyright: 'Copyright &copy; 2020 Anthony Blackham'

# Configuration
theme:
  name: 'readthedocs'
  language: 'en'

# Pages
pages:
- Home: index.md
- Installation: Installation.md
- Getting Started: Getting-Started.md
- Style Guide: Style-Guide.md
- Configuration: Configuration.md
- Deploy: Deploy.md
```
