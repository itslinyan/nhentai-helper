# nHentai Helper

Also support NyaHentai. Because its domain is constantly changing, if the script does not run on some domains, you can add the URL to the user matching list.

Support Tampermonkey and Violentmonkey. Not and will not support Greasemonkey.

## Main features

1. You can download doujin as zip (or cbz). **You must keep the page in the foreground when downloading.**
2. Add pjax support for list page. Changing pages will not interrupt downloads.
3. Download queue support on dojin list page. It will warn you when you download an already downloaded doujin, even they were uploaded by different people but have the same name. Up to 1000 history records.

![](https://i.loli.net/2019/01/26/5c4c5d5914197.png)

![](https://i.loli.net/2018/12/26/5c23a39505d14.png)

## Setting

![](https://i.loli.net/2020/02/18/iZKI9hfcLymdrBj.png)

1. **Download Thread**  
   If you think the download speed is too slow, you can try to increase the number of download threads from this setting.
2. **Open On New Tab**  
   Gallery page will be open on a new window by default, turn off it if you don't like it.
3. **Custom Download URL**  
   **WARNING: Please don't set this if you don't know what it does.**  
   Tip: You may need to add your domain into *XHR security* for this script.  
   Provide a URL containing the following placeholder:
   - `{{mid}}` - Media ID
   - `{{index}}` - Page index, starting from 1
   - `{{ext}}` - Image file extension
4. **Compression Filename**  
   Default is `{{japanese}}.zip`. You can custom the naming of downloaded compression file, including the file extension, such as `{{english}}.cbz`.  
   Available placeholders:  
   - `{{english}}` - English name of doujin
   - `{{japanese}}` - Japanese name of doujin
   - `{{pretty}}` - English simple title of doujin
   - `{{id}}` - Gallery ID
   - `{{pages}}` - Number of pages
5. **Compression Level**  
   Accept a numer in `0-9`, default is `0`.  
   `0` means "no compression", `1` means "best speed", `9` means "best compression".  
   Actually, for doujin, compression output size of `0` and `9` usually differ by less than **1%**.
6. **Filename Length**  
   Zeros will be padded to the start of image filename when its length lower than the value you specified. This can avoid the sorting confusion caused by sorting only by string in some cases.

## Other features

### Language filter

You can select a language in the navigation bar to filter doujins.

![](https://i.loli.net/2019/03/25/5c98d07cca0ac.png)

### 100% view height

Effective when reading online, only for NyaHentai (now nHentai already has this feature).

![](https://i.loli.net/2019/09/04/EYu5iP9L46b8XUf.png)
