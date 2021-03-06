# [smi : social media icons &amp; links](http://nevvix.com/smi)

## Create a social media icon bar without iframes or spying analytics.

The goal is for anyone to use this code to create a custom social media icon bar without the `iframe`s used by social media widgets.

The SVG icon images are produced from Dan Leech's [Simple Icons](https://simpleicons.org/) project.

The Font Awesome icons are from Dave Gandy's [Font Awesome](http://fontawesome.io/").

## Why use it?

* ["Those tiny Tweet, Like, +1 buttons you see on websites are actually brutally large elements to load for (mobile) devices."](http://zurb.com/article/883/small-painful-buttons-why-social-media-bu)
* ["Services like AddThis and ShareThis will always spy on and tag your audience when you use their widgets"](http://ma.tt/2014/07/canvas-fingerprinting-addthis)
* ["If your image is instead a set of dom nodes, it cuts that extra HTTP request out, making your website faster and more user friendly."](http://code.tutsplus.com/articles/why-arent-you-using-svg--net-25414)

## Usage using Simple Icons

Insert `require_once '{where smi is located}/smi/smi.php';` at the top of your PHP page.

Insert `<link rel="stylesheet" href="smi/si/smi.css">` in the `<head>` section of your HTML code.

Use the `smi/si/smi.json` template to create your own data set of links and functionality.

Then embed PHP `smi()` calls in your page.

`smi()`'s optional arguments can be in native PHP array or JSON string format.

## Usage using Font Awesome icons

Insert `require_once '{where smi is located}/smi/smi.php';` at the top of your PHP page.

Insert `<link rel="stylesheet" href="smi/si/smi.css">` in the `<head>` section of your HTML code.

Use the `smi/fa/smi.json` template to create your own data set of links and functionality.

Then embed PHP `smi()` calls in your page.

`smi()`'s optional arguments can be in native PHP array or JSON string format.

## Examples using Simple Icons

`<?= smi("si", ["space"=>"3px"]) ?>`

`<?= smi("si", '{"px": "24", "space": "1rem"}') ?>`

`<?= smi("si", ["px"=>"32", "icons"=>["Facebook","Google+","Pinterest"], "space"=>"4px"]) ?>`

`<?= smi("si", '{"all": true, "px": "64"}') ?>`

## Examples using Font Awesome icons

`<?= smi("fa", ["space"=>"3px"]) ?>`

`<?= smi("fa", ["px"=>"24", "space"=>"3px"]) ?>`

`<?= smi("fa", ["px"=>"32", "space"=>"3px"]) ?>`

`<?= smi("fa", ["px"=>"64", "icons"=>["fa-facebook-square","fa-twitter-square","fa-at-square"], "space"=>"3px"]) ?>`

[Official page and examples](http://nevvix.com/smi)
