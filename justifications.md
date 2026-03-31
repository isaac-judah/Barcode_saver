## Single Purpose

This Chrome extension allows users to store, organize, and manage barcode lists in categorized groups with optional cloud sync. Users can create categories, add/remove barcodes, reorder categories via drag-and-drop, and optionally sync data to a cloud backend for backup and cross-device access.

## Storage Justification

The `storage` permission is required to:
- Persist barcode data locally so users can access their lists offline
- Store session data (login state) to maintain authentication between browser sessions
- Save category order and organization preferences

Without this permission, all data would be lost when the extension is closed or the browser restarts.

## SidePanel Justification

The `sidePanel` permission is used to display the extension's interface in Chrome's side panel. This allows users to quickly access and manage their barcode lists without leaving their current tab, improving workflow efficiency for inventory or store management tasks.

## Host Permissions Justification

The host permission `https://*.supabase.co/*` is required to:
- Connect to Supabase (a cloud database service) for optional data sync
- Authenticate users against their store accounts
- Store and retrieve barcode data from the cloud for backup and cross-device access

This is a minimal wildcard limited to the single Supabase project used by this extension.

## Remote Code

This extension does NOT load or execute any remote code. The `https://*.supabase.co/*` host permission is used only for API calls to a cloud database - all extension logic runs locally in the browser.

## Data Usage

This extension handles the following user data:

| Data Type | Purpose | Storage |
|-----------|---------|---------|
| Store number | User account identification | Local + Cloud |
| Password hash | Authentication (hashed, not plain) | Local + Cloud |
| Category names | Organizing barcodes | Local + Cloud |
| Barcode values | Core functionality | Local + Cloud |

Data is used solely for the stated purpose of barcode list management. No data is sold, shared with third parties, or used for advertising/analytics.