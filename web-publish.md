# Web Publish

You can now publish Objects as static web pages (HTTPS links) on your personal subdomain if you have \*any name. These pages are uploaded to our servers as unencrypted HTML files.&#x20;

This is an early version— linked Objects, and blocks like Queries and Collections aren’t supported yet. Multi-page publishing and other enhancements are on the way, and we’d love your feedback to guide these improvements.

<figure><img src=".gitbook/assets/webpublishing_2x (new).png" alt=""><figcaption></figcaption></figure>

### Encryption

When users use web publishing, we upload objects unencrypted for a number of reasons:

* Users explicitly choose an object to publish. So we limit the chance of accidental leakage.
* If users want their website to be indexed by search engines, it should be plaintext.
* The solution of decrypting in the browser and including the encryption key in the URL is a bit tricky in the case of multi-object exports.
* We do rendering and caching server-side to limit resource consumption.

The object is decrypted locally on the device and then uploaded to the web publishing server in Anyblock format.

If you have files in your object, we include the encryption keys for those files. But because each file has a unique locally-generated encryption key, it doesn't compromise your account in any way.
