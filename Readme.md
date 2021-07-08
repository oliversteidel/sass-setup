# How to setup sass quickly
---

## 1. Setup sass using PARCEL <br><br>

### 1.1. Init project<br>
    npm init
creates package.json

### 1.2. Install the latest version of Dart sass <br>
    npm install sass -D
installs dart sass as Devdependency <br>
[Dart sass documentation](https://sass-lang.com/documentation)

### 1.3. Install parcel <br>
    npm install parcel-bundler -D
installs parcel as Devdependency <br>    
[Parcel Documentation](https://parceljs.org/getting_started.html)   

### 1.4. Create starter files and setup parcel <br>
- create main.scss
- create index.html and link to the **main.scss** to tell Parcel that you're writing sass
- go into package.json and change the "scripts" value to<br><br>

```js
"scripts": {
    "dev": "parcel src/index.html",
    "build": "parcel build src/index.html"
  },
```

### 1.5. Run Parcel<br>
    npm run dev

- Parcel watches your changes to your index.html and main.scss
- it creates a /dist folder and compiles your scss into css
- it opens a dev-server
- to stop parcel type: <kbd>ctrl</kbd> + <kbd>c</kbd>

### 1.6. Ready for production<br>

    npm run build

- Parcel builds your projectfor production and optimizes the compiled css with autoprefixes, cssnano ,etc.
- this is much slower than the "run dev" compiling 




