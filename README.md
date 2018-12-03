# ROCKSYDNEY WIKI

## Table of Contents
1. [Banner Design Guideline](#banner-design-guideline)
2. [CMS Manual](#cms-manual)
   1. [Uploading Banner](#uploading-banner)
   2. [Sorting Banner Order](#sorting-banner-order)
3. [Embedding Online Video](#embedding-online-video)

## Banner Design Guideline

The optimal size for the website banner is 1920 x 543px. 

![Banner Guideline](https://github.com/viperfx07/rocksydney-wiki/raw/master/rocksydney_banner_guideline.jpg)

The mobile safe area is the area where copy should sit so that it shows correctly on various screen size on any devices. I've prepared the Guides in a PSD file for design convenience. Please download it [here](https://github.com/viperfx07/rocksydney-wiki/raw/master/rocksydney_banner_guideline.psd).

## CMS Manual

### Uploading Banner
![Banner Upload Manual](https://github.com/viperfx07/rocksydney-wiki/raw/master/upload_banner_1.jpg)

To upload the banner, you need to login to the [CMS](https://rocksydney.org.au/admin). After logging in, please follow below steps:
1. Hover on `QODE Slider` and choose `Add New Slide`. After choosing `Add New Slide`, you will see the page as per screenshot above.
2. Enter a title
3. Make sure the **Slide Background Type** is _Image_
4. Click on the _Upload_ button next to **Slide Image**. 
   1. After clicking the Upload button, you can choose an image if it's already uploaded from the **Media Library** or if it hasn't been uploaded, you can drag & drop the image you want to upload.
   2. Then after the image is uploaded, click the image and press Select Image

![Banner Upload Manual](https://github.com/viperfx07/rocksydney-wiki/raw/master/upload_banner_2.jpg)

5. Select **Main** under Sliders / All Sliders tab.
6. Click `Publish` to publish your changes.

### Sorting Banner Order

![Banner Upload Manual](https://github.com/viperfx07/rocksydney-wiki/raw/master/upload_banner_3.jpg)

To re-ordering the banner is fairly simple. Hover on `QODE Slider` and choose `Slides`. After choosing `Slides`, you will see the page as per screenshot above.
1. Navigate your mouse to the slide you want to edit, then click **Quick Edit**. 
2. The smaller the number entered in _Order_, will be shown first before a greater number. Note: You may need to check the other slides' order as well
3. After entering the _Order_, click **Update**.


## Embedding online video


### Offline way (Fastest)

**Note:** _If you have done step 1 - 3, please skip to 4 forwards. Steps below were done in Chrome and for Youtube video only_
1. Copy the source below

``javascript:(()=>{
	var youtube_parser = (url) =>{ 
		var regExp = /.*(?:youtu.be\/|v\/|u\/\w\/|embed\/|watch\?v=)([^#\&\?]*).*/; 
		var match = url.match(regExp); return (match&&match[1].length>=11)? match[1] : false; 
	}; 
	var x = prompt('Enter youtube video url: '); 
	alert(`<div class='embed-container'><iframe src='https://youtube.com/embed/${youtube_parser(x)}' frameborder='0' allowfullscreen></iframe></div>`)
})()``


![Adding bookmark](https://github.com/viperfx07/rocksydney-wiki/raw/master/embed_video_1.jpg)

2. Create a bookmark by right clicking the bookmark area and choose **Add page**

![Adding bookmark](https://github.com/viperfx07/rocksydney-wiki/raw/master/embed_video_2.jpg)

3. Give whatever name you want and paste the source from **step 1** in the URL box
4. Once the bookmark is created, copy the video url you'd like to embed

![Adding bookmark](https://github.com/viperfx07/rocksydney-wiki/raw/master/embed_video_3.jpg)

5. Click the bookmark and paste the video url

![Adding bookmark](https://github.com/viperfx07/rocksydney-wiki/raw/master/embed_video_4.jpg)

6. You will see a popup as above screenshot. Copy the highlighted part starting from `<div class='embed-container'>` to `</div>`

6. Paste it on the Wordpress editor

### Online way

![Embedding Video](https://github.com/viperfx07/rocksydney-wiki/raw/master/embedding-video.jpg)

1. Copy the url of the video you'd like to embed
2. Go to https://embedresponsively.com
3. If the url is **Youtube**, choose tab **Youtube.com** and paste it on the input box
4. Click **Embed**
5. Copy starting from `<div class='embed-container'>` to `</div>` (highlighted on the picture)
6. Paste it on the Wordpress editor

