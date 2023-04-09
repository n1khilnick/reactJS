<h1 align="center">
    React <img src="https://github.com/n1khilnick/react-parcel/blob/master/react-gif.gif" alt="react",top ="-10px", width="27px",min-width="114px" />  Parcel  
<h1>
	
## Getting Started
#### Create React apps with no build configuration(without using create-react-app) using `parcel`.

<p align="center">
 
  <img src="https://github.com/n1khilnick/react-parcel/blob/master/react-parcel-gif-from-unscreen-transparent.gif" alt="react-parcel" />
</p>

## Installing

### Steps to setup


1. Make the directory :
```bash
mkdir <app-name>
```
2. Create package.json :
 
 ```bash
  cd <app-name>
  npm init
 ```
  
3. Enter whatever you want to or else press enter key to skip :
```bash
	package name: <package-name> 
	version: (1.0.0)
	description: <App-Description>
	entry point: (index.js) 
	test command: 
	git repository:
	keywords:
	author: <Your-Name>
	license: (ISC)
```

4. Confirm _"yes"_ 


5. Go to the app folder and install followings :

>install react
```bash
npm i react
```
>install react-dom
```bash
npm i react-dom
```
>now install parcel	
```bash
npm i parcel --save-dev          <!-- (saving as -developer) -->
```
 

6. After installationn go to package.jsoon and add the this into the _"scripts"_ :

```json
"scripts": {
  "start":"parcel index.html",
  "stop":"parcel index.html",
}

```
 
7. Go to the _"app-name"_ folder and create _"index.html"_ and insert following :

```html
		<!DOCTYPE html>  
		<html lang="en">
		<head>
			<meta charset="UTF-8">
			<meta http-equiv="X-UA-Compatible" content="IE=edge">
			<meta name="viewport" content="width=device-width, initial-scale=1.0">
 			<link rel="icon" href="https://github.com/n1khilnick/reactJS/blob/master/react-parcel.png" />
			<link rel="apple-touch-icon" href="https://github.com/n1khilnick/reactJS/blob/master/react-parcel.png" />
			<title>Document</title>
		</head>
		<body>

			<div id="root"></div>
			<script src="index.js" type="module">
			</script>
			
		</body>
		</html>
```	
	
8. After this create _"index.js"_ and insert following :
		
```js
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
	<App />
);
	
```



9. After This Crate _"App.js"_ file  and paste following :

```js
import React from 'react';

   function App() {
	return (
	<div>App</div>
	)
   }

export default App;		
```
		
		
10. Start the app using :
 
```bash
npm start
```

11. If the parcel causes any build error use the below command in the Git Bash or Unix Shell :
 
```bash
 <rm -rf .parcel-cache/*  		<---- Removes all files in the given path recursively ---->
```

12. Start the app again.

---

