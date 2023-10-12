# How do I change the line spacing in Thunderbird?

I was surprised by the modified UX from version 115. I don't know why the rows displaying incoming emails were disproportionately narrowed. It seems very reckless to me. After searching through a few posts, I found that many users are concerned with these ordeals.

I was determined to straighten out the situation a little, at least in my case.

## How to Fix Line Spacing In Thunderbird after version 115 updated?

Here I am attaching instructions on how I solved the situation.

First, enable your own style according to this guide: https://github.com/Aris-t2/CustomCSSforTb

You are using userChrome.css which is part of this repository.

```css
/* Height of menu bar */
toolbar {
  min-height: 28px !important;
}

/* Height od row in message list */
table[is="tree-view-table"] {
  line-height: 2em !important;
}

/* Height of item in tree on left side */
:is(ul, ol):is([role="tree"], [role="group"]) li > div {
  line-height: 2em;
}
```

The only thing that adjusts the style is the height of the lines in the menu, in the tree on the left and the height of the lines with emails.

**Happy coding.**

**Pavex**

