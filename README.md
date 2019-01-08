# SuperBadge
SuperBadge Android Library 
Android Library to display ratings and other information in a beautiful badge!!
[![](https://jitpack.io/v/JP1016/SuperBadge.svg)](https://jitpack.io/#JP1016/SuperBadge)
![enter image description here](https://i.imgur.com/IvGIhbB.jpg)



# Gradle
**Step 1.** Add the JitPack repository to your build file
```
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
**Step 2.** Add the dependency
```
dependencies {
     implementation 'com.github.JP1016:SuperBadge:v1'
	}
```

## Maven
**Step 1.** Add the JitPack repository to your build file
```markup
	<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>
```
**Step 2.** Add the dependency
```markup
<dependency>
	    <groupId>com.github.JP1016</groupId>
	    <artifactId>SuperBadge</artifactId>
	    <version>v1</version>
</dependency>
```

## Usage
**XML**
```markup

<com.devzstudio.superbadge.SuperBadge
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:id="@+id/badge"
    app:sb_primaryText="Netflix"
    app:sb_secondaryText="Streaming App"
    app:sb_image="https://media.netflix.com/dist/img/meta-image-netflix-symbol-black.png"
    app:sb_tertiaryText="9.5"
    app:sb_tertiaryTextColor="#FF292A"/>
``` 

**Java**
```
        //Init
        SuperBadge sb=findViewById(R.id.badge);

        //Callback
        sb.setOnBageClickListener(new SuperBadge.OnBadgeClickListener() {
            @Override
            public void onBadgeClick() {

                Toast.makeText(SampleActivity.this, "Clicked on Badge", Toast.LENGTH_SHORT).show();

            }
        });

```

**Kotlin**
```
  //Init
   val sb = findViewById<SuperBadge>(R.id.badge)
  
  //Callback
  sb.setOnBageClickListener { Toast.makeText(this@SampleActivity, "Clicked on Badge", Toast.LENGTH_SHORT).show() }
  
  ```
**Contact**
```
 For any queries mail me at emast007@gmail.com
 Feel free to customize 
 Notify us to feature your app here , free github backlink for your app 