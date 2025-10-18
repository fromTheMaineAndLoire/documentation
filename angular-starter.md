# Angular-starter

## New Project

```
ng new jewelery-front
```

### Component

```
ng generate component component-component
```


### Start server

```
ng serve
```

### Issues 

Issue when you are trying to reach http://localhost:42000/


```
import { bootstrapApplication, BootstrapContext } from '@angular/platform-browser';
.....
const bootstrap = (context: BootstrapContext) => bootstrapApplication(App, config, context);

```