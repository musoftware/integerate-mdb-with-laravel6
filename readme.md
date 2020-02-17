// LARAVEL 6
// VUEJS 2


REPLACE 


window.Vue = require('vue');


With

import 'mdbvue/lib/css/mdb.min.css';
window.Vue = require('vue');
import * as mdbvue from 'mdbvue'
for (const component in mdbvue) {
    Vue.component(component, mdbvue[component])
}
