# CLACTER
A chronicle for worldbuilders, characters and their tangled fates.

## Run and install

Serve this folder from an HTTPS site (or `localhost` while developing), then open
`clacter.html`. The app stores chronicles and images in the browser's local
IndexedDB/Origin Private File System; clear neither site data nor browser storage
if thou wouldst keep them. Android browsers offer **Install app** or **Add to Home
screen**. On iOS, open the page in Safari, tap **Share**, then **Add to Home
Screen**.

## Articles and characters

In the wiki, choose **Articles**, select a world or character, then press **Edit**.
Saving returns to the reading view. The editor understands headings (`#`, `##`,
`###`), **bold**, *italic*, lists beginning with `-`, and character mentions such
as `@Aurelia` or `@Queen_Aurelia_the_Pale`. Image uploads are inserted with
captions; the equivalent article syntax is:

```text
[[image:portrait.png|Aurelia beneath the ash trees|right]]
```

Use `left` instead of `right` to float an image to the left. Mentions and custom
character properties (for example `mother: @Aurelia`) populate **Character Links**
and **Family Tree**. Add as many properties as needed when creating a
character. The **Google Docs** control imports a `.docx` downloaded from Google
Docs, carrying headings and embedded images into the selected world's article.

## Import and export

**Export ZIP** creates a portable archive containing `world.json` and the images
under `images/`. Import accepts this format and restores its articles, characters,
properties, and images. Large images are streamed through ZIP64 and OPFS where
the browser supports them. For archives exceeding 1 GiB, export requires a
browser with streaming file-save support; imports of individual images over
64 MiB require OPFS. Actual storage limits remain those imposed by the device
and browser.

