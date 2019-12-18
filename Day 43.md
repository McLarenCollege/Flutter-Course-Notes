# Day 43

## Adding App Icons and Publishing on Play Store

### Creating app icon:
- [Using asset studio](https://romannurik.github.io/AndroidAssetStudio/icons-launcher.html#foreground.type=clipart&foreground.clipart=360&foreground.space.trim=1&foreground.space.pad=0.25&foreColor=rgba(96%2C%20125%2C%20139%2C%200)&backColor=rgb(68%2C%20138%2C%20255)&crop=0&backgroundShape=square&effects=none&name=ic_launcher)
- Using [Canva](https://www.canva.com/) (Size 512 by 512 px)

### Adding app icon to Flutter
- To add icon to Flutter we need to generate icons in different sizes 
[using asset studio](https://romannurik.github.io/AndroidAssetStudio/icons-launcher.html#foreground.type=clipart&foreground.clipart=360&foreground.space.trim=1&foreground.space.pad=0.25&foreColor=rgba(96%2C%20125%2C%20139%2C%200)&backColor=rgb(68%2C%20138%2C%20255)&crop=0&backgroundShape=square&effects=none&name=ic_launcher)

- In the downloaded folder, go to res and keep it open as we will need the content of these folders
- Now go to your flutter project, android -> app -> src -> main -> res -> mipmap-hdpi  