# Salesforce Quick Access

A Chrome extension with everyday Salesforce admin and developer tools, one click away. It works through the Salesforce session you are already signed in with: there is no account to create, no server, and nothing is sent to the developer.

> **Unofficial.** Salesforce Quick Access is an independent product. It is not affiliated with, endorsed by, or sponsored by Salesforce. Salesforce is a trademark of Salesforce, Inc.

[Install for Chrome](https://chromewebstore.google.com/detail/salesforce-quick-access/anjccglcmoocjjaeehdndfcgeajhkbhk) · [Install for Edge](https://microsoftedge.microsoft.com/addons/detail/salesforce-quick-access/dpoglfhjfbdfcaokbaohbaalmdpdpgeg) · [Privacy policy](PRIVACY_POLICY.md)

## What it does

| Tool | What it is for | Changes data? |
|---|---|---|
| **Record Inspector** | Every field of a record in one table (API name, label, type, value). Edit a value in place, follow lookups, read a field's history, and see what uses a custom field. | Only when you edit a field |
| **Data export** | A SOQL editor with suggestions as you type: fields (through parent relationships too), a FIELDS(ALL) shortcut that sets the LIMIT it needs, and a picklist's values after `=`. See the results and download them as a CSV. Click an Id to open the record in the Inspector or in Salesforce, or copy it. Your last 20 queries for each org are kept on your computer so you can run them again. | No |
| **Quick Deploy** | Move a few Apex classes, triggers, Lightning web components, Aura components, Visualforce pages, custom fields, labels, flows, validation rules and custom metadata records to another org you are signed into. Validate first. Deploying to production asks you to type that org's name. | Yes, in the target org |
| **Recent changes** | Which components changed lately, newest first, and who changed them. Opens on your own changes from today and yesterday. Add any of them to Quick Deploy. | No |
| **My work** | Group the components you change for a story or task, add each from Recent changes or search, keep notes and pre- and post-deployment steps, then deploy the whole group through Quick Deploy. Kept on your computer, per org. For teams that don't use branches. | No |
| **Compare access** | How two profiles or permission sets differ. A plain-language answer first, then a matrix of object, system, Apex, Visualforce and custom permissions, and field permissions one object at a time. Export it, or copy it as a checklist. | No |
| **Change owner** | Change the owner of many records. A backup file is created first. | Yes |
| **Grant access** | Add access to Apex classes, pages, fields and objects across profiles and permission sets. | Yes |
| **Cleanup tools** | Find what references a record, delete by ID after previewing what goes with it, remove old flow versions, clear debug logs. | Yes, with confirmation |
| **Log Analyzer** | Turn debug logs into triggers, flows, DML, SOQL and limits, with filters. | No |
| **Clear cache** | Force a fresh load of one tab. | No |
| **Utilities** | A JSON beautifier, a string converter, search everything (`Ctrl+K`), pinned items, and switching between orgs. | No |

Tools that change data say so, and ask you to confirm. Production orgs need an extra confirmation.

## Getting started

1. Install the extension from the Chrome Web Store.
2. Sign in to Salesforce as usual and open any Salesforce page. Refresh it once after installing.
3. Click the toolbar button to open the sidebar, or use the **Inspect** and **Data export** tabs on the right edge of the page.

## Privacy

The extension talks only to the Salesforce org you are using. It has no analytics, no remote configuration and no remotely hosted code. Salesforce records are not stored: only preferences and the state of a running job are. Read the full [privacy policy](PRIVACY_POLICY.md).

## Permissions

| Permission | Why it is needed |
|---|---|
| `cookies` | To read your Salesforce session cookie, so requests are made to your own org as you. It is only ever sent to that org. |
| `tabs` | To find the tab of the org you are using, and to open the Inspector, Data export and Compare access pages beside it. |
| `storage` | To remember your orgs, preferences and pins, your last 20 Data export queries for each org, your My work lists, and the state of a running deployment or owner change. |
| `clipboardRead`, `clipboardWrite` | To paste into the utilities, and to copy results and checklists. |
| `browsingData`, `declarativeNetRequestWithHostAccess` | For the Clear cache tool. |

Access is limited to Salesforce domains. The extension can do only what you can already do in Salesforce.

## Good to know

- It works in Chrome and Edge, and you need to be signed in to Salesforce.
- Compare access compares what each profile or permission set grants explicitly. A permission that implies others (such as Modify All Data) is not expanded.
- If a list can't be read, for example because your user lacks a permission, the extension says which list and gives Salesforce's reason. It does not hide the gap.

## Privacy

The extension uses the Salesforce session you already have open in your browser and talks only to the Salesforce org you are using. It has no analytics and no remote configuration, and it never sends Salesforce data anywhere else. Settings, pins, saved queries and your My work lists are kept on your computer only. The full policy is in [PRIVACY_POLICY.md](PRIVACY_POLICY.md).

## Support

Questions or problems: [open an issue](https://github.com/patelkiran3090/Salesforce-Quick-Access/issues).
