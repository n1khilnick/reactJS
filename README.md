<h1 align="center">
    React - Parcel
</h1>

![react-parcel](https://cdn-images-1.medium.com/max/2000/1*gCNh33wfDRiSaBc_qv4h7g.png)

###___Create React App  without using create-react-app (Instructions)____###
-----------------------------------------------------------------------------

1.Go to the <react-app> directory

2.Make the directory :

    mkdir <app-name>

3.Crate package.json ;

  cd  <app-name>
  npm init
  
4.Enter whatever you want to or else press enter key to skip.

package name: (pokemonapi) <br>
version: (1.0.0) <br>
description: <App-Description> <br>
entry point: (index.js) <br>
test command: <br>
git repository:<br>
keywords:<br>
author: <Your-Name> <br>
license: (ISC)

5.Confirm "yes" 

6.Go to the app folder and install followings :

 npm i react
 npm i react-dom
 npm i parcel --save-dev          (saving as -developer)
 
 

7.After installationn go to package.jsoon and add the this into the "scripts" :

	"start":"parcel index.html",
	"stop":"parcel index.html",

 
8.Go to the <app-name> folder and create "index.html"

and insert following :


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
	
	
9.After this create "index.js" and insert following :

		import React from 'react';
		import ReactDOM from 'react-dom/client';
		import App from './App';

		const root = ReactDOM.createRoot(document.getElementById('root'));
		root.render(
			<App />
		);




10.After This Crate "App.js" file  and paste following :

		import React from 'react'

		function App() {
		  return (
			<div>App</div>
		  )
		}

		export default App;
		
		
11.Start the app using "npm start" .

12.If the parcel causes any build error use the below command in the Git Bash or Unix Shell :

  rm -rf .parcel-cache/*            (Remove all files in the given path recursively.)
  
  
13.Start the app again.
