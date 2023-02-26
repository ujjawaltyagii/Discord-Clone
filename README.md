# Discord-Clone
Created responsive Discord Website using Tailwind CSS, HTML and JavaScript.

## Set up
1. Fork this repository.
2. Clone it to your computer `` git clone https://github.com/your-username/Discord-Clone.git ``
3. Navigate to the project folder  ``cd Discord-Clone ``
4. (to run commands "nodejs" and "Tailwind" setup should be already installed) If not then, 

   (IGNORE step 5 if already installed)
5. first download Nodejs then 
-> create a folder and open it in VScode or any code editor

-> now open terminal in Vscode and type
   `` npm init`` 

-> in package name : ``tailwind_demo ``

-> in description  : ``Tailwind `` 

-> now just "enter" till terminal shows
     
![Untitled](https://user-images.githubusercontent.com/115401171/219952298-71df6150-0582-4156-bc1a-8fb6862a5a88.png)
Now in terminal type following commands (continuation of step 5)
`` npm i vite``

`` npm install -D tailwindcss postcss autoprefixer``

``npx tailwindcss init``

-> now create a file in same(parent folder) with name: ``postcss.config.js``

-> now paste below content in this ``postcss.config.js`` file:

```
 module.exports = {
  plugins: {
  tailwindcss: {},
    autoprefixer: {},
  }
} 
```

-> now in file ``tailwind.config.js`` (delete all previous data and paste :
```
/** @type {import('tailwindcss').Config} */

module.exports = { 
  content: ["*"], 
  theme: { <br>
    extend: {}, 
  }, <br>
  plugins: [],
}
``` 
-> now open file ``package.json``
-> in "scripts" in new line add
```
     "start": "vite"
```
-> now create a file ``main.css``
-> now add following code in ``main.css``
```     
     @tailwind base;
     @tailwind components;
     @tailwind utilities;
```
-> now create a file ``index.html`` and link css file in HEAD Tag

  e.g:
```
 <link rel="stylesheet" href="./main.css">
```
-> now in Terminal type : 
     ``npm start``
 
you will see this :

![img](https://user-images.githubusercontent.com/115401171/219953559-bb4e8ed2-142f-41ea-8d31-5e54395596da.png) 

-> now CLICK on this https link to start live server
