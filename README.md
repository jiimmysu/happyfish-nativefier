# happyfish-nativefier(for MacOS)
Problem: Enable the Flash setting of browser when you everyday play happyfish Facebook desktop flash game.
Solve: Use nativefier to package the Facebook game url and build a mac application to prevent this problem. 
https://blog.user.today/electron-happyfish-flash-blocked/

## 1.Find the newest Adobe Flash Player version number.
Type this [chrome://components/](chrome://components/) in the address bar of Google Chrome.

## 2.Use the command below to generate mac application.
`nativefier --name "開心水族箱" "https://apps.facebook.com/happyfishbowl/?fb_source=bookmark_favorites&ref=bookmarks&count=0&fb_bmpos=_0" --flash --flash-path "/Users/XXXX/Library/Application Support/Google/Chrome/PepperFlash/32.0.0.223/PepperFlashPlayer.plugin" --inject ./style.css --icon ./icon.png`

* Replace the username(XXXX) and Adobe Flash Player version(32.0.0.223) of your own.

## 3.You will get a APP-darwin-x64 folder in your project folder.
## 4.Drag APP.app into the "Application" folder.(You can find "Application" on the sidebar of Finder.)