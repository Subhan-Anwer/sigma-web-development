# Sigma Web Development Course

## Tutorial # 10 | Audio, Video & Media in HTML

[![Sigma Web Development Course - Tutorial # 10](https://img.youtube.com/vi/XZwBNDGuWGU/maxresdefault.jpg "Tutorial # 10 - Audio, Video & Media in HTML")](https://www.youtube.com/watch?v=XZwBNDGuWGU&list=PLu0W_10lII10agq10TrH10XLIKQvv0iaF2X3w&index=10)

---

## Media Format & Supported Media in HTML


### Common Video Formats

<br>

| Format  | File | Description |
| :---- | :--- | :--- |
| **MPEG**  | `.mpg` `.mpeg` | MPEG. Developed by the Moving Pictures Expert Group. The first popular video format on the web. Not supported anymore in HTML. |
| **AVI**  | `.avi` | AVI (Audio Video Interleave). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers. |
| **WMV**  | `.wmv` | WMV (Windows Media Video). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers. |
| **QuickTime**  | `.mov` | QuickTime. Developed by Apple. Commonly used in video cameras and TV hardware. Plays well on Apple computers, but not in web browsers. |
| **RealVideo**  | `.rm` `.ram` | RealVideo. Developed by Real Media to allow video streaming with low bandwidths. Does not play in web browsers. |
| **Flash**  | `.swf` `.flv` | Flash. Developed by Macromedia. Often requires an extra component (plug-in) to play in web browsers. |
| **Ogg**  | `.ogg` | Theora Ogg. Developed by the Xiph.Org Foundation. Supported by HTML. |
| **WebM**  | `.webm` | WebM. Developed by Mozilla, Opera, Adobe, and Google. Supported by HTML. |
| **MPEG-4 or MP4**  | `.mp4` | MP4. Developed by the Moving Pictures Expert Group. Commonly used in video cameras and TV hardware. Supported by all browsers and  recommended by YouTube. |

<br>

> **Note:** Only MP4, WebM, and Ogg video are supported by the HTML standard.

---

### Common Audio Formats

<br>

| Format  | File | Description |
| :---- | :--- | :--- |
| **MIDI**  | `.mid` `.midi` | MIDI (Musical Instrument Digital Interface). Main format for all electronic music devices like synthesizers and PC sound cards. MIDI files do not contain sound, but digital notes that can be played by electronics. Plays well on all computers and music hardware, but not in web browsers. |
| **RealAudio**  | `.rm` `.ram` | RealAudio. Developed by Real Media to allow streaming of audio with low bandwidths. Does not play in web browsers. |
| **WMA**  | `.wma` | WMA (Windows Media Audio). Developed by Microsoft. Plays well on Windows computers, but not in web browsers. |
| **AAC**  | `.aac` | AAC (Advanced Audio Coding). Developed by Apple as the default format for iTunes. Plays well on Apple computers, but not in web browsers. |
| **WAV**  | `.wav` | WAV. Developed by IBM and Microsoft. Plays well on Windows, Macintosh, and Linux operating systems. Supported by HTML. |
| **Ogg**  | `.ogg` | Ogg. Developed by the Xiph.Org Foundation. Supported by HTML. |
| **MP3**  | `.mp3` | MP3 files are actually the sound part of MPEG files. MP3 is the most popular format for music players. Combines good compression (small files) with high quality. Supported by all browsers. |
| **MP4**  | `.mp4` | MP4 is a video format, but can also be used for audio. Supported by all browsers. |

<br>

> **Note:** Only MP3, WAV, and Ogg audio are supported by the HTML standard.

<br>

---

<br>

## HTML Video - `<video>` Tag

The HTML `<video>` element is used to show a video on a web page.

### Syntax of `<video>` Element

The basic syntax of using a `<video>` element is below:

```bash
<video src="video.mp4" controls>Your browser does not support the video tag.</video>
```
The text between the `<video>` and `</video>` tags will only be displayed in browsers that do not support the `<video>` element.

<br>

#### Control Attribute

Control attribute adds controls, like play, pause, volume, speed and download.

#### Autoplay Attribute

To start a video automatically, use the autoplay attribute:

**Example:**
```bash
<video src="video.mp4" controls autplay></video>
```

<br>

> **Note:** Chromium browsers do not allow autoplay in most cases. However, muted autoplay is always allowed.

#### Muted Attribute

Muted attribue plays the video mute however, you can unmute the video if you have control attribue.

Add muted after autoplay to let your video start playing automatically (but muted).

#### Loop Attribute

Loop attribute plays the video in loop.


<br>

---

<br>

## HTML Audio - `<audio>` Tag

The HTML `<audio>` element is used to play an audio file on a web page.

### Syntax of `<audio>` Element

The basic syntax of using a `<audio>` element is below:

```bash
<audio src="audio.mp3" controls>Your browser does not support the audio element.</audio>
```

The **control**, **autoplay**, **muted** and **loop** are also the attribute of `<audio>` and works same in `<video>` and `<audio>` elements.

<br>

---

<br>

## The `<iframe>` Tag

The iframe tag is used to load another website in your website.

**Example:**

```bash
<iframe src="https://en.wikipedia.org/wiki/IFrame" width="500" height="300" allowfullscreen="true"></iframe>
```

**Output:** 

<!-- <iframe src="https://en.wikipedia.org/wiki/IFrame" width="500" height="300" allowfullscreen="true"></iframe> -->

### YouTube Videos using Iframe
The easiest way to play videos in HTML, is to use YouTube. Iframe element can be used to that too.

Add the YouTube video url in the src attribute of the `<iframe>` element.

Or go to YouTube video and Click on the Share button > Click Embed > Copy the `<iframe>` tag and paste in the HTML file.

<br>

---

<br>

## The `<svg>` Tag

SVG stands for Scalable Vector Graphics. Its a vector form of an image and are scalable, means it will not pixelate or blur.

SVG defines vector-based graphics in XML, which can be directly embedded in HTML pages.

### Syntax for `<svg>` Tag

The HTML `<svg>` element is a container for SVG graphics.

**Example:**

```bash
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow"/>
</svg>
```

**Output:**

<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow"/>
</svg>

SVG can also be used as filepath in the `<img>` tag src attribute.

- store the SVG content in `.svg` a file like `image.svg`
- add this namespace declaration in the file `xmlns="http://www.w3.org/2000/svg"`
- inside the `<img>` tag give the file path in src attribute.
- 