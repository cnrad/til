When working on my personal site, I encountered odd behavior where an absolutely-positioned child element would be positioned different if the parent had `filter: blur(...)` on it. After a bit of digging, I found [this](https://drafts.fxtf.org/filter-effects/#FilterProperty):

> A value other than none for the filter property results in the creation of a containing block for absolute and fixed positioned descendants unless the element it applies to is a document root element in the current browsing context.

Turns out, using `blur()` essentially wraps the element in a relatively positioned container (sort of), which was changing the positioning of the child div. TIL
