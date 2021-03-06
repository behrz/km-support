---
layout: post
title: Events - Clicks On
categories: [tools, event-library]
author: Eric Fung
summary: Trigger events when someone clicks on an element.
---
## Create the Event

There are probably some key buttons on your site that are critical to the success of your business. They might be:

* Buttons to share your content (social media)
* Account creation buttons
* Purchase buttons

Many clickable elements on your site can be tracked so don’t limit yourself to just buttons. If it’s important and clickable, start tracking it.

It’s easy to tell KISSmetrics what clicks to keep track of. You’re going to go to your site, view the source code, and find the ID or a Class name of the clickable element you want to track. Name your new event, enter in the id or class name, and you’re done.

More detailed instructions coming soon!

## Technical Notes

* The "Clicks On" event type in the Event Library is equivalent to the JavaScript Library command [`trackClick`][trackClick]. You can use one or the other.
* The Event Library has trouble if you use **Ajax** to dynamically load page elements after the page has loaded (`document.ready()`). Our script scans the page once for the elements on which to instrument tracking.
* Currently, the Event Library takes only a *single* HTML ID or a *single* class name. If you'd like to use the full range of nested CSS selectors, please try using JavaScript Library calls for these types of events. If that does not work for you, please let us know if you are interested in seeing this functionality within the Event Library.

[trackClick]: /apis/javascript/javascript-specific#tracking-clicks