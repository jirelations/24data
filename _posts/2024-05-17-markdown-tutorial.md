---
layout: tutorial
session: 5
tags: [4,5,tutorial]
category: tutorial
image: markdown.svg
---

### 1. Edit a Markdown file from the Recipes project

1. In Github Desktop, make sure you have the latest changes from the Recipes project on your computer by changing to the "master" branch and then pressing "Fetch origin" and (if shown) "Pull origin".
2. Follow the steps in the [Git Tutorial section 2](git-tutorial) to create a new branch in Github and open one of the files in the `_posts` directory of the Recipes project using Visual Studio Code.
3. In Visual Studio Code, make a word or phrase **bold** by putting `**` on each side of it. Because Visual Studio Code supports Markdown, you will see the word change to bold when you edit it.
4. You can check what your Markdown will look like by clicking the "Preview" button to the right of your tab in Visual Studio Code.
5. Put a word or phrase in _italics_ by putting `_` on each side of it. (You can do the same thing by using `*` instead of `_`.) In Visual Studio Code, you can also use some keyboard shortcuts like `Ctrl+B` for bold and `Ctrl+I` for italics, the same way you would in Microsoft Word. (On Mac: `⌘+B` and `⌘+I`)
6. Try creating or changing a numbered list by typing a `1.` at the beginning of a line, followed by a space and some text. Then press the `Return`/`Enter` key to create a new line. The next number will automatically be added. For example,  

    ```markdown
    1. 200g Flour
    2. ...
    ```
7. To add a link, put the text of the link between square brackets `[]`, followed by the web address in parentheses `()`, like this:
    ```markdown
    [text of the link](https://example.com)
    ```

    There shouldn't be any space between the `]` and the `(`.
8. Adding images is similar. Try copying this into your document:  
    ```markdown
    ![Dancing Cat](http://i355.photobucket.com/albums/r460/Maddy11_02/cat-dance.gif)
    ```

### 2. Sync your Markdown file to the Recipes project

1. Save your changes to the file by pressing `Ctrl+S` (Mac `⌘+S`) or using the File > Save menu in Visual Studio Code.
2. In Github Desktop, commit your changes and publish your branch (see [Git Tutorial 2.4](git-tutorial)).
3. Go to <https://gitlab.gwdg.de/24recipes/24recipes.pages.gwdg.de> and log in. Let me know if this is your first time logging into Gitlab, so that I can give you permission to do the merge request. 
4. Create a Merge Request to get the changes from your branch into the "master" branch. (See [Git Tutorial section 4](git-tutorial)). I will have to manually approve this merge request.

### 3. Try some HTML in your Markdown

With Markdown you can do basic text formatting, but with HTML you can do much more. Markdown is normally converted into HTML web pages (or other formats), but you can actually put sections of HTML _into_ your Markdown file when you want to do something fancy. 

1. Open one of the Markdown files from the Recipes project (as in Step 1), but this time <span style="color:red">make a word or short phrase (not more than 1 line) red</span>. You can copy and paste this before the text you want to turn red: `<span style="color:red">` and this after the text: `</span>`. 
2. Note the structure of what you inserted. HTML needs a "start tag" -- this is the `<span ...>` and an end tag, the `</span>`. In the start tag you can also have "attributes" -- here, the `style="color:red"` separated by a space from the name of the tag or from other attributes. The whole thing -- everything between the start and end tags -- is called an "element". 
3. Suppose you want to make the dancing cat image huge. Try this:
    ```html
    <img src="http://i355.photobucket.com/albums/r460/Maddy11_02/cat-dance.gif" width="500px"/>
    ```
    You might notice that the `<img>` element has no end tag, but it does have a weird `/` before the final `>`. In HTML (and XML), there's sometimes no need for text in between tags (as in the case of an image). In these cases a `/>` at the end of your tag signals that the element is complete. A start tag and end tag all in one!
4. Save and commit your changes, and sync them to the Recipes project the same way you did in Step 2 above.

### 4. View the full HTML page

We've put some HTML _inside_ Markdown, but you haven't yet seen what your whole page looks like on the Recipes website. Once I've merged in your changes (step 2 above), you'll see your page appear at <https://24recipes.pages.gwdg.de/>.

1. Click on the page you edited. Notice what it looks like (bold and italic text, numbered list, image).
2. Now right-click anywhere on a blank part of the page and then click "View Page Source". (The wording might be a bit different depending on your browser.) This is what the page you edited looks like in HTML code. The first part (under `<head>`) was created automatically, but if you scroll to the bottom, you'll see the content you edited.