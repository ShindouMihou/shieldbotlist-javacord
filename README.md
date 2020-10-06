[![](https://jitpack.io/v/ShindouMihou/shieldbotlist.svg)](https://jitpack.io/#ShindouMihou/shieldbotlist)
# Shield Bot List API (for Java)
This is an unofficial API built for Java users, feel free to improve it as much as you like.
It will be maintained by me for the meantime, but I will be accepting pull requests if ever there is a need for one.

How to install?

**Maven**

Add the jitpack.io repository.
```	<repositories>
		<repository>
		    <id>jitpack.io</id>
		    <url>https://jitpack.io</url>
		</repository>
	</repositories>```
  
Add the dependency.
```	<dependency>
	    <groupId>com.github.ShindouMihou</groupId>
	    <artifactId>shieldbotlist</artifactId>
	    <version>v1.0</version>
	</dependency>```

**Gradle**
Add it in your root build.gradle at the end of repositories:

	```allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}```
  
Step 2. Add the dependency

	```dependencies {
	        implementation 'com.github.ShindouMihou:shieldbotlist:Tag'
	}```
  
How to use:
```ShieldBotApi sbh = new ShieldBotApi("token", clientID);
sbh.setServerCount(int)```

Replace int with the server count, choose how you like, for example in Javacord:
```
    public static void setupDBL(DiscordApi bot, String token, long clientID) {
    ShieldBotApi sbh = new ShieldBotApi("token", clientID);
    sbh.setServerCount(bot.getServers().size());
    }
```
