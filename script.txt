"use strict";
 
const list = document.querySelector(`#list`);

const todos = [ `Lab 1`, `Lab 2`, `Learn DOM Manipulation`, `Look into jQuery`, `Lab 3` ];
 
function createListItem(input) {
	const item = document.createElement(`li`);
	const itemText = document.createTextNode(input);

	item.appendChild(itemText);
	list.appendChild(item);
}

function fillList() {
	var listText;
	for (var i = 0; i < todos.length; i++){
		listText = createListItem(todos[i]); 
	}; 
return listText;
}

// TODO: Loop over todos, create elements, and append them to the ul
