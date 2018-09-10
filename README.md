#Simple Vue transitions

##Installation 
###Adding via NPM
```console
    npm install netsells/vue-transitions -D
``` 
###Adding via Yarn
```console
    yarn add netsells/vue-transitions --dev
``` 
##Available transitions
### expand-down
```javascript
    import TransitionExpandDown from 'vue-transitions';
```
##Usage
```html
    <transition-expand-down>
        <component v-if="value" />
    </transition-expand-down>
```