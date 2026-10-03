---
title: Privacy Policy — Bulk Page Restrictions for Confluence
---

# Privacy Policy

**App:** Bulk Page Restrictions for Confluence
**Publisher:** Atesen Software (independent developer, Türkiye)
**Contact:** sametatesen2@gmail.com
**Last updated:** 3 October 2026

## 1. What this app does with data

The app runs inside your Atlassian Cloud site on the Atlassian Forge platform. It reads and changes the view and edit restrictions of Confluence pages, folders, whiteboards and databases when a user asks it to, and produces a read-only audit report of restricted pages.

**To show a preview, apply a change, resume an interrupted change and undo it,** the app stores, for each change:

- the Atlassian account ID of the user who started it;
- the change requested (for example "replace person A with person B"), including the account IDs or group IDs and the names of the people and groups chosen;
- for each page in the tree: page ID, title, type, position in the tree, the view and edit restrictions before and after the change (as Atlassian account IDs and group IDs), the result and an error code;
- the display names of the people and the names of the groups that appear in those restrictions, so the preview and CSV report are readable.

**The audit report is not stored.** It is assembled in your browser while you view it and downloaded as a file only if you choose to.

The app does not read page content, comments, attachments, email addresses or user profiles beyond the display name returned with a restriction.

## 2. Where data is stored and where it goes

All processing and storage happen on Atlassian's Forge platform, inside Atlassian's cloud infrastructure (Forge hosted storage). The app has no servers of its own and **makes no requests outside Atlassian**. There are no analytics services, advertising networks or sub-processors, and **no data is sent to Atesen Software**.

## 3. How long data is kept

Change records are deleted automatically **30 days** after the change was started. Once a week the app reports the stored account IDs to Atlassian's personal data reporting service; when Atlassian reports that an account has been closed, that account's ID and name are deleted from all stored changes (undo is then no longer possible for the pages concerned). Uninstalling the app removes the app's storage according to Atlassian's Forge data retention policies.

## 4. Logs

Application logs contain change IDs, counts, HTTP status codes and error codes. **They never contain page titles, names, account IDs or restriction lists.** Forge logs are stored by Atlassian and are visible to the publisher only through Atlassian's developer tooling, with Atlassian's own retention limits.

## 5. Roles

For data processed by this app on your site, your organization is the controller and Atesen Software acts as a processor to the limited extent described here. Atlassian is the infrastructure provider; see Atlassian's privacy policy for how they process data in your cloud site.

## 6. Your requests

To ask about data handled by this app, or to request deletion of change records on your site, write to sametatesen2@gmail.com. Records can also be deleted from the app's **History** tab at any time.

## 7. Security

All Confluence requests run with the permissions of the user who uses the app (Forge `asUser`); the app cannot read or change anything that user cannot. Every change is shown as a preview first, needs an explicit confirmation, re-reads each page before writing it and leaves pages that changed in the meantime alone. Who can see stored changes: the page-by-page details (titles and restriction lists) are shown only to the person who made the change. Confluence administrators see a one-line summary of every change, space administrators of the changes in their space, and either can undo a change with their own permissions.

## 8. Changes

Material changes to this policy are announced in the release notes on the app's Atlassian Marketplace listing.
