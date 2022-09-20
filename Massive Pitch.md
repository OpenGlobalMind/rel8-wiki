# Massive Pitch

This page is a [[Tiles|Tile]] proposal. 

Massive Wiki used as PowerPoint. Please watch [this short, simple video](https://www.youtube.com/watch?v=bWkwOefBPZY) for context. 

The tl;dr: Imagine that instead of a slide deck that was a single document, a presentation instead was a playlist of pages in a wiki name space. 

This Tile needs code that:
- Marks a wiki page as the playlist for a presentation
- Has a "play" feature on that page that 
	- Goes full screen
	- Adds next/previous capabilities
	- Plays wiki pages in the playlist's order
- Offers minimal functional style settings to satisfy as a presentation
- Not essential: ability to start presenting from an arbitrary page in the playlist (to resume a pitch)
- Advanced and not essential: Slide-sorter view, with the ability to re-order slides

Multiple [HTML5 and Markdown presentation apps](https://bra.in/8qzJw6) exist, many of which are open source. Many of them use dividers inside one document to separate slides, which is not the intention here. But some of that code may be very useful here. 

## Similar Prototypes

### [Massive Pitch individual pages prototype](https://massive-pitch.netlify.app/)
In this prototype, if you navigate to a page that has this javascript on it and you indicate in the URL a file for pages this code will add a next and previous button. This allows you to crate multiple playlists out of individual pages without iframes. It is limited that each page has to have this enabled.  ([code](https://github.com/OpenGlobalMind/massive-pitch))


### [Web Story Prototype](https://web-story-prototype.netlify.app/)
in this prototype you can create a list of URLs and put the number of seconds after each one then click play and the code will open up another tab and will display each page after waiting the correct number of seconds. ([code](https://github.com/OpenGlobalMind/webstory))

---

## Proposal #1
a hosted web page and javascript code that reads a list of web pages from an external file named in the URL. You can navigate the list of pages in several ways similar to powerpoint.

### Initial Features
- Show the first page from the list in the web page
- a "Next" button to go to the next page
- a "Previous" button to go to the previous page
- Keyboard shortcuts to the buttons
- Option to have pages show up in another tab instead of in this web page

### Limitations
- If pages are openned up inside the page some web pages will not work if the owner expressly forbids it. This is a security feature of the web and would be difficult to circumvent.
- If the pages are openned up in another tab some owners can make the tab unable to be used again and a new tab will be spawned. This is a security feature of the web and would be difficult to circumvent.

### Possible Future Features
- Full Screen Button
- Quick naigation drop down
- Open new tab in another window and go full screen (dual screen presentation)
- A screen showing all the pages at one
- Ability to re-organize/ hide pages
- Hierarchical table of contents for quick navigation
