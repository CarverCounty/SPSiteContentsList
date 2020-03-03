# SharePoint Site Contents List

![GitHub](https://img.shields.io/github/license/CarverCounty/SPSiteContentsList?style=for-the-badge)
![GitHub file size in bytes](https://img.shields.io/github/size/CarverCounty/SPSiteContentsList/SiteContents.html?style=for-the-badge)
![GitHub Release Date](https://img.shields.io/github/release-date/CarverCounty/SPSiteContentsList?style=for-the-badge)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/CarverCounty/SPSiteContentsList?style=for-the-badge)

This is a simple solution for screen scraping the lists, libaries, and subsites from a SharePoint 2013<sup>[1](#1)</sup> Site Contents page.<br>This comes in handy for extracting a list of a site's contents and metadata for cleanup purposes.<br>It can be used by any user with access to upload files.<sup>[2](#2)</sup>


## How to Deploy

This four step process is the simplest deployment, but it will not include your branding or navigation.<br>If that's something you'd like, please use the [Alternate Deployment](#alternate-deployment) instructions below.

1. Download the [SiteContents.html](https://github.com/CarverCounty/SPSiteContentsList/releases/latest) file.<sup>[3](#3)</sup>

2. Upload the file to a library, like SiteAssets, within your SharePoint Farm.

3. Now simply open the file and enter the URL to a SharePoint site into the textbox, or click the Submit button to run the script for the current site.<sup>[4](#4)</sup>

4. You can now copy the results using the Copy to Clipboard button and paste them into OneNote, Word, or another application to further detail notes about each item.


### Alternate Deployment

1. Download the [SiteContents.html](https://github.com/CarverCounty/SPSiteContentsList/releases/latest) file.<sup>[3](#3)</sup>

2. Upload the file to a library, like SiteAssets, at the __root of the site collection__.<sup>[5](#5)</sup>

3. Copy the link to the file.

4. Create a new page on the site or determine an existing page<sup>[6](#6)</sup> where you'll add the webpart.

5. Edit the page and add a new Content Editor webpart.

6. Edit the webpart and paste the link to the script into the Content Link field.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Content Link field in Webpart Editor](https://www.co.carver.mn.us/Home/ShowImage?id=11184)

7. Save the changes to the webpart and publish the page.

8. Now simply open the page and enter the URL to a SharePoint site, or click the Submit button to run the script for the current site.<sup>[4](#4)</sup>

9. You can now copy the results using the Copy to Clipboard button and paste them into OneNote, Word, or another application to further detail notes about each item.


## Results

![Results of final product](https://www.co.carver.mn.us/Home/ShowImage?id=11182)


## Notes

_<sup><a name='1'>1</a></sup>This has only been tested on SharePoint 2013 using Chrome or Internet Explorer 11._

_<sup><a name='2'>2</a></sup>The results are permission trimmed, meaning you will only see what you have access to see in the results._

_<sup><a name='3'>3</a></sup>To download the script, click the SiteContents.html link on the [latest release](https://github.com/CarverCounty/SPSiteContentsList/releases/latest)._

_<sup><a name='4'>4</a></sup>For the Submit button to work on the current site, the script or page must be saved to the root of a document library. It cannot be placed in a folder._

_<sup><a name='5'>5</a></sup>The script can be uploaded to any individual site. However, by uploading it to the root of the site collection, the script can be referenced on any subsite without needing to upload it to multiple sites. Additionally, should the script need to be modified in the future, it only needs to be changed in one place to be applied to all subsites where it's being used._

_<sup><a name='6'>6</a></sup>This script will not work on a page that uses ```_layouts/15/start.aspx#``` in the URL. This happens on site homepages when the Minimal Download Strategy site feature is activated. Simply deactivate this feature, manually modify the URL, or add the webpart to a page other than the homepage._


## License

This project uses the following license: [Unlicense](LICENSE).


## Disclaimer

We provide no guarantee of any kind this script will be kept up to date, nor do we guarantee support of any kind to make it work in any environment other than our own.
