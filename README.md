# Commands

Spectral theme: https://themes.gohugo.io/themes/spectral/
Github: https://github.com/sbruder/spectral

### 1. Create a new site:
   
`hugo new site <name of site>`
`cd <name of site>`

### 2. Add theme as submodule

`git submodule add --depth=1 https://github.com/sbruder/spectral.git themes/spectral`
###### => Init:
`git submodule update --init --recursive`
###### => Update: 
`git submodule update --recursive --remote`

###### Updating theme:

`hugo mod get -u`

### 3. Adding modules

###### Only first time (init my code as module too):
`hugo mod init github.com/sparkerlewis/<NAME_REPO>`

###### Add module: 
`hugo mod get -u github.com/gethugothemes/hugo-modules/videos`

Add On config.toml:

```
[module]
  [[module.imports]]
    path = "example.com/theme-repository"
```

###### delete module :
Si vous souhaiter supprimer un module, vous pouvez utiliser la commande hugo mod tidy. Cela supprimera les modules non utilisés et les dépendances inutilisées.

`hugo mod tidy`


### Deployment:

Deployment with github pages: https://pages.github.com/
