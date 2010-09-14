#NSTimer+TIAdditions
*Super-simple NSTimer category to fire and reset the timer*  

Tim Isted  
[http://www.timisted.net](http://www.timisted.net)  
Twitter: @[timisted](http://twitter.com/timisted)

##License
NSTimer+TIAdditions is offered under the **MIT** license.

##Summary
`NSTimer+TIAdditions` is a category on `NSTimer` to add functionality to fire and reset the timer date.

In a Twitter client, for example, you might have a timer that checks for new tweets every 2 minutes. If the user requests a timeline refresh manually, you can call `ti_fireAndAdjustDate` to fire the timer immediately, then reset the timer such that it next fires 2 minutes after the current time.

The category adds two methods:

* `ti_fireAndAdjustDate`, which immediately fires the timer, then resets the next fire date based on the timer's `timeInterval`.
* `ti_adjustDateWithoutFiring`, which just resets the next fire date.