# PowerPanel support pages

## Public available support content for website (http://powerpanel.io/support)

This is the public support manual for PowerPanel. You can contribute or pull these pages to make them available for your own customers through your own website.

All these page's are using the standard Markdown language. For the Markdown manual read this page: https://guides.github.com/features/mastering-markdown/

For a cheetsheet download this file: https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf

## Repository Guidelines

- There is a fixed menu structure. This is based on the PowerPanel menu items. Place all articles in the correct folders.
- In the root folder you have an images folder. Place all images you used in the articles in this folder (and make sure you don't overwrite any).
- Each language has their own folder. In each of these folders you can find a sitemap.json file. This file is build on the default PowePanel menu structure. This structure will also be used for the support pages. 
- If you want to create support pages in a new language you can create a new language folder with the ISO two-letter language codes names (https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
- Only translate the **values** for 'description', 'displayname' and 'permalink' in the json file. Leave the name and type unchanged  
```    
{
    "displayname": "Gebruiker toevoegen",
    "description": "Hier uitleg over gebruiker toevoegen",
    "type": "file",
    "name": "add_newuser.md",
    "permalink": "add-new-user"
}
```
- All of the folder names need to be lowercase
- Use always the full path to the images like below: 
```![PowerPanel example](/supportpages/images/photo.png)``` (Github does not show the image, this is fine.)
