We have no idea what we're doing but whatever we do will be documented here.  
It will be based on [Bootstrap](https://getbootstrap.com/) and will be responsive.  
We welcome any feedback or suggestions.
* Turns out that we don't need a new theme, just a new [template](https://github.com/socialatm/test/blob/master/view/php/default.php)

### Getting started

_pathtowebsite/view/en/htconfig.tpl_ line 100  
`App::$config['system']['theme'] = 'redbasic';`  
gets written to:    
_pathtowebsite/.htconfig.php_ during install.  
Default theme lives at:  
_pathtowebsite/view/theme/redbasic_   

### Can we make it stand alone?

From the main website folder:

* modules are located at: `./Zotlabs/Module/`
* PDL files are located at: `./view/pdl/`  
* template files are located at: `./view/tpl/`  
* layout template files are located at: `./view/php/`
* css files are located at: `./view/css/`
* If you don't select a template in your **.pdl** the default template will be used.
* The main files we're working with right now are the layout template and the css files, both named default.
* Do not add a blank default.css file, it will give you nightmares...  

It's really rough but yes, we have it up and working on our development server.

### Testing

When you're ready test your new layout template rename the **default.php** template **default-old.php** and name your new template **default.php**  
Same goes for the **default.css** file. That way if needed you can always change them back.





