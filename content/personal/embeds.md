+++
title = "Images & Embeds"
date = 2024-09-28T16:30:22Z
tags = ["embeds", "multimedia", "social-media", "video", "interactive"]
description = "Image rendering and YouTube embed shortcodes."
+++

## Images

### Standard Image (Markdown)

![A scenic mountain landscape](https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=900)

### Image with Title

![Abstract architecture](https://images.unsplash.com/photo-1486325212027-8081e485255e?w=900 "Modern architecture lines")

### Local Image

![Site logo](/images/logo.png)

---

## Figure Shortcode

Hugo's built-in `figure` shortcode gives more control over captions and linking.

```
{{< figure src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=900"
    alt="Mountain landscape"
    caption="A panoramic mountain view at golden hour."
    width="100%" >}}
```

{{< figure src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=900" alt="Mountain landscape" caption="A panoramic mountain view at golden hour." width="100%" >}}

---

## YouTube Embed

Using Hugo's built-in `youtube` shortcode:

```
{{< youtube dQw4w9WgXcQ >}}
```

{{< youtube dQw4w9WgXcQ >}}

---

### YouTube with Custom Parameters

```
{{< youtube id="dQw4w9WgXcQ" autoplay="false" >}}
```

{{< youtube id="dQw4w9WgXcQ" autoplay="false" >}}

