# xeetBrain

xeetBrain transfers all your [X](https://x.com/) xeets into the [Obsidian](https://obsidian.md/) graph view.

Why?
---

**TLDR: I found X to be a nice thinking tool to organize my thoughts. Now I want to visualize the connections between these thoughts.**

Over the years I have found myself absorbing information, but not really thinking about what my own opinion on the matter is.

I find that the X / Twitter / Mastadon platform enables [depth](https://en.wikipedia.org/wiki/Depth-first_search) + [breadth](https://en.wikipedia.org/wiki/Breadth-first_search) thinking. Users can continuosly write down their thoughts in a linear-breath wise fashion, and  can also expand upon a thought in a depth-wise fashion.


How it works ( so far )
---

Users of xeetBrain must download their [X archive](https://x.com/settings/download_your_data), e.g. a collection of all their xeets.

You then place your `tweets.js` into xeetBrain and it outputs a zip archive containing a folder with all of your xeets, each in markdown, linked together in a linearly time-wise.

```
Your X data -> xeetBrain -> Obsidian vault
```

Notes
---

As of writing this, I only plan on making it work with X, until I transfer my thoughts to a local [Mastodon](https://github.com/mastodon/mastodon) node. Mastodon is basically an open-source X / Twitter. You are always welcome to fork or submit a pull request.

To Do
---

- [ ] Frontend:
   - [ ] Input:
      - [ ] Place to put your files into (drag and drop / selector)
   - [ ] System
      - [ ] Button that says 'Convert' that activates converter function
   - [ ] Output: a box that contains a .zip archive of all your xeets in markdown format
- [ ] Backend (converter function):  
   - [ ] Input -> Load data from drop box into converter function
   - [ ] System:
      - [ ] parse & clean data
      - [ ] extract all the necessary data
      - [ ] put it into markdown format
      - [ ] backlink all relevant xeets to eachother
      - [ ] zip all the xeets
   - [ ] Output:
      - a .zip archve of all your xeets, linked together, in markdown format
Edge cases
 - [ ] Linear xeets
 - [ ] Replies to your own xeet
 - [ ] Quotes to your own xeet
