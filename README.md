# PowerPanel support pages

## Public available support content for website (http://powerpanel.io/support)

This is the public support manual for PowerPanel. You can contribute or pull this pages to make them availble for your own customers via your website.

All this page's are using the standard Markdown language. For the Markdown manual read this page: https://guides.github.com/features/mastering-markdown/

For a cheetsheet download this file: https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf

## Repository Guidelines

- There is a fixed menu structure. This is based on the PowerPanel menu items. Place all articles in the correct folders.
- In the root folder you have an images folder. In this folder place all images you have used in the articles (make sure you don't overwrite any).
- For every langauge there is an own folder. In this folder you can find a sitemap.json file. This file is build on the default PowePanel menu structure. This structure will be used also for the support pages. 
- If you want to create suport pages in a new language you can create a new language folder always use the ISO two-letter language codes (https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
- Translate only then values on description, displayname and permalink in the json file. Leave the name and type unchanged  
```    
{
    "displayname": "Add new user",
    "description": "How to add a extra or new user to the panel",
    "type": "file",
    "name": "add_newuser.md",
    "permalink": "add-new-user"
}
```
- All folder names need to be lowercase
- Use always the full path to the images like below: 
```![PowerPanel example](/support/images/photo.png)``` (Github does not show the image this is fine.)
