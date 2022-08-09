# Full Responsive

> [Responsive design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design#responsive_design) = [Fluid design](https://blog.hubspot.com/website/fluid-design) + [Adaptive design](https://www.invisionapp.com/defined/adaptive-design)

The final solution for a _full responsive_ design. With this package you will easily program liquid/fluid designs as well as adaptive designs from your design to your app in the most straightforward way possible.

### Fluid design
![fluid design example](https://img.favpng.com/23/16/10/responsive-web-design-vector-graphics-electronic-media-illustration-euclidean-vector-png-favpng-MZMSfBRQ3J9jt8BsX3viNYDEJ.jpg)

On fluid (or liquid) designs, you lay out widgets defining with proportions their sizes. 
### Adaptive design
![adaptive design example](https://marketing.invisionapp-cdn.com/cms/images/lr1orcar/marketing-pages/012ecee36138fcb5d0ea06eda0c81ba6ef61f251-851x565.png?w=2000&fm=jpg&q=90)
On adaptive design you program a specific UI for every screen size

## How to use

Define in your app this
```dart
main(){
    FullResponsiveApp(
        resolutions:[
            Resolution(844,390),
            Resolution(1024,768),
        ]
    )
}
```
For every screen your app has define:
```dart
class ScreenFoo extends StatelesWidget{
    @override
    Widget build(BuildContext context){
        return FullResponsiveScreen(
            
        );
    }
}
```
## Design resolution sizes advice.

When you design it's a good practice to take in consideration [the most popular resolutions used](https://gs.statcounter.com/screen-resolution-stats/desktop/worldwide) as well as the [IOS device sizes](https://www.ios-resolution.com/). For that we suggest you use one of the following sizes:
 - small: **390x844**
 - medium: **1024x768**
 - big: **1920x1080**