adapt-nakedMedia
===================

This is a straight copy of adapt-contrib-media with all skinning and playbars hidden which also (should) stops on last frame the idea being you can use it to replace basic flash animations which click to interact method, hoping transparency works with the video formats we use but have yet to test <- nope to trasparency unfortunatly

Use a poster as cant work out how to get showfirst frame on load working

A basic media component that plays audio and video. This component uses the HTML5 audio and video specification and has a Flash/Silverlight alternative for browsers that don't support HTML5.

The component uses [MediaElement.js](http://mediaelementjs.com/) (v2.13.1) which enables users, amongst other things, to offer subtitles and accessible, skinnable (with CSS) controls. MediaElement.js carries an MIT license and is therefore compatible with Adapt.

Installation
------------

First, be sure to install the [Adapt Command Line Interface](https://github.com/cajones/adapt-cli), then from the command line run:

		adapt install adapt-nakedMedia

Usage
-----

For example JSON format, see [example.json](https://github.com/adamlaird/adapt-nakedMedia/blob/master/example.json).

Audio example

	"_media": {
		"mp3": "course/assets/audio.mp3",
		"ogg": "course/assets/audio.ogg"
	},

Video example

	"_media": {
		"mp4": "course/assets/video.mp4",
		"ogv": "course/assets/video.ogv"
	},

YouTube Video example

  "_media": {
    "source": "http://www.youtube.com/watch?v=nOEw9iiopwI",
    "type": "video/youtube"
  },

Important
---------

MediaElement.js v2.13.1 requires a small patch to enable it to work in IE8 when used in conjunction with Adapt.
