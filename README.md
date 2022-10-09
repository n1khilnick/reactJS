<h1 align="center">
    React - Parcel
    <p align="left" >
  <img src="https://github.com/n1khilnick/react-parcel/blob/master/react-gif.gif" alt="react" max-width="6%",min-width="6%" />
</p>
</h1>
 
<p align="right", width="100px", height="100px">
  <img src="https://github.com/n1khilnick/react-parcel/blob/master/react-parcel-gif-from-unscreen-transparent.gif" alt="react-parcel" />
</p>




## Getting Started

Create React apps with no build configuration with parcel

## Installing

### Steps to setup

###___Create React App  without using create-react-app (Instructions)____###
-----------------------------------------------------------------------------


**1. Make the directory :**

    mkdir <app-name>

**2. Crate package.json ;**
 
 ```
  cd <app-name>
 ```
 ```
  npm init
 ```
  
**3. Enter whatever you want to or else press enter key to skip.**
```
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

**4. Confirm "yes"** 
_____________________

**5. Go to the app folder and install followings :**
	
```git
 	npm i react
```
	
```git
 	npm i react-dom
```
```git
 	npm i parcel --save-dev          <!-- (saving as -developer) -->
```
 

**6. After installationn go to package.jsoon and add the this into the "scripts" :**

```json
"scripts": {
  "start":"parcel index.html",
  "stop":"parcel index.html",
}

```
 
**7. Go to the "app-name" folder and create "index.html" and insert following :**

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
	
**8. After this create "index.js" and insert following :**
		
```js
		import React from 'react';
		import ReactDOM from 'react-dom/client';
		import App from './App';

		const root = ReactDOM.createRoot(document.getElementById('root'));
		root.render(
			<App />
		);
	
```



**9. After This Crate "App.js" file  and paste following :**

```js
		import React from 'react'

		function App() {
		  return (
			<div>App</div>
		  )
		}

		export default App;
		
```
		
		
**10. Start the app using "npm start" .**
_________________________________________

**11. If the parcel causes any build error use the below command in the Git Bash or Unix Shell :**
 
```git
 <rm -rf .parcel-cache/*  		<--- (Remove all files in the given path recursively.)---->
```

**12. Start the app again.**
___________________________
