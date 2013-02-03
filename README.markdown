### NSString+JavaAPI

An NSString category that brings a Java-like string manipulation API to Objective-C

### Building

Nothing fancy here, just add the sources to your project and go.

### Usage

To use this code, you must do two things:

1.  `#import "NSString+JavaAPI.h"`.

2.  Pretend that you're coding in Java.
    

### Limitations

This category is not as powerful as the full-fledged Java string processing API.  In particular, 
split() only operates on string literals and does not support passing a regular-expression as 
in Java.  

Additionally, various methods from the Java String API that are less commonly used and/or that 
have close syntactic and semantic relatives in the standard NSString API are not included in this 
category.  

### FAQ

**_Why create a Java-like String API for Objective-C?_**<br />
Because having worked with both Java Strings and NSString's I found the latter to be lacking in some areas.  
For example, it should not be necessary to say `[str stringByTrimmingCharactersInSet:[NSCharacterSet whitespaceAndNewlineCharacterSet]]` 
when all I want to do is trim leading and trailing whitespace.  Saying `[str trim]` is simpler and more intuitive and less likely to leave you with carpal-tunnel.

**_Why should I use this library?_**<br />
Use this library if you've got experience with Java and find yourself occasionally frustrated by the more obtuse and/or verbose aspects of the standard NSString API.

**_Why should I NOT use this library?_**<br />
Don't use this library if you've never worked with Java, or if you're just plain happy with the standard NSString API's.

**_What are your license terms?_**<br />
Use this code if you want, otherwise don't.  That's it.  
