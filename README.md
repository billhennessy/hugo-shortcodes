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

The HTML audio and video tags require later browsers. You can see which [browsers comply here](https://en.wikipedia.org/wiki/HTML5_audio). 

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

* path-to-audio with quotes `/audio/my-voice-recording.mp3`
* preload (auto | metadata | none)

Example:

```
{{< audio "/audio/my-voice-recording.mp3" auto >}}

```

!Important: remember the preceding `/` on file location.

Note: I use only `auto` to prevent skipping in Chrome browser.

The HTML audio tag works with `.mp3`, `.ogg`, and `.wav` files only.

### video.html

Currently supports only MP4.

Video requires four arguments:

* path-to-audio with quotes `/video/my-video.mp4`
* width in pixels 
* height in pixels 
* preload (auto | metadata | none)

Example:

```
{{< video "/video/my-video.mp4" 600 400 auto >}}

```

!Important: remember the preceding `/` on file location.



## Deployment

Just follow your usual deployment method. 

For deploying self-hosted audio and video files, I create a directory `/static/audio` and `/static/video`. 

## Built With

* HTML audio and video tags


## Contributing

Feel free to improve or add any Hugo shortcodes you'd like. Just submit a pull request. 

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/billhennessy/hugo-shortcodes/tags). 

## Authors

* **Bill Hennessy** - Sales Engineer and developer

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details



