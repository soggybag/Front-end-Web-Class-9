# Front-end-Web-Class-9

## Objectives

- Analyze pages for responsive design
- Apply media queries 

|   |   |   |   |
|---|---|---|---|

### 1 - @media

Use @media to define rules that apply only to specific media. 

#### What is "media" 

Media can be just about anything. CSS defines the following media types: 

- all
- print
- screen
- speech

But that's not all these can be qualified by checking the features of the current media. 
CSS looks at the following features see the list here: 

[https://developer.mozilla.org/en-US/docs/Web/CSS/@media](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)

There are also some modifiers that can applied: and, only, max, min. 

You can put these together to create CSS rules that apply in a wide variety of situations. 
Generally the most common use is creating rules that apply to mobile vs desktop. 
These are usually written to target different screen sizes. 

#### Break points 

The term "break point" describes the width at which we can assume fits the screen size of a range of devices. 
For example, if a device has a maximum width of 320px then it must be one of the early iPhones or a very smaller computer.
If the minimum width is 768px it's at least an iPad in portrait, though it could be a larger device. 

### 3 - Responsive stratgeies 

In general terms you will want to design for one platform mobile or desktop. 
Then use media queries to target rules for the other platform. 

For example, imagine you have designed your web site for the desktop. 
You have a box that is 33% width. On mobile this would be too narrow, 
you decide that on molbile boxes should be 100%. 
In CSS this might look this:

```
.box {
    width: 33%;
}

@media screen and (max-width: 414px) { 
    .box {
        width: 100%;
    }
}
```

The first rule sets the width of .box to 33%. 
The @media block contains a block of CSS that defines the width of .box to 100%.
Notice that following @media we have said that the media type is screen and
features a maximum width of 414px. 

The rules defined inside @media are only applied when the conditions are met.

Here it is in picture form:

__Desktop__

![Desktop](Notes/desktop.png)

__Mobile__

![Mobile](Notes/mobile.png)

#### Points vs Pixels 




## Resources 

- http://1stwebdesigner.com/responsive-design-breakpoints/
- https://css-tricks.com/snippets/css/media-queries-for-standard-devices/
- https://developers.google.com/web/fundamentals/design-and-ui/responsive/








### Closer look at jQuery

Adding and removing classes from an element or group of elements 
probably has the most practical applications with jQuery.



Slide shows 

- Horizontal 
- Vertical 
- Two axis
- Opposing motion
- Put a slide show in a window
- use the whole page
