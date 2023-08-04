### Code Editor

Something that I always felt was lacking in WYSIWYG editors (even the top ones, like [Notion](https://notion.so/)) is good support for **code editing**. Granted, technical writing is a niche use-case and you can get by with simple syntax highlighting and some copy-pasting. That said, I wanted to try something else — I wanted to integrate a full-blown code editor.

![Integrated code editor](https://assets.vrite.io/6409e82d7dfc74cef7a72e0d/NLQ2piOpD-6jOZEtv67gT.png)

By referencing [the ProseMirror docs](https://prosemirror.net/examples/codemirror/), forwarding the editor state back and forth, and adjusting the layout, I managed to integrate [Monaco Editor](https://microsoft.github.io/monaco-editor/) — the web editor extracted from VS Code — together with [Prettier](https://prettier.io/) (for code formatting) right into the Vrite Editor (I know, that’s a lot of editors in one place 😅).

Granted, this is not VS Code in your content editor, but this way you get great syntax highlighting for many languages, while also having formatting and auto-completion for at least a few — like JavaScript or HTML.