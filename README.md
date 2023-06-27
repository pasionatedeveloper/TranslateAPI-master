[//]: # (# TranslateAPI)

[//]: # (Simple Java library to translate your text using Google Translate without using of API KEY)

[//]: # ()
[//]: # (# Screenshot)

[//]: # (![alt text]&#40;https://raw.githubusercontent.com/iammannan/TranslateAPI/master/demo2.webp&#41;)

[//]: # ()
[//]: # (# Download)

[//]: # ()
[//]: # (* Step 1. Add it in your root build.gradle at the end of repositories:)

[//]: # (```java)

[//]: # (    allprojects {)

[//]: # (        repositories {)

[//]: # (          ...)

[//]: # (          maven { url 'https://jitpack.io' })

[//]: # (        })

[//]: # (    })

[//]: # (```)

[//]: # (* Step 2. Add the dependency)

[//]: # (```java)

[//]: # (   dependencies {)

[//]: # (	        implementation 'com.github.iammannan:TranslateAPI:1.1')

[//]: # (	})

[//]: # (```)

[//]: # (  * Full Code - Example)

[//]: # (  ```java)

[//]: # (    	TranslateAPI translateAPI = new TranslateAPI&#40;)

[//]: # (                        Language.AUTO_DETECT,   //Source Language)

[//]: # (                        Language.TAMIL,         //Target Language)

[//]: # (                        "Your Text"&#41;;           //Query Text)

[//]: # ()
[//]: # (                translateAPI.setTranslateListener&#40;new TranslateAPI.TranslateListener&#40;&#41; {)

[//]: # (                    @Override)

[//]: # (                    public void onSuccess&#40;String translatedText&#41; {)

[//]: # (                        Log.d&#40;TAG, "onSuccess: "+translatedText&#41;;)

[//]: # (                        textView.setText&#40;translatedText&#41;;)

[//]: # (                    })

[//]: # ()
[//]: # (                    @Override)

[//]: # (                    public void onFailure&#40;String ErrorText&#41; {)

[//]: # (                        Log.d&#40;TAG, "onFailure: "+ErrorText&#41;;)

[//]: # (                    })

[//]: # (                }&#41;;)

[//]: # ( ```)

[//]: # (![alt text]&#40;https://raw.githubusercontent.com/iammannan/TranslateAPI/master/demo1.png&#41;)

[//]: # ()
