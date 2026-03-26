# Troubleshooting Document Save Issues

If your document changes are disappearing or not saving correctly, follow the steps below to diagnose and resolve the issue.

## Symptoms

* Changes you made to a document disappear after saving or navigating away.
* You see a brief error or the page reloads unexpectedly while editing.
* Version history does not show your recent changes.
* The browser console shows `Uncaught (in promise)` errors or `401 (Unauthorized)` responses.

## Common Causes

### Session Expiry During Editing

Vissibl uses short-lived access tokens for security. If your session token expires while you are editing a document, save requests may fail silently. The token is refreshed automatically, but changes made during the brief expiry window may not be saved.

**What happens:**

1. Your access token expires while the document editor is open.
2. You press save (or auto-save triggers), but the request is rejected with a `401 Unauthorized` error.
3. The token refreshes successfully, but the original save is not retried.
4. Your changes are lost because they were never persisted to the server.

### Browser Extension Interference

Some browser extensions (password managers, ad blockers, privacy tools) can interfere with the application's network requests. A common sign is repeated `Uncaught (in promise)` errors in the browser console with the message:

> A listener indicated an asynchronous response by returning true, but the message channel closed before a response was received

This error originates from browser extensions, not from Vissibl itself, but it can occasionally disrupt save operations.

## How to Resolve

### 1. Refresh Your Session Before Editing

If you have been idle for more than a few minutes, refresh the page before making changes. This ensures your access token is current.

### 2. Save Frequently

Use **Ctrl+S** (or **Cmd+S** on Mac) regularly while editing. If a save fails, you will still have the content in your editor and can retry.

### 3. Check for Save Confirmation

After saving, watch for a save confirmation indicator. If you do not see one, try saving again after a brief pause.

### 4. Disable Interfering Browser Extensions

Try editing in an **incognito/private browsing window** (with extensions disabled) to rule out browser extension interference.

### 5. Keep Only One Tab Open

Having multiple Vissibl tabs open can cause session conflicts where one tab's token refresh invalidates another tab's session. Edit documents in a single tab.

### 6. Check Your Network Connection

A dropped or unstable internet connection can cause save failures. Ensure you have a stable connection while editing.

## If the Issue Persists

If you continue to experience lost changes after following the steps above, please contact support with the following information:

* Your account email address.
* The document you were editing.
* The approximate time the issue occurred.
* A screenshot of any errors in the browser console (press **F12** to open developer tools, then select the **Console** tab).

See [Contacting Support](contacting-support.md) for how to reach us.
