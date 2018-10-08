# Animatoo
A lightweight and easy to use Android library that provides many activity transition animations
⋅⋅* min SDK 16 (Android Jellybean 4.1)
⋅⋅* written in Java

A lightweight, easy-to-use Android library that provides awesome activity transition animations

To download the demo app for this library from Google Playstore so you can see it in action, click here:

## Installation

Add this into your root build.gradle file:

```java
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
Add the dependency to your module build.gradle:
```java
dependencies {
	        implementation 'com.github.mohammadatif:Animatoo:master'
}
```
## Usage
Animatoo has 15 different activity transition animations:

01. in and out.
02. swipe left.
03. swipe right.
04. split.
05. shrink.
06. card.
07. zoom.
08. fade.
09. spin.
10. diagonal.
11. windmill.
12. slide up.
13. slide down.
14. slide left.
15. slide right.

Using Animatoo is extremely simple, A single short line of code following startActivity(...) is all that's needed, for example:
```java
startActivity(new Intent(context, TargetActivity.class));
Animatoo.animateZoom(context);  //fire the zoom animation
```
Another example, this time firing the animation when the back button is pressed:
```java
@Override
public void onBackPressed(){
  super.onBackPressed();
  Animatoo.animateSlideLeft(context); //fire the slide left animation
}
```
All the available methods for this library:
```java
Animatoo.animateZoom(context);
Animatoo.animateFade(context);
Animatoo.animateWindmill(context);
Animatoo.animateSpin(context);
Animatoo.animateDiagonal(context);
Animatoo.animateSplit(context);
Animatoo.animateShrink(context);
Animatoo.animateCard(context);
Animatoo.animateInAndOut(context);
Animatoo.animateSwipeLeft(context);
Animatoo.animateSwipeRight(context);
Animatoo.animateSlideLeft(context);
Animatoo.animateSlideRight(context);
Animatoo.animateSlideDown(context);
Animatoo.animateSlideUp(context);

```
