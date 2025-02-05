[![](https://jitpack.io/v/ivankostadinovic/ComposeZoomableImage.svg)](https://jitpack.io/#ivankostadinovic/ComposeZoomableImage)

# ComposeZoomableImage

Forked from https://github.com/umutsoysl/ComposeZoomableImage for my own purposes. 
- Scroll support
- Double-tap zoom
- More optional parameters for better vesatility

# Demo

<img src="gif/demo.gif" width="270" height="500"/>


# Setup

```implementation 'com.github.ivankostadinovic:ComposeZoomableImage:<latest-version>'```

# Usage

```kotlin
 // in case you are using a bitmap
 val painter = BitmapPainter(bitmap)

 // image url - with coil library
 val painter = rememberAsyncImagePainter("https://imgrosetta.mynet.com.tr/file/12220872/12220872-1200x824.jpg")

 // resource drawable
 val painter = painterResource(id = R.drawable.compose)

 ZoomableImage(
            painter = painter,
            isRotation = false,
            modifier = Modifier.fillMaxWidth().size(250.dp),
            scrollState = scrollState // if you are using this image inside a scrollable component
        )

```


License
--------
    Copyright 2021 Umut Soysal.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
