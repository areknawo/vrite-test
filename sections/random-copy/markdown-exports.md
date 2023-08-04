### Markdown Exports

Now, with the editor working, the last important part was to output Markdown. TipTap provides methods to retrieve both HTML and ProseMirror JSON representations of the content. I decided to use the JSON (since it’s easier to work with) and created functions to transform it into various outputs. I called these _“Content Transformers”_.

![](https://assets.vrite.io/6409e82d7dfc74cef7a72e0d/Ti3gDzFHWvSRgu0X4UgS7.png)

Using Content Transformers I created an “Export” menu, outputting the content in HTML, GitHub Flavored Markdown (GFM), and ProseMirror JSON (e.g. for custom processing) to a Monaco Editor, with options to download or copy it.

While there might be better ways to do this, this one provides a lot of flexibility and makes sure your content can be properly processed to Markdown or any other format you need.