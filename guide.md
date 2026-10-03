---
title: User guide — Bulk Page Restrictions for Confluence
---

# User guide

Bulk Page Restrictions changes the **view** and **edit** restrictions of a page and everything below it in one step. Nothing changes until you have reviewed a preview and confirmed it, and every change can be undone.

## Where to find it

| Where | Who sees it | What you can do |
|---|---|---|
| Page **•••** menu → **Bulk restrictions for this page tree** | Anyone who can view the page | Change the tree below that page; see your own changes |
| **Space settings → Integrations → Bulk Page Restrictions** | Space admins | Change any tree in the space, run the space audit report, see every change made in the space |
| **Confluence administration → Bulk Page Restrictions** | Confluence admins | Everything above, for any space |

The app always works with **your own Confluence permissions**. Pages you can't see are not listed; pages you can't edit are skipped and reported.

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

### Why you appear on restrictions

Confluence requires the person who changes a restriction to be named on it. When a change writes a restriction you are not on, you are added to it; the preview shows this as **+ you**. To remove yourself afterwards, ask another admin to remove you.

### Safety checks

- Each page is read again just before it is changed. If its restrictions changed after the preview, the page is left alone and reported as *changed since preview*.
- Pages with 200 or more people or groups in one restriction are left alone.
- You can't remove or replace yourself.

## Undo

Open the change (it is shown after it finishes, or from **History**) and select **Undo this change**. Each page is put back to its restrictions before the change. If a page was changed again after your change, undo leaves it alone and reports it. Because of the Confluence rule above, you stay on restrictions that undo writes.

## CSV report

**Download CSV report** lists every page with its view and edit restrictions before and after, the result, and any error.

## Audit report

**Audit report** (space settings and Confluence administration) scans a space and lists every page that has a view or edit restriction, or inherits a view restriction from a page above it, with the people and groups on each. It is read-only and works even when the licence isn't active. Download it as CSV for access reviews.

Only pages you can see are included — Confluence hides pages restricted from you from apps as well.

## History and data

Changes are kept for 30 days and then deleted automatically. See the [privacy policy](privacy.html).
