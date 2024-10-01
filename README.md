# [DearFlip jQuery/JS Flipbook Plugin](https://js.dearflip.com/)
Create realistic 3D FlipBook from PDF or images using jQuery powered DearFlip plugin. DearFlip creates PDF FLipbooks and Image Flipbook with 3D modes and 2D modes. This is JS/jQuery port of [DearFlip FLipbook/PDF Viewer](https://dearflip.com/) solution.

**Related Solutions:** jQuery flipbook, JS flipbook, PDF flipbook, JavaScript flipbook

## License
#### Attribution-NonCommercial-NoDerivatives 4.0 International
  
[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

This is a non-commercial Lite Version. You are free to use for only personal non-profit use, testing/trial not otherwise.
For commercial versions follow the links below:
[jQuery/JS Flipbook](https://js.dearflip.com/) or 
[WordPress Flipbook](https://wordpress.dearflip.com/)

For Desktop versions follow the links below:
[PDF Viewer](https://chrome.google.com/webstore/detail/pdf-to-flipbook-viewer-df/bbbnbmpdkfkndckfmcndgabefnmdedfp) Google Chrome Extension
For Wordpress Demo: Get DearFlip lite Wordpress : [3D Flipbook](https://wordpress.org/plugins/3d-flipbook-dflip-lite/) from Wordpress Repository

## Usage
### File Structure
DearFlip, also known as dFlip, flipbook plugin is jQuery based. Basically you can copy the files in folder to your working directory. We recommend copying the whole dflip folder as it is.

```
dflip/
  ├── css/
  ├── fonts/(fonts folder are not used since 2.0)
  ├── images/
  ├── sound/
  └── js/
      └── libs/
```
```
// In older versions, before v1.4.2, dflip folder was expected in the root where the html file is served.
// if not the location was required to be indicated.
// As of version 1.4.2, (not required in normal conditions, will be auto-detected)
var dFlipLocation = "http://www.yoursite.com/dflip/";
```
 
### Basic File Tempate
```
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Basic HTML Template</title>

<!-- Flipbook StyleSheets -->
<link href="http://www.yoursite.com/dflip/css/dflip.min.css" rel="stylesheet" type="text/css">
<!-- themify-icons.min.css is not required in version 2.0 and above -->
<link href="http://www.yoursite.com/dflip/css/themify-icons.min.css" rel="stylesheet" type="text/css">

</head>
<body>
<div class="_df_book" id="flipbok_example" source="location of pdf.pdf"></div>

<!-- Scripts -->
<script src="http://www.yoursite.com/dflip/js/libs/jquery.min.js" type="text/javascript"></script>
<script src="http://www.yoursite.com/dflip/js/dflip.min.js" type="text/javascript"></script>

</body>
</html>
```

### Example HTML Syntax
```
<!--Embedded Usage--> 
<div class="_df_book" source="http://www.yoursite.com/books/intro.pdf"></div>

<!--Button Lightbox Usage--> 
<div class="_df_button" source="http://www.yoursite.com/books/intro.pdf"> Intro Book</div>

<!--Thumbnail Lightbox Usage Images-->
<div class="_df_thumb" source="http://www.yoursite.com/books/intro.pdf"
     tags="3d,images" thumb="http://www.yoursite.com/books/thumbs/intro.jpg">Images</div>
````

### Extending with options
```
<div class="_df_button" id="button_pdf">Dflip Manual</div>
<div class="_df_button" id="button_image">Dflip Pictures</div>

//Just add option_ in front of the element id to create the required option variable
var option_button_pdf = {
    source:'http://www.yoursite.com/someplace/pdf-to-be-loaded.pdf',
    webgl:true,
    height:500
    //we recommend using default auto height
};

var option_button_image = {
     source : ['http://www.yoursite.com/books/thumbs/alice.jpg',
               'http://www.yoursite.com/books/thumbs/dflip.jpg',
               'http://www.yoursite.com/books/thumbs/nightangle.jpg'],
     webgl:true
};
```

More documentation at [DearFlip Flipbook JS/jQuery Docs](https://js.dearflip.com/docs/)


