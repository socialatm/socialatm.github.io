From: [https://github.com/fengyuanchen/cropperjs](https://github.com/fengyuanchen/cropperjs)

javascript image cropper that we use to crop cover photos and profile pictures.

used in 2 places:
`Zotlabs\Module\Profile_photo.php` and `Zotlabs\Module\Cover_photo.php`.  

they both call the template file **crophead.tpl** which contains the cropperjs javascript and css links.

We call it from the browser and only use the `dist` and `docs` folders.