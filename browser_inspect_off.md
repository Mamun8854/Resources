## Inspect element disable
```javascript
document.addEventListener('contextmenu', function (event) {
        event.preventDefault();
    });
```
## Check for F12 key press event
```javascript
    document.addEventListener('keydown', function(event) {
        if (event.keyCode == 123) { // F12 key code
            event.preventDefault(); // Prevent default browser behavior
            alert("Opening developer tools is not allowed."); // Display a message
        }
        if (event.shiftKey && event.ctrlKey && event.keyCode == 73) { // Shift + Ctrl + I
            event.preventDefault(); // Prevent default browser behavior
            alert("Opening developer tools is not allowed.");
        }
    });
```
