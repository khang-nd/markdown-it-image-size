# markdown-it-image-size

Adds `width` and `height` attributes to `img` tags rendered by markdown-it.

## Why

Browsers use the `width` and `height` attributes to [determine aspect ratios of images](https://developer.mozilla.org/en-US/docs/Web/Media/images/aspect_ratio_mapping). If the attributes are set, the browser can reserve space for the image even though it's not finished loading yet, thus preventing [cumulative layout shifts](https://web.dev/cls/) after images load.
