# happyfish-nativefier(for MacOS)
https://blog.user.today/electron-happyfish-flash-blocked/

## 1.Go to [chrome://components/](chrome://components/) to find Adobe Flash Player version.

## 2.Use the command below to generate mac application.
nativefier --name "開心水族箱" "https://apps.facebook.com/happyfishbowl/?fb_source=bookmark_favorites&ref=bookmarks&count=0&fb_bmpos=_0" --flash --flash-path "/Users/XXXX/Library/Application Support/Google/Chrome/PepperFlash/32.0.0.223/PepperFlashPlayer.plugin" --inject ./style.css --icon ./icon.png