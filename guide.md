---
title: User guide — Bulk Page Restrictions for Confluence
---

# User guide

Bulk Page Restrictions changes the **view** and **edit** restrictions of a page and everything below it in one step. Changes are written after you confirm the preview. Undo is available within 30 days for eligible changes.

## Where to find it

| Where | Who sees it | What you can do |
|---|---|---|
| Page **•••** menu → **Bulk restrictions for this page tree** | Anyone who can view the page | Change the tree below that page; see your own changes |
| **Space settings → Integrations → Bulk Page Restrictions** | Space admins | Change any tree in the space, run the space audit report, see every change made in the space |
| **Confluence administration → Bulk Page Restrictions** | Confluence admins | Everything above, for any space |

The app always works with **your own Confluence permissions**. Pages you can't see are not listed; pages you can't edit are skipped and reported.

[Follow the first-change walkthrough](first-preview.html) for a small practice run.

## Make a change

1. Choose the **top page**. The change covers that page and every page, folder, whiteboard and database below it — at any depth.
2. Choose what to do:
   - **Add** a person or group to the restrictions. By default, pages that have no restriction today are left open, so adding someone never locks a page by accident. Choose *Restrict them to this person or group too* only if you want those pages restricted.
   - **Remove** a person or group. When the last name is removed from a restriction, the restriction disappears and the page is open to everyone with access to the space.
   - **Replace** one person or group with another — for example when someone leaves the company or a team is renamed. Only restrictions that name the first person or group are changed.
   - **Copy from top page** — give every page below the top page exactly the same restrictions as the top page.
   - **Remove all** view and/or edit restrictions.
3. Choose **View and edit**, **View only** or **Edit only**.
4. Select **Preview changes**. The app reads every page and shows, for each one, who is on the view and edit restrictions today and after the change (added names in green, removed names struck through).
5. Untick any page you want to leave alone, then **Apply** and confirm.

Keep the window open while the change runs. If it closes, open the change from **History** and select **Resume** — it continues where it stopped.

## Add a user to all restricted pages across spaces

Use this when someone needs access to every restricted page in several spaces at once, for example a new auditor, manager or IT admin. Available in **Confluence administration → Bulk Page Restrictions** (version 2.18 and later).

1. On **Change restrictions**, next to *Add someone to every restricted page across spaces*, select **Choose who and which spaces**.
2. **Who to add:** pick a person or a group.
3. **Which spaces:** select **All spaces**, or tick the spaces you want (up to 100; use the filter to find them).
4. Select **Find restricted pages**. The app checks every page, folder, whiteboard and database in those spaces, at any depth, and keeps only the pages that have a **view restriction of their own** and don't list that person or group yet.
5. The preview shows one row per space: how many restricted pages will change, how many already list the person, and example page titles. The page list below shows every page with its space. Untick any page to leave it alone.
6. Select **Apply** and confirm once. All spaces are done in the same run.

What it changes and what it leaves alone:

- Pages **without** a view restriction stay open. Nothing new gets restricted.
- Edit restrictions are not touched.
- A page that only inherits a view restriction from a page above it is not changed: the person gets access through the page above, which is restricted itself and is changed.
- Pages restricted so that **you** can't see them can't be found, because the app works with your own permissions. Ask the page owner or a space admin for access first.
- Confluence keeps the person who changes a restriction on it, so you may be added to some pages (shown as **+ you**).

To take the whole run back, open it from **History** and select **Undo this change**. A large run continues in small steps; if the window closes, open it from **History** and select **Resume**.

## Edit restrictions on a page tree

Confluence carries parent **view** restrictions down the tree. Each page has its own **edit** restrictions. A space-level edit restriction applies throughout the space. See [Atlassian’s guide to inherited restrictions](https://support.atlassian.com/confluence-cloud/docs/add-or-remove-page-restrictions/#How-inherited-restrictions-work).

Bulk Page Restrictions writes the selected changes when you click **Apply** and confirm. Start a fresh preview to include a newly created or moved page, or to copy later changes from the top page.

**Copy from top page** replaces the selected restriction lists below that page. It can give more people edit access to a child with stricter settings. Compare the before and after lists in the preview and untick any exception. Choose **Edit only** to leave view restrictions unchanged.


### Why you appear on restrictions

Confluence requires the person who changes a restriction to be named on it. When a change writes a restriction you are not on, you are added to it; the preview shows this as **+ you**. To remove yourself afterwards, ask another admin to remove you.

### Safety checks

- Each page is read again just before it is changed. If its restrictions changed after the preview, the page is left alone and reported as *changed since preview*.
- Pages with 200 or more people or groups in one restriction are left alone.
- You can't remove or replace yourself.

## Undo

Open the change (it is shown after it finishes, or from **History**) and select **Undo this change**. Undo restores the previous restrictions where possible. If a page was changed again after your run, undo leaves it alone and reports it. Because of the Confluence rule above, you stay on restrictions that undo writes.

## CSV report

**Download CSV report** lists every page with its view and edit restrictions before and after, the result, and any error.

## Audit report

**Audit report** (space settings and Confluence administration) scans a space and lists every page that has a view or edit restriction, or inherits a view restriction from a page above it, with the people and groups on each. It is read-only and works even when the licence isn't active. Download it as CSV for access reviews.

Only pages you can see are included — Confluence hides pages restricted from you from apps as well.

## History and data

Changes are kept for 30 days and then deleted automatically. See the [privacy policy](privacy.html).
