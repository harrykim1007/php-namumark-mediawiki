## License
This extension can be used freely according to GNU Affero GPL 3.0. Please see the attached document for details on the license.

## Dependencies
* [EmbedVideo](https://www.mediawiki.org/wiki/Extension:EmbedVideo)
* [Cite](https://www.mediawiki.org/wiki/Extension:Cite)
* [Math](https://www.mediawiki.org/wiki/Extension:Math) or [SimpleMathJax](https://www.mediawiki.org/wiki/Extension:SimpleMathJax)
* [Poem](https://www.mediawiki.org/wiki/Extension:Poem)

## Installation
1. Create a new NamuMark folder in the MediaWiki extensions folder. Or, if you can use git directly on the server, command the following in the extensions folder of MediaWiki installed.

		git clone https://github.com/Oriwiki/php-namumark-mediawiki.git NamuMark

1. Click [here](https://github.com/Oriwiki/php-namumark-mediawiki/archive/master.zip) and download the file, unzip it, and put all the unzipped files in the NamuMark folder. (It is not necessary if you did it with git.)
1. Enter the following in LocalSettings.php.

    ```php
	require_once "$IP/extensions/NamuMark/namumark.php";
	$wgRawHtml = true;
	$wgAllowImageTag = true;
	$wgNamespacesWithSubpages[NS_MAIN] = true;
	$wgNamespacesWithSubpages[NS_TEMPLATE] = true;
	$wgAllowDisplayTitle = true;
	$wgRestrictDisplayTitle = false;
	$wgDefaultUserOptions['numberheadings'] = 1;
    ```
