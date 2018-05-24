# PowerPanel support pages

## Public available support content for website (http://powerpanel.io/support)

This is the public support manual for PowerPanel. You can contribute or pull these pages to make them available for your own customers through your own website.

All these page's are using the standard Markdown language. For the Markdown manual read this page: https://guides.github.com/features/mastering-markdown/

For a cheetsheet download this file: https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf

## Repository Guidelines

- There is a fixed menu structure. This is based on the PowerPanel menu items. Place all articles in the correct folders.
- In the root folder you have an images folder. Place all images you used in the articles in this folder (and make sure you don't overwrite any).
- Each language has their own folder. The folder structure needs to coresponde on the structure of the sitemap.json. 
- If you want to create support pages in a new language you can create a new language folder with the ISO two-letter language codes names (https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
- In the root of this project you can find a sitemap.json file. This file is build on the default PowerPanel menu structure. This structure will also be used for showing the support pages on the website. 
- Adding a new langauge you need also add the language to the sitemap.json file. Add a new value pair to the object 'description' and 'displayname' in the json file. Leave the name,permalink and type unchanged.  


**Example of the items in sitemap.json**


``` json    
{
  "displayname": {
    "nl": "Nieuwe gebruiker toevoegen",
    "en": "Add new user",
    "es":"Añadir nuevo usuario"
  },
  "description": {
    "nl": "Uitleg over een nieuwe gebruiker toevoegen",
    "en": "Some explanation about adding a new user",
    "es":"Alguna explicación sobre la adición de un nuevo usuario"
  },
  "type": "file",
  "name": "add_newuser.md",
  "permalink": "add-new-user"
}
```
- All of the folder names need to be lowercase
- Use always the full path to the images like below: 
```![PowerPanel example](/supportpages/images/photo.png)``` (Github does not show the image in preview, this is fine.)
