FastJson Retrofit Converter
===================

Retrofit ships with support for OkHttp's `RequestBody` and `ResponseBody` types but the library is
content-format agnostic. This modules contained herein are additional converters for JSON which uses FastJson.
For more information please see [the website][1].

Download
--------

###  Gradle:
#### dependency:
Add it in your root build.gradle at the end of repositories:
```groovy
allprojects {
		repositories {
			...
			maven { url "https://jitpack.io" }
		}
	}
```

 *For fastjson-android:*
```groovy
compile 'com.github.d0calv1n:retrofit-converter-fastjson:2.3.0'
```

Usage
-------
FastJson Retrofit Converter requires at minimum Java 7 or Android 2.3.
To use, supply an instance of your desired converter when building your `Retrofit` instance.

```java
Retrofit retrofit = new Retrofit.Builder()
  .baseUrl("https://api.example.com")
  .addConverterFactory(FastJsonConverterFactory.create())
  .build();
```

License
=======
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

 [1]: http://square.github.io/retrofit/
 [2]: https://bintray.com/ligboy/maven/retrofit-converter-fastjson/_latestVersion
 [3]: https://bintray.com/ligboy/maven/retrofit-converter-fastjson-android/_latestVersion
