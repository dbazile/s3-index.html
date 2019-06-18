# s3-index

![screenshot](/screenshot.png)

> Simple directory browser for an S3 bucket.


## Usage

Edit this section of `index.html`, then just drop the file in the root of your bucket:

```

    //
    // Configuration
    //

    const BUCKET_URL = 'https://<MY BUCKET NAME>.s3.amazonaws.com'
    const CONTENT_BASE_URL = BUCKET_URL + '/'
    const PREVIEW_LIMIT = (parseInt(location.search.replace(/^\?preview_kb=(\d+)/g, '$1'), 10) || 500) * KB

```


## Disclaimers

### This thing is pretty naive

This thing does a massive one-time scrape of 5000 keys at load time.  If your bucket has all those things in a single folder...  Well, there's no pagination.

### ES2015+, Flexbox

Life is too short to support ancient browsers for tiny side projects.
