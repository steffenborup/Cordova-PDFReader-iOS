Cordova-PDFReader-iOS
==================

PDF Reader Cordova plugin for iOS 7+ (based on Reader https://github.com/vfr/Reader)

This is a fork of https://github.com/etabard/Cordova-PDFReader-IOS

![iPad Page](http://i.imgur.com/jaeCPz1.png)

![iPad Thumbs](http://i.imgur.com/1b4kY9s.png)

![iPod Page](http://i.imgur.com/y8wWRDN.png)

![iPod Thumbs](http://i.imgur.com/nddT2RP.png)


Features
------------

Multithreaded: The UI is always quite smooth and responsive.

Supports:

 - iBooks-like document navigation.
 - Device rotation and all orientations.
 - Encrypted (password protected) PDFs.
 - PDF links (URI and go to page).
 - PDFs with rotated pages.
 - PDFs with landscape double page feature

Installation
------------

To install from **command line**:

    cordova plugin add https://github.com/steffenborup/Cordova-PDFReader-iOS.git

or:

    phonegap local plugin add https://github.com/steffenborup/Cordova-PDFReader-iOS.git


Documentation
-------------

Supported URI scheme: file
For other schemes, please download it first with cordova plugin fileTransfer.

    //Open a pdf
    PDFReader.open('absolutepath.pdf', options, success, error);

    //Available options
    {
        password: null,
        flatUI: true,
        showShadows: true,
        enableThumbs: true,
        disableRetina: false,
        enablePreview: true,
        bookmarks: true,
        landscapeDoublePage: true,
        landscapeSingleFirstPage: true,
        toolbarBackgroundColor: null,
        textColor: null,
        enableShare: false
    }

    //Event when PDF Reader is closed
    document.addEventListener('PDFReaderClosed', function() {console.log('closed');})

    //Clear PDF Reader cache
    PDFReader.clearCache(filePath, finishedCallback);




----------
----------
----------
