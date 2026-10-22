<!-- Fill in the three bracketed placeholders before publishing: [YOUR NAME OR COMPANY], [YOUR EMAIL], [EFFECTIVE DATE]. -->

# SALESFORCE Quick Access: Privacy Policy

**Effective date:** 9th Oct, 2026   
**Publisher:** Kiran Patel
**Contact:** patelkiran3090@gmail.com

## In short

- Salesforce Quick Access has no servers of its own. The publisher does not receive, collect, store, share or sell any of your data.
- The extension works only with the Salesforce orgs you are logged into. Its requests go to those orgs and nowhere else.
- Your settings are stored in your browser, on your device.
- There is no analytics, advertising, tracking or telemetry.

## What the extension accesses, and why

| What | Why | What happens to it |
| --- | --- | --- |
| Your Salesforce session cookie (`sid`). This is authentication information. | To make requests to your Salesforce org as you, and, for Quick Deploy, to see which orgs you are logged into. | Used only in requests to the org it belongs to. It is never written to storage, never displayed, and never sent to the publisher or anyone else. |
| The web addresses of your open Salesforce tabs. | To know which org and record you are working in, and to open and reload tabs. | Not stored, apart from the org hostnames described below. Tabs that are not on a Salesforce domain are ignored. |
| Data from your Salesforce org that you ask to see: records and their fields, users, metadata (such as Apex classes, flows and profiles), and debug logs. | To show it to you, and to carry out the actions you ask for. | Shown in the extension on your device. This data can include personal information about your customers or colleagues. Changes you ask for (editing a field, changing owners, granting access, deploying) are sent to your Salesforce org. |
| Text you paste into the JSON beautifier or string converter. | To format or convert it. | Processed on your device. Not stored and not sent anywhere. |
| Your clipboard. | Only when you click Paste from Clipboard (read) or a Copy button (write). | Used for that action only. |

## Where your data goes

- **To Salesforce only.** Requests go over HTTPS to the Salesforce org or orgs you are logged into.
- **Quick Deploy.** It reads components from the org you are in and writes them to the target org you choose. Both are your orgs, and the data goes directly from your browser to Salesforce. It does not pass through any server of ours.
- **Files you download.** The backup file from Change Owner and any raw debug log you download are saved to your computer by your browser.
- **Nothing is sent to the publisher or to any third party.**

## What is stored on your device

**Local storage** stays until you uninstall the extension or clear its data:

- your theme (light or dark)
- the items you pinned, for each org
- your Clear Cache preferences
- each org's company name and whether it is a sandbox
- a list of Salesforce org hostnames the extension has seen, with a label and a last-seen time, so it can show that a session has expired

**Session storage** is held in the browser's memory and cleared when you close the browser:

- the progress of a running Quick Deploy or Change Owner job (component names, status, and the record IDs of a planned owner change)
- which tabs have Clear Cache switched on
- which pop-out windows are open

The extension does not use Chrome sync storage. Nothing stored contains passwords or session credentials.

## Clear Cache

When you turn Clear Cache on for a tab, or click Clear now, the extension removes cached data for your Salesforce origin (Cache Storage, and optionally IndexedDB and localStorage) and asks Salesforce for fresh copies of the files that tab loads. It does not remove cookies, saved passwords, browsing history, or data belonging to any other site.

## Permissions

| Permission | Used for |
| --- | --- |
| `cookies` | Reading the Salesforce session cookie, and listing the orgs you are logged into |
| `tabs` | Finding your Salesforce tabs, opening and reloading tabs, and keeping one pop-out window per org |
| `storage` | Saving the settings described above |
| `clipboardRead`, `clipboardWrite` | The Paste and Copy buttons |
| `browsingData`, `declarativeNetRequestWithHostAccess` | Clear Cache |
| Access to Salesforce domains | Calling your org's APIs, and showing the Inspect tab on record pages |

The extension requests no access to any site outside Salesforce.

## What we do not do

- We do not sell, rent or share your data.
- We do not use your data for advertising or profiling.
- We do not use your data to determine creditworthiness or for lending purposes.
- We do not collect analytics or track your usage.
- We do not load or run code from remote servers.
- No person at the publisher can read your data, because the publisher never receives it.

## Limited Use disclosure

The use of information received from your browser and from your Salesforce orgs by Salesforce Quick Access adheres to the Chrome Web Store User Data Policy, including the Limited Use requirements. The extension uses this information only to provide the user-facing features described on its Chrome Web Store page. It does not transfer the information to anyone except as needed to provide those features (requests to your own Salesforce org) or to comply with the law. It does not use the information for advertising, and no person at the publisher reads it.

## Security

Requests to Salesforce use HTTPS. The session cookie is used in memory only while a request is made. The extension asks for access only to Salesforce domains.

## Your choices

Uninstalling the extension removes everything it has stored on your device. You can also clear its stored data from Chrome's extension settings, and you can unpin items or turn off Clear Cache at any time.

## Children

Salesforce Quick Access is a tool for Salesforce developers and administrators and is not directed to children.

## No affiliation with Salesforce

Salesforce Quick Access is not affiliated with, endorsed by, or sponsored by Salesforce, Inc. Salesforce is a trademark of Salesforce, Inc. Your use of Salesforce is governed by your own agreement with Salesforce.

## Changes to this policy

If the extension changes what data it handles, this policy and its effective date will be updated before the change is released.

## Contact

Questions about this policy: patelkiran3090@gmail.com
