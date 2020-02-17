## How to integrate mdbootstrap with vuejs 2 LARAVEL 6

# REPLACE 

``` js
window.Vue = require('vue');
```

# With
``` js
import 'mdbvue/lib/css/mdb.min.css';
window.Vue = require('vue');
import * as mdbvue from 'mdbvue'
for (const component in mdbvue) {
    Vue.component(component, mdbvue[component])
}
```