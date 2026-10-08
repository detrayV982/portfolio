# Build log: Artifact 1 portfolio

Tool: Claude (free web chat), Sonnet 5.5. Started Tuesday, October 6, 2026.

This log records what I asked for and what came back. Claude wrote all of the site code. I made the decisions listed below and still need to do the verification at the bottom.

## Prompts and changes

1. I asked whether Claude could read the course site, then asked it to complete Artifact 1 and to ask me questions first. Claude read the Artifact 1 page and the course AI policy before building anything.
2. Claude asked four questions: what the about section should include, visual style, who writes the placeholder ideas, and which tech stack. I said to skip anything that is not necessary and gave no preference on the rest.
3. Claude's calls from those answers:
   - Short intro instead of a full about section (the assignment asks for a few sentences).
   - Dark, minimal style.
   - Plain HTML, CSS, and JavaScript with no build step, so it deploys straight to GitHub Pages.
   - Claude drafted the ideas on cards 2 to 5. I plan to edit them.
4. Claude produced the site as separate HTML, CSS and JavaScript files plus this log. The cards are generated from one data block, so finishing an artifact means editing one object there.
5. I created the empty public repo `detrayV982/portfolio` on GitHub. Claude could not push to it because its GitHub link was not set up on my account, so I upload the files myself.
6. I asked Claude to draft the card 1 reflection from what actually happened in this chat, and I kept the placeholder ideas on cards 2 to 5 because I had not thought about them yet. Claude also swapped the footer link from this log to the GitHub repo, since a raw .md link renders badly on GitHub Pages.

7. On October 8 I told Claude to replace the Artifact 2 idea with my own: a job search tool that scans for new postings and notifies me so I can apply first. Claude updated the card text. The idea is mine, the wording is Claude's.

8. I asked Claude to combine everything into one file to make uploading easier. The CSS and JavaScript now live inside `index.html`. The card data is the first script block in that file, marked `window.CARDS`.

## What I still need to do

- Read the card 1 reflection and edit it so it says what I actually think.
- Swap the ideas on cards 2 to 5 for ones I like, whenever I have them.
- Upload the files to the repo, turn on GitHub Pages, and submit the link on Canvas.
- Open the live site on my phone and my laptop and click through it.

## What I have checked

Claude ran a syntax check on the JavaScript and loaded the page in a headless browser at desktop and phone widths. All five cards rendered, there was no horizontal scrolling, and there were no console errors. I have not opened it myself yet. Update this section after I open the deployed site.

## Note on the reflection

The card 1 reflection began as a Claude draft based on the events above. I edit it before I submit, and the course policy says reflections should come from me.

## Parts I am trusting

- The CSS layout (grid, responsive breakpoints). I have not read it line by line.
- The card-rendering script builds the cards with `textContent`, so text in the card data is never treated as HTML.
