---
title: Run your first bulk restriction change in Confluence
description: Preview a small Confluence page tree, confirm the pages to change, and check the results in Bulk Page Restrictions.
---

# Run your first bulk restriction change in Confluence

Start with a small test tree where you can edit restrictions. For this example, choose a tree with an existing edit restriction and a test group that should be allowed to edit. Preview is read-only. Applying a change requires an active app licence.

## 1. Open it from a page

Page **•••** menu → **Apps** → **Bulk restrictions for this page tree**. The page you open it from is the top of the tree.

![Page menu with Apps and Bulk restrictions for this page tree](img/first-1-menu.jpg)

## 2. Choose the group to add

Choose **Add** and **Edit only**. Under **Choose who to add**, search for your test group and select it. Keep **Leave them open (recommended)** selected so pages without an edit restriction stay open.

![Choosing a group in the Bulk Page Restrictions dialog](img/first-2-pick.jpg)

## 3. Preview and select pages

Click **Preview changes**. Check the number of pages scanned and the number that would change. Read the before and after restrictions in the table, then untick any page you want to leave alone.

![Example preview showing the number of pages checked and ready to change](img/first-3-preview.jpg)

![Preview table with added names in green](img/first-4-table.jpg)

If the preview shows no changes, check whether your group is already listed or the pages lack an edit restriction. Choose an already restricted test page where the group is absent and preview again.

## 4. Apply and check the result

1. Click **Apply to N pages** above the table. Check the count in the confirmation, then choose **Yes, change N pages**.
2. Keep the window open and wait for **Done**. The **Result** column explains skips, including pages whose restrictions changed after the preview. Select **Download CSV report** to keep a record.
3. Check an applied page in Confluence. For a rehearsal, open the completed change or find it in **History** and select **Undo this change** within 30 days. If someone changed a page's restrictions after your run, undo leaves that page alone and reports it.

[Full user guide](guide.html) · [Get setup help](support.html)
