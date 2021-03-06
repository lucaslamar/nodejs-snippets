<!--
*** Obrigado por estar vendo o nosso README. Se você tiver alguma sugestão
*** que possa melhorá-lo ainda mais dê um fork no repositório e crie uma Pull
*** Request ou abra uma Issue com a tag "sugestão".
*** Obrigado novamente! Agora vamos rodar esse projeto incrível :D
-->

<!-- Insignias Markeplace 
[![Visual Studio Marketplace Version]()]()
[![Visual Studio Marketplace Installs]()]()
[![Visual Studio Marketplace Rating]()]()
![GitHub]()
-->

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://www.linkedin.com/in/lucas-lamar-531930102/">
    <img src="assets/belleEpoqueLogo.png" width="400px" alt="Logo">
  </a>

  <h3 align="center">NodeJs Snippets</h3>
</p>

<!-- ABOUT THE PROJECT -->

### Installation (Not yet possible)

To install an extension you can run **Command Pallete** using the command `Ctrl + Shift + P` or` Cmd + Shift + P`, type `Install Extensions` and finally give an` Enter`, done that search by BelleEpoque and you will find the extension 
**es6-nodejs-snippets**.

### Supported languages (file extensions)

- JavaScript (.js)

### Snippets info

Every space inside `{ }` and `( )` means that this is pushed into next line :)
`$` represent each step after `tab`.

_TypeScript_ has own components and own snippets. Use search or just type `ts` before every component snippet.

I.E. `tsrcc`

## Snippets

### Basic Methods

|  Prefix | Method                                              |
| ------: | --------------------------------------------------- |
|  `imp→` | `import moduleName from 'module'`                   |
|  `imn→` | `import 'module'`                                   |
|  `imd→` | `import { destructuredModule } from 'module'`       |
|  `ime→` | `import * as alias from 'module'`                   |
|  `ima→` | `import { originalName as aliasName} from 'module'` |
|  `exp→` | `export default moduleName`                         |
|  `exd→` | `export { destructuredModule } from 'module'`       |
|  `exa→` | `export { originalName as aliasName} from 'module'` |
|  `enf→` | `export const functionName = (params) => { }`       |
|  `edf→` | `export default (params) => { }`                    |
|  `fre>` | `array.forEach(currentItem => {})`                  |
|  `fof→` | `for(const item of object) {}`                      |
|  `fin→` | `for(const item in object) {}`                      |
|  `anfn→`| `(params) => {}`                      							|
|  `nfn→` | `const add = (params) => {}`                        |
|  `dar→` | `const [first, second] = [1,2]`                     |
|  `dob→` | `const {rename} = fs`                      					|
|  `sti→` | `setInterval(() => {});`                      			|
|  `sto→` 	| `setTimeout(() => {});`                      			|
|  `prom→` 	| `return new Promise((resolve, reject) => {});`    |
|  `thenc→`	| `.then((res) => {}).catch((err) => {});`          |
|  `met→` 	| `methodName = (params) => { }`                    |
|  `amet→`	| `async method(params) {}`                      		|
|  `constructor` | `constructor() {}`                      			|

### Console

| Prefix | Method                              |
| -----: | ----------------------------------- |
| `clg→` | `console.log(object)`               |
| `clo→` | `console.log("object", object)`     |
| `ctm→` | `console.time("timeId")`            |
| `cte→` | `console.timeEnd("timeId")`         |
| `cas→` | `console.assert(expression,object)` |
| `ccl→` | `console.clear()`                   |
| `cco→` | `console.count(label)`              |
| `cdi→` | `console.dir`                       |
| `cer→` | `console.error(object)`             |
| `cgr→` | `console.group(label)`              |
| `cge→` | `console.groupEnd()`                |
| `ctr→` | `console.trace(object)`             |
| `cwa→` | `console.warn`                      |
| `cin→` | `console.info`                      |

### Sequelize

| Prefix   | Method                                  |
| -----:   | -----------------------------------     |
| `cms→`   | `Create a Sequelize model`              |
| `ccms→`	 | `${1:columns}: Sequelize.${2:STRING}$3,`|
| `ccmss→` | `${1:column}: Sequelize.STRING$2`       |
| `ccmsi→` | `${1:column}: Sequelize.INTERGER$2`     |
| `ccmsf→` | `${1:column}: Sequelize.FLOAT$2`        |
| `ccmse→` | `${1:column}: Sequelize.ENUM$2`         	|

### MongoDB

| Prefix   | Method                              |
| -----:   | ----------------------------------- |
| `cfmoo→` | `Create a Moongoose model`        	 |

### Node.js

| Prefix | Method                              																													 |
| -----: | ----------------------------------- 																													 |
| `cfne→`| Creates a basic express file        																													 |
| `fcc→` | create file of class                																													 |
| `fcce→`| create a file of class with extends  																												 |
| `fgr→` | Creates routes.js                   																													 |
| `gr→`  | `${1:routes}.${2:get}('/${3:rotas}', ${4:Rota}Controller.${5:index});` 											 |
| `grp→` | `${1:routes}.${2:get}('/${3:rotas}/:${4:id}', ${5:Rota}Controller.${6:index});`							 |
| `grpm→`| `${1:routes}.${2:get}('/${3:rotas}/:${4:id}', ${5:midware} , ${6:Rota}Controller.${7:index});`|
| `grm→` | `${1:routes}.${2:get}('/${3:rotas}', ${4:middlewares} ${5:Rota}Controller.${6:index});`       |

## Node Components

### constructor

```javascript
constructor() {
	$1
	}

```

### cpro

```javascript
new Promise((resolve, reject) => {,
	let condition = false;
	if(condition) {
		resolve('data')
			} else {
			  reject('error')
		}
		})
```

### cfne

```javascript
const express = require('express');
  
const ${1:server} = express();,
      
${1:server}.use(express.json());,

const port = 3000;,
      
${1:server}.get('/', (req, res) => json({message: 'Hello World!'}));,
      
${1:server}.listen(port);
```

### fgr

```javascript
import { Router } from 'express';
			
const ${1:routes} = new Router();
	$2
			
export default ${1:routes};
```
### igr

```javascript
${1:app}.${2:get}('/${3:rotas}', (req, res) => {
	res.json({});
	});
```
### igrm

```javascript
${1:app}.${2:get}('/${3:rotas}', ${4:middleware} , (req, res) => {
	res.json({});
		});
```

### igrp

```javascript
${1:app}.${2:get}('/${3:rotas}/:${4:id}', (req, res) => {
	res.json({});
		});

```
### igrpm

```javascript
${1:app}.${2:get}('/${3:rotas}/:${5:id}', ${4:middleware}, (req, res) => {
	res.json({});
		});

```
### fcc

```javascript
class $TM_FILENAME_BASE {
	$1
	}
			
export default new $TM_FILENAME_BASE();

```
### fcce

```javascript
class $TM_FILENAME_BASE extends ${1:Class}  {
	$2
	}
			
	export default new $TM_FILENAME_BASE();
```

### cms

```javascript
import Sequelize, { Model } from 'sequelize';
			
class $TM_FILENAME_BASE extends Model {
	static init(sequelize) {
		super.init(
			{
			  $1
			},
			{ sequelize }
		);
			
		return this;
			}
	}
			
	export default $TM_FILENAME_BASE;
```

### cfmoo

```javascript
import mongoose from 'mongoose';
			
const ${1:ExemploSchema} = new mongoose.Schema({
			   
	});
			
export default mongoose.model(' $TM_FILENAME_BASE',  ${1:ExemploSchema});
```

### icgm

```javascript
${1:server}.use(req, res, next) => {
			
	next();
});
```

### icgme

```javascript
${1:app}.use(function(err, req, res, next) {
	console.error(err.stack);
	res.status(500).send('Algo Errado :/!');
});
```

### cgm

```javascript
function ${1:functionName} (req, res, next) => {
			
	next();
});

```

### ecgm

```javascript
function ${1:functionName} (req, res, next) => {
			
	next();
});
```

<!-- CONTRIBUTING -->

## Contribute

1. Make the _fork_ of the project (<https://github.com/lucaslamar/es6-nodejs-snippets/fork>)
2. Create a _branch_ for your modification (`git checkout -b feature/fooBar`)
3. Make _commit_ (`git commit -m '[FEAT] - Estrutura inicial do projeto'`)
4. _Push_ (`git push origin feature/fooBar`)
5. Create a new _Pull Request_

<!-- LICENSE -->

## license

Distributed under the MIT license. See `LICENSE` for more information.

<!-- CONTACT -->

## Contact

Lucas Lamar - [Github](https://github.com/lucaslamar) - **lucass.lamar@gmail.com**