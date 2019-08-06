# where_to_go
An angular project

## Notes: how to get Angular-APP runable in GitHubPage
1. `ng build` the angular project *where to go* source-code in a repository;
2. setup a new project/repository in GitHub with the same name *where_to_go*, upload the builded App into the project (either in root or in `/docs` folder);
3. in "setting"-"GitHub Pages" choose the publich source accordingly (if the builded App was uploaded into root, then in "Source" choose "master branch"; if uploaded into `/docs` then choose "master branch /docs folder");
4. add `/where_to_go/` at all `src` or `href` attributes in *index.html* (because the app will be called from \https://*.github.io/NAME_of_Project_or_Repository/): e.g.
```
    <head>
        ...
        <base href="/where_to_go/">
        ...
        <link rel="stylesheet" href="/where_to_go/styles.5dcff8311d083158376a.css">
    </head>
    <body>
        <script src="/where_to_go/runtime-es2015.858f8dd898b75fe86926.js" type="module"></script>
        ...
    </body>
```
5. create a *404.html* with the same content of *index.html*
6. the App will be runable at URL https://zhangsorcerer.github.io/where_to_go/ (*where_to_go* is the name of the project and repository in GitHub) 
