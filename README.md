# Mainevent Branch
Main repo for the Future Skills Academy mini site. This repository is used by GitHub pages to build a html site hosted online.

The Master branch is unused and will not be used to build pages. Only use the branch named "gh-pages" to place code.
All files within the gh-pages repository are visible to anyone authenticated with w3ID that visits: https://pages.github.ibm.com/fsa2017/mainevent/subfolder/file.extension

The default page that https://pages.github.ibm.com/InterConnect/manchester-Uni/ redirects to is index.html - this cannot be changed and will always be the default root page.

Relative links work to redirect to other pages - for example `<a href="agenda.html">` will redirect correctly without needing the absolute path.

## Security
The page is secured by IBM w3id - when accessing the site for the first time in a new browser session the user will be redirected to the IBM w3id page to log in. This restricts the page to all IBMers. Currently there is no other way to restrict access to specific members/bluegroups, nor is there any way of showing the site to anyone who is not authenticated with a w3id.
This ensures that the page, along with the GitHub repository, is secured behind the IBM firewall

Changes pushed to the gh-pages branch will directly change the website (within 2-3 mins)

## Themes & CSS
The site uses standard HTML with a small amount of JavaScript for some animations. The CSS uses the Materialize framework, based around Google's Material Design principles of texture and shadow. This can be found at http://materializecss.com . The minified version of the framework is found in the css folder, and contains all of the components listed on the Materialize site. To add a component, colour or JavaScript item, simply check the class name online and use this.
Please note, this site uses Materialize's containers and helpers to split the page into 12 columns, which are then used to size components in a uniform way. More information can be found at http://materializecss.com/grid.html

## Updating the site

#### Standard Site updates
To update the site, make changes locally to the HTML, then commit changes to the gh-pages branch. For larger layout/potentially breaking changes it is best to create a new branch, test it locally by visiting the file's location, and then merging the brnaches when ready.
A commit to the gh-pages branch should become live at the URL within 5 minutes in normal cases.
#### Enterprise GitHub Pages Issues
!! As of June 2017, IBM Whitewater GitHub has been suffering from issues with pushing changes to IBM GitHub pages. This is casued by queued requests not pushing correctly, which causes a backlog. The Whitewater team is attempting to resolve this issue, so view the status/any updates on https://status.whitewater.ibm.com/history. When commits are not going live within 10 minutes, DO NOT re-commit changes as this places you in the back of the queue. Merging branches may work faster, or alternatively waiting overnight tends to allow the backlog to clear and your commits to work. The main site should not go offline during this time.
#### Reminders
To make reminders visible, remove the "hide" class on line 62 to render a red bar. Change the text on line 63 to suit the reminder and it will appear in pulsing red/white as a full bar. Add further reminders as Plain text separated with a `<br>` tag to ensure the spacing will work correctly.
