# TUTORIAL 2: INSTALL BOOTSTRAP 5

## STEP 1
- Open Terminal and run code
```
npm install bootstrap --save
```

## STEP 2
- Create **plugins/bootstrap.js**
- Copy and paste the following code
```
import 'bootstrap/dist/js/bootstrap.bundle.min.js';

export default defineNuxtPlugin(nuxtApp => {
  // You can add any global bootstrap initialization here
  console.log('Bootstrap is loaded!');
});
```

## STEP 3
- Create **app/assets/css/main.css**
- Copy and paste the following code
```
@import 'bootstrap/dist/css/bootstrap.min.css';

body {
    background-color: #EDF2F9;
}
```

## STEP 4
- Open file **nuxt.config.ts**
- Copy and paste the following code
```
export default defineNuxtConfig({
  compatibilityDate: '2025-11-13',
  devtools: { enabled: true },
  css: [
    'bootstrap/dist/css/bootstrap.min.css',
    '~/assets/css/main.css',
  ],
  build: {
    transpile: ['bootstrap'],
  },
  plugins: [
    { src: '~/plugins/bootstrap.js', mode: 'client' },
  ],
})
```

## STEP 4
- Save

#
[<< Prev](https://github.com/ajmalnorshawali/setup-nuxt3-bootstrap5/blob/main/Tutorial%201_%20Install%20Nuxt.md)
|
[Next >>](https://github.com/ajmalnorshawali/setup-nuxt3-bootstrap5/blob/main/Tutorial%203_%20Nuxt%20Views.md)
