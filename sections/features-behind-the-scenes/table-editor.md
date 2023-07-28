### Table Editor

The “whole grail of WYSIWYG editing” (as stated in [the TipTap docs](https://tiptap.dev/api/nodes/table#introduction)) took a while to get right. While TipTap provides extensions for supporting Table formatting, the UI is a different story. Table formatting UIs are notoriously difficult to get right. That’s why I was quite happy when I finally felt like I built something that was… alright.

![Table editor](https://assets.vrite.io/6409e82d7dfc74cef7a72e0d/CThF1-P0HI4iWTIWlvQ0s.png)

When your cursor is inside the table, you’ll see a bottom menu appear, which you can use e.g. insert and remove rows, columns, and headers. On the other hand, when you select some cells, you’ll see a menu to e.g. merge, split, or delete them. It’s not Excel-level but, for an inline table, I think it’s pretty good.