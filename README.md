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

Just compile and run your code.
