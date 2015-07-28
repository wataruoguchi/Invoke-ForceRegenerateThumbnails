# Invoke-ForceRegenerateThumbnails
Invoke a WordPress plugin "Force Regenerate Thumbnails" queuing by JSON

## How to prepare?
1. Check the link address when you usually invoke it. WP Admin page > Media > Mousehover "Force Regenerate Thumbnails" > right click and copy the URL.
    ``ex.) http://hostname/wp-admin/tools.php?page=force-regenerate-thumbnails&goback=1&ids=99999&_wpnonce=1b3f7d3384``
2. replace _wpnonce in get() method by the one you see in the link address
3. Make a JSON file and name it "imageIdList.json"
    ``ex.) [{"post_id": 99998}, {"post_id": 99999} ....]``
4. Save this html file and the JSON file in root directory.
5. Open this html page by a browser, view a console window of the browser, then click a button.
6. Wait until it's done.
