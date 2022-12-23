When creating the menu, I decided to get rid of the idea of ​​breakpoints to hide the main menu and show the burger menu.
To do this, I decided to use the innerWidth property of the window. In the original version, the checkScreen() function,
which determined the screen extension was written in the created() lifecycle hook, but it turned out that when changing the width of the browser window
 the checkScreen() function does not work correctly (the variable into which the current screen extension is written does not change,
but retains its original value). To fix, an event listener was added: window.addEventListener("resize", this.checkScreen)

# relvise

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
