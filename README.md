# Slack Black Theme

A darker, more contrasty, Slack theme.

# Installing into Slack

Mac OS:
1. Open `/Applications/Slack.app/Contents/Resources/app.asar.unpacked/src/static/ssb-interop.js`
2. At the very bottom, add
```js
document.addEventListener('DOMContentLoaded', function() {
  $.ajax({
   url: 'https://raw.githubusercontent.com/NesterovichAlexey/Slack-Theme/master/custom.css',
   success: function(css) {
     $("<style></style>").appendTo('head').html(css);
   }
 });
});
```
3.That's it! Restart Slack and see how well it works.

NB: You'll have to do this every time Slack updates.

Clone https://github.com/widget-/slack-black-theme
