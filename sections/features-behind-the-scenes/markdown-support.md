### Markdown Pasting

Handling Markdown pasting was a surprising challenge. Naturally, you’d expect an editor that works with Markdown to be able to parse and properly load the Markdown you pasted, so some work had to go into that.

TipTap provides [input rules](https://tiptap.dev/guide/custom-extensions/#input-rules) to handle so-called “Markdown shortcuts” while typing, and [paste rules](https://tiptap.dev/guide/custom-extensions/#paste-rules) for offering the same parsing functionality while pasting. The problem is, paste rules work line-by-line, which means parsing something like a blockquote, codeblock, or a list, just isn’t possible.

To handle pasting block Markdown content like this, I had to tap into ProseMirror and implement a custom mechanism (though somewhat based on TipTap’s paste rules), detecting starting and ending points of the blocks and parsing them with [Marked.js](https://marked.js.org/).

Thankfully, with this done, most Markdown can be pasted freely into the editor and should be parsed just fine!