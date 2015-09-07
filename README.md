# node-merge-objects
Merge two objects and concatenate arrays that are values of the same object key.
## Installation
	npm install merge-objects --save
## Usage
	var merge = require('merge-objects');

	object1 = {a: 1, b: [2, 3]};
	object2 = {b: [4, 5], c: 6};

	result = merge(object1, object2);
	console.log(result); //logs {a: 1, b: [2, 3, 4, 5], c: 6}