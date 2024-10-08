# ShadeHelp
This is a library for creating individual or sequenced help text bound to generic elements on a page.

# Live Demo
![Screenshot](/meta_image.jpg?raw=true "Screenshot")
https://smsithlord.github.io/shade-help/

# Compatibility
Tested Working: Edge & Chrome on Windows

# Usage
See "index.html" for a full usage example.
```
const shade = new ShadeHelp();
shade.showHelp({
	element: document.querySelector('#myContent'),
	helpInfo: {
		label: 'Label Text Here',
		content: 'Label body text here.'
	}
});
shade.on('advance', ()=>{
	console.log('User desires to advance the help sequence...');
	console.log('We have no more help to show, so just destroy ourselves.');
	shade.destroy();
});
```
# License
Released under the MIT License. See LICENSE for details.