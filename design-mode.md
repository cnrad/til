TIL there's a property on the `document` object named `designMode` that when toggled to "on"[^1], allows you to edit the entire document without having to hack around in the devtools panel. Pretty neat! 

Not sure how I missed this when I was messing around on websites with inspect element in middle school.

[^1]: It's a little interesting that "on" and "off" were chosen to be used instead of `true`/`false` - especially when the [designMode setter converts it to a boolean](https://html.spec.whatwg.org/#design-mode-enabled) anyways. If anyone happens to know why, let me know!



https://github.com/user-attachments/assets/f0d89af9-f463-4e06-bc8b-01439348c82e
