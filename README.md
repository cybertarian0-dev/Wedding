# My Video Hub

A simple, responsive video-viewing website that can be published free with GitHub Pages.

## 1. Add your video

Open `index.html` and find the settings near the bottom:

```js
const SITE_TITLE = "My Video Hub";
const VIDEO_TITLE = "Featured video";
const VIDEO_DESCRIPTION = "Add a short description of your video here.";
const VIDEO_URL = "PASTE_YOUR_VIDEO_URL_HERE";
```

Replace the sample values. `VIDEO_URL` should be either:
- a **direct video file URL** ending in `.mp4`, `.webm`, or `.ogg`; or
- an **embed URL** from a video host, such as `https://www.youtube.com/embed/VIDEO_ID`.

For a four-hour video, upload it to a video hosting service first, then use its supported embed URL. A normal sharing link may not work in the player; use the host's embed option.

## 2. Publish with GitHub Pages

1. Sign in at https://github.com and create a new **public** repository, for example `my-video-hub`.
2. Upload `index.html` to the repository's top level (the root).
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch **main** and folder **/(root)**, then click **Save**.
6. Wait a minute or two. GitHub will show your website address, usually:
   `https://YOUR-USERNAME.github.io/my-video-hub/`

## 3. Change the video later

Edit `index.html` on GitHub, update `VIDEO_URL` and the title/description, and commit the change. The website will update after GitHub Pages rebuilds.

## Important limitations

- GitHub Pages hosts the **website files**; it does not provide a public video-upload form or a video database.
- Visitors cannot upload videos through this static site.
- Avoid storing a large or four-hour video in the GitHub repository. Use a video host for the video itself and let this page embed it.
- Make sure your video host allows embedding and that the video privacy settings allow your intended viewers to watch.
