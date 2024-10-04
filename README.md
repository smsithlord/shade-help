# ShadeHelp
This is an library for creating individual or sequenced help text bound to generic elements on a page.

# Live Demo
https://smsithlord.github.io/shadehelp/

# Compatibility
Tested Working: Edge & Chrome on Windows

# Usage
See "index.html" for a full usage example.
```
const shade = new ShadeHelp();
shade.showHelp({
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