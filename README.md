![Image](/adhishlal.png)

# Android GIF Viewer/Loader 
Loading GIF files with animations have always been a challenge when we code for Android devices. Seeing this problem by most of the Android Developers across the globe, I thought of publishing a GIF loader library.

Now to load the GIF images into your Android Application, all you need to do is add a dependency to your app level gradle.build along with the jitpack configuration:

### Installing

1) Add it in your root build.gradle at the end of repositories:
```
	allprojects {
		repositories {
			...
			maven { url 'https://www.jitpack.io' }
		}
	}
```

2) Step 2. Add the dependency
```
	dependencies {
	        compile 'com.github.adhishlal:gifloader:1.1'
	}
```
Next, go to your XML file wherever you want to show the GIF file along with the animation and add the following widget
```
        <lal.adhish.gifprogressbar.GifView
            android:id="@+id/progressBar"
            android:layout_width="@dimen/_50sdp"
            android:layout_centerInParent="true"
            android:layout_margin="@dimen/_5sdp"
            android:layout_height="@dimen/_50sdp"
            android:layout_gravity="center" />
```
Once this is done, open your Java class where you are inflating the above widget’s layout and initialise this as shown below and also set the GIF image resource which you want to show:
```
GifView pGif = (GifView) findViewById(R.id.progressBar);
pGif.setImageResource(R.drawable.loader);
```
Bravo! You just did it.

Just compile and run your code.:thumbsup:

### Show Some :heart:
[![GitHub stars](https://img.shields.io/github/stars/badges/shields.svg?style=social&label=Star)](https://github.com/adhishlal/GifLoader)
[![GitHub forks](https://img.shields.io/github/forks/badges/shields.svg?style=social&label=Fork)](https://github.com/adhishlal/GifLoader/fork)
[![GitHub watchers](https://img.shields.io/github/watchers/badges/shields.svg?style=social&label=Watch)](https://github.com/adhishlal/GifLoader) 
[![GitHub followers](https://img.shields.io/github/followers/espadrine.svg?style=social&label=Follow)](https://github.com/adhishlal/)
[![Twitter Follow](https://img.shields.io/twitter/follow/espadrine.svg?style=social&label=Follow)](https://twitter.com/er_adhish)
