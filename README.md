# Hugo Shortcodes

Simple shortcodes for Hugo. 

* Audio: Implements the HTML audio tag
* Video: Implements the HTML video tag to run self-hosted videos.

## Getting Started

Just copy these shortcodes into your shortcodes directory:

```
path-to-hugo-repo/layouts/shortcodes/
```

### Prerequisites

Assumes you have a local Hugo repo.

### Installing

Clone this repo:

```
git clone https://github.com/billhennessy/hugo-shortcodes.git
```

Copy the shortcodes to your local repo:

```
cp ~/path-to-shortcodes-repo/layouts/shortcodes/*.html ~/path-to-hugo-repo/layouts/shortcodes
```

Your local Hugo repo should now contain `video.html` and `audio.html`

## Usage

### audio.html

Audio requires two arguments:

* path-to-audio with quotes `audio/my-voice-recording.mp3`
* preload (auto | metadata | none)

Example:

```
{{< audio "/audio/my-voice-recording.mp3" auto >}}

```

Note: I use only `auto` to prevent skipping in Chrome browser.

The HTML audio tag works with `.mp3`, `.ogg`, and `.wav` files only.

### video.html

IN DEVELOPMENT



## Deployment

Just follow your usual deployment method. 

## Built With

* HTML audio and video tags


## Contributing

Just submit a pull request.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/billhennessy/hugo-shortcodes/tags). 

## Authors

* **Bill Hennessy** - Sales Engineer and developer

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details



