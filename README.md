## JSNOtify

> A small javascript snippet to push notifications under browser.

## Usage

> Of course for showing notifications.

## Test

> Paste the below script in your browser console to check it's functionality.

```js
function pushAPI() {
  if (!Notification) {
    alert('{ Code Up Your Ass }'); 
    return;
  }

  if (Notification.permission !== "granted")
    Notification.requestPermission();

  var notification = new Notification('', {
    icon: '', //put an image source here
    body: '', //enter your message
  });

  notification.onclick = function () {
    window.open('https://github.com/CodeDotJS/'); // change the link and put something else of your own.  
  };
}
```

## License

_NO_
