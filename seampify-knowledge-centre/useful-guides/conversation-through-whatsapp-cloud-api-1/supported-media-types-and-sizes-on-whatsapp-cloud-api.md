---
icon: file-circle-plus
---

# Supported media types & sizes on WhatsApp Cloud API

{% hint style="danger" %}
The maximum supported file size for media messages on Cloud API is 100MB.
{% endhint %}

### Audio <a href="#audio" id="audio"></a>

| Audio Type | Extension | MIME Type                                                   | Max Size |
| ---------- | --------- | ----------------------------------------------------------- | -------- |
| AAC        | .aac      | audio/aac                                                   | 16 MB    |
| AMR        | .amr      | audio/amr                                                   | 16 MB    |
| MP3        | .mp3      | audio/mpeg                                                  | 16 MB    |
| MP4 Audio  | .m4a      | audio/mp4                                                   | 16 MB    |
| OGG Audio  | .ogg      | audio/ogg (OPUS codecs only; base audio/ogg not supported.) | 16 MB    |



### Document <a href="#document" id="document"></a>

| Document Type        | Extension | MIME Type                                                                 | Max Size |
| -------------------- | --------- | ------------------------------------------------------------------------- | -------- |
| Text                 | .txt      | text/plain                                                                | 100 MB   |
| Microsoft Excel      | .xls      | application/vnd.ms-excel                                                  | 100 MB   |
| Microsoft Excel      | .xlsx     | application/vnd.openxmlformats-officedocument.spreadsheetml.sheet         | 100 MB   |
| Microsoft Word       | .doc      | application/msword                                                        | 100 MB   |
| Microsoft Word       | .docx     | application/vnd.openxmlformats-officedocument.wordprocessingml.document   | 100 MB   |
| Microsoft PowerPoint | .ppt      | application/vnd.ms-powerpoint                                             | 100 MB   |
| Microsoft PowerPoint | .pptx     | application/vnd.openxmlformats-officedocument.presentationml.presentation | 100 MB   |
| PDF                  | .pdf      | application/pdf                                                           | 100 MB   |



### Image <a href="#image" id="image"></a>

Images must be 8-bit, RGB or RGBA.

| Image Type | Extension | MIME Type  | Max Size |
| ---------- | --------- | ---------- | -------- |
| JPEG       | .jpeg     | image/jpeg | 5 MB     |
| PNG        | .png      | image/png  | 5 MB     |



### Sticker <a href="#sticker" id="sticker"></a>

WebP images can only be sent in [sticker messages](https://developers.facebook.com/docs/whatsapp/cloud-api/messages/sticker-messages).

| Sticker Type     | Extension | MIME Type  | Max Size |
| ---------------- | --------- | ---------- | -------- |
| Animated sticker | .webp     | image/webp | 500 KB   |
| Static sticker   | .webp     | image/webp | 100 KB   |



### Video <a href="#video" id="video"></a>

Only H.264 video codec and AAC audio codec supported. Single audio stream or no audio stream only.

| Video Type | Extension | MIME Type | Max Size |
| ---------- | --------- | --------- | -------- |
| 3GPP       | .3gp      | video/3gp | 16 MB    |
| MP4 Video  | .mp4      | video/mp4 | 16 MB    |

<br>
