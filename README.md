# Krunker.js 
<div align="center">
  <br />
  <p>
    <a href="https://krunker.io"><img src="https://i.imgur.com/qvTc8OA.png" width="546" alt="Krunker.js" /></a>
  </p>
  <br />
  <p>
    <a href="https://nodei.co/npm/krunker.js/"><img src="https://nodei.co/npm/krunker.js.png?downloads=true&stars=true" alt="npm installnfo" /></a>
  </p>
</div>
[![npm downloads](https://img.shields.io/npm/dt/krunker.js.svg?maxAge=3600)](https://www.npmjs.com/package/krunker.js) [![Dependencies](https://img.shields.io/david/xazgg/krunker.js.svg?maxAge=3600)](https://david-dm.org/xazgg/krunker.js.svg) [![RunKit](https://badge.runkitcdn.com/krunker.js.svg)](https://npm.runkit.com/krunker.js) [![NPM Version](https://img.shields.io/npm/v/krunker.js.svg?maxAge=3600)](https://www.npmjs.com/package/krunker.js)

###### [GitHub](https://github.com/xAzz) | [Discord](https://discord.gg/wB3P92h)

A simple, easy to use module for interacting with the [Krunker.io Social Page](https://krunker.io/social.html)

## Setup and Installation

```
$ npm i krunker.js
```

## Example Usage

```js
// Require the NPM Module
const KrunkerJS = require('krunker.js');
// Create a new instance
const Krunker = new KrunkerJS();

// Get the stats of the user
Krunker.getUser('Helinho').then(data => {
	// Console log the user stats as an object
	console.log(data);

	// Convert Player Score to Level
	Krunker.getLevel(data);
	// Convert Time Played
	Krunker.getPlayTime(data);
	// Get user KDR
	Krunker.getKDR(data);
	// Get W/L
	Krunker.getWL(data);
	// Get SPK
	Krunker.getSPK(data);
});
```

## Another Example

```js
// Require the NPM Module
const KrunkerJS = require('./index.js');
// Create a new instance
const Krunker = new KrunkerJS();

(async () => {
	// Get the stats of the user
	const user = await Krunker.getUser('Helinho');
	// Console log the user stats as an object
	console.log(user);
})();
```

## Help

If you don't understand something in the documentation, you are experiencing problems, or you just need a gentle
nudge in the right direction, please don't hesitate to join my [Development Server](https://discord.gg/wB3P92h).