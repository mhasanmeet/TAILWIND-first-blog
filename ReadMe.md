# Design a blog with tailwindcss
----------

## Tailwind Installation
### For Tailwind we will use ---

* postcss
* Vite 

-- First we need to create a package Json file 
```
npm init -y 
```

-- Then we will install Tailwind by command 
```
npm install -D tailwindcss postcss autoprefixer vite
```

-- For tailwindcss configure
```
npx tailwindcss init -p
```

-- Then we create html and css file
-- Then we need to insert/include tailwindcss directive into stylesheet
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

-- Then we need to change package.json file scripts test section & updated as
```
"dev": "vite"
```

-- Then we need to change in tailwind config file, for catch tailwindcss in the html we need to define which file should be compiled. We define all html file will compiple as way as, 
```
content: ["*.html"]
```

-- Then if we run command as 
``` npm run dev 
```
we will get browser hotlink, like:
```
local: http://localhost:3000/
```

-- Then if we make change or use tialwindcss then will show in the browser.


### Design a blog with tailwindcss
#### For designing a blog with tailwind we will use, 

* google fonts 
* fontawesome 

-- If we want to use different font family then we need to change in tailwind config file, as

fontFamily section in extend, 

```
 theme: {
    extend: {
        fontFamily: {
           'poppins':  ['poppins', 'sans-serif'],
           'roboto': ['Roboto', 'sans-serif']
        }
    },
  },
```
------------------------

Remember something, 

-- As our project run on vite, the tailwind css can not get if we only click html file
-- for getting compiled css file we need to **

-- npm run build the files, for that

* first create a dist folder and create a css file where compiled css file will be build there
* then for build purpose we created a css file like "style.css" from outside dist folder, we need that file
* install tailwind globally as run command ```npm install -D tailwindcss```
* then buil file run command ```npx tailwindcss -i {compiled css file} -o {watch css file} --watch```
* then we get a compiled css file

----------------------------- 

More work todo 

* JavaScript functionality
* slider active
* CSS variable
* BEM style css
* Responsive media query


