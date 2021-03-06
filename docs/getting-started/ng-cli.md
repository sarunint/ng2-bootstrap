### Getting started with angular-cli
 
#### Installing angular-cli

*Important*: please check `angular-cli` version, it should be => "1.0.0-beta.16"

*Note*: you can skip this part if you already have application generated by `ng-cli` and webpack
  
```bash
npm i -g angular-cli
ng new my-app
cd my-app
ng serve
```

#### Adding ng2-bootstrap
 
 - install `ng2-bootstrap`
 ```bash
   npm install ng2-bootstrap --save
 ```
 
- open `src/app/app.module.ts` and add
```typescript
import { AlertModule } from 'ng2-bootstrap/ng2-bootstrap';
...

@NgModule({
   ...
   imports: [AlertModule, ... ],
    ... 
})
```

- open `src/app/app.component.html` and add
```
<alert type="success">hello</alert>
```

- and last thing you need is css, open `src/index.html` and add link to Bootstrap css
```html
<head>
  ...
  <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
</head>
```
