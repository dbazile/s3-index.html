# s3-index

![screenshot](/screenshot.png)

> Simple directory browser for an S3 bucket.


## How to use?

Just drop `index.html` in the root of the bucket.  If you need to configure things, jump down to the top of the `script` tag.


## Disclaimers

### This thing is pretty naive

This thing does a massive one-time scrape of 5000 keys at load time.  If your bucket has all those things in a single folder...  Well, there's no pagination.

### ES2015

Life is too short to support ancient browsers for tiny side projects.
