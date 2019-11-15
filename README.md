# happyfish-nativefier(for MacOS)
- Problem: I must enable the Flash player setting of the browser everytime when I play Facebook desktop flash game "happyfish".
- Solution: Use nativefier to package the Facebook game page url and build a MacOS application to prevent this problem. 

https://blog.user.today/electron-happyfish-flash-blocked/

## 0.Find the newest Adobe Flash Player version number.
Type this `chrome://components/` in the address bar of Google Chrome.

## 1.Copy this Project, and run npm.
- `git clone https://github.com/jiimmysu/happyfish-nativefier.git`
- `npm install`

## 2.Use the command below to generate MacOS application.
`nativefier --name "開心水族箱" "https://apps.facebook.com/happyfishbowl/?fb_source=bookmark_favorites&ref=bookmarks&count=0&fb_bmpos=_0" --flash --flash-path "/Users/XXXX/Library/Application Support/Google/Chrome/PepperFlash/32.0.0.293/PepperFlashPlayer.plugin" --inject ./style.css --icon ./icon.png`

* Replace the username(XXXX) and Adobe Flash Player version(32.0.0.293) of your own.

## 3.You will get an "APP-darwin-x64" folder in your project folder.
## 4.Drag APP.app into the "Application" folder.
You can find "Application" on the sidebar of Finder.
