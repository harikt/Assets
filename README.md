# Assets for Process Wire

Assets module help you to move your `index.php` file of Process Wire
CMS to any part you like. The images, css, js etc will be served via 
assets for the first time.

On the next time, the requested file will be served by apache for it
will be in your document root. ( Assets module will try to copy the 
file to the document root on the first request)

## Known Issues

The file `/wire/modules/Jquery/JqueryTableSorter/JqueryTableSorter.js` 
is encrypted data. 

So the mimetype detect it as http://www.mime-type.net/application/x-elc/, 
so is not served.

You want to give appropriate permissions for the assets to write the `css`,
`images` and `js` in the `web` root folder.
