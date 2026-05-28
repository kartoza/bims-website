---
title: BIMS Documentation
summary: Central documentation site for BIMS projects
    - Dimas Ciputra
date: 28-05-2026
some_url: https://github.com/kartoza/bims-website
copyright: Copyright 2023, Kartoza
contact:
license: This program is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
#context_id: 1234
---

# GitHub App Integration

Set up a GitHub App to allow BIMS to automatically create and assign issues in a GitHub repository when users submit data uploads. This guide covers creating the app, generating credentials, installing it on your target repository, and entering the credentials into the BIMS admin.

---

## Create a New GitHub App

If you do not yet have a GitHub App, follow these steps.

### Navigate to App Settings

1. Go to **GitHub.com** and sign in.
2. Click your profile photo (top-right) > **Settings**.
![Profile menu showing Settings option](<img/github-app-setup-1.png>)

3. In the left sidebar, scroll down and click **Developer settings**.
![Left sidebar with Developer settings highlighted](<img/github-app-setup-2.png>)

4. Click **GitHub Apps** > **New GitHub App**.
![GitHub Apps page with New GitHub App button](<img/github-app-setup-3.png>)

### Fill in the App Details

Fill in the required fields on the new app form:
![New GitHub App registration form](<img/github-app-setup-4.png>)

| Field | Value                                                              |
|---|--------------------------------------------------------------------|
| GitHub App name | A unique name, e.g. `BIMS support`                                 |
| Homepage URL | Your project URL or repository URL, .e.g. `https://fbisafrica.org` |
| Webhook | Uncheck "Active"                                                   |

### Set Repository Permissions

Under **Permissions > Repository permissions**, set the following based on what the app needs to do:
![Repository permissions section with permission dropdowns](<img/github-app-setup-5.png>)

| Permission    | Level | When needed                  |
|---------------|---|------------------------------|
| Issues        | Read & write | Open/update issues           |
| Metadata      | Read-only | Required for all repo access |

> Only grant the minimum permissions required.

### Set Where the App Can Be Installed

Under **Where can this GitHub App be installed?**, choose:

- **Only on this account** - if the target repo is in the same org/account.
- **Any account** - if the target repo is in a different org or owned by someone else.

### Create the App

Click **Create GitHub App**. You will be redirected to the app's settings page.

---

## Generate a Private Key

The app needs a private key to authenticate as itself.

1. On the app's settings page, scroll down to **Private keys**.
2. Click **Generate a private key**.
![Private keys section with Generate a private key button](<img/github-app-setup-8.png>)

3. A `.pem` file will be downloaded automatically. Store this securely - it is the app's credential.
Note the **App ID** displayed at the top of the settings page. You will need it alongside the private key.
![App ID displayed at the top of the app settings page](<img/github-app-setup-9.png>)

---

## Install the App on the Target Repository

Installing the app grants it access to specific repositories.

### Install from the App Settings Page

1. On the app's settings page, click **Install App** in the left sidebar.
![Install App option in left sidebar](<img/github-app-setup-10.png>)

2. Click **Install** next to the account or organization that owns the **target repository**.
![List of accounts with Install button](<img/github-app-setup-11.png>)

3. On the installation screen, choose:
   - **All repositories** - grants access to every repo in that account.
   - **Only select repositories** - recommended. Select only the specific target repo.
![Repository access selection screen](<img/github-app-setup-12.png>)

4. Click **Install**.

### Install on a Repository in a Different Organization

If the target repo belongs to a different GitHub organization:

1. The app must have **"Any account"** selected in its installation setting (see step 1.4).
2. Share the app's public link with the org owner, or navigate to:
   ```
   https://github.com/apps/<app-slug>/installations/new
   ```
3. The org owner installs it and selects the target repository.

---

## Update an Existing GitHub App

If you already have a GitHub App and need to add access to a new repository:

### Update Permissions (if needed)

1. Go to **Settings > Developer settings > GitHub Apps**.
2. Click **Edit** on your app.
![GitHub Apps list with Edit button highlighted](<img/github-app-setup-14.png>)

3. Under **Permissions & events**, update the repository permissions as needed.
4. Click **Save changes**.
5. GitHub will notify all existing installations about the permission change. Each installation owner must **approve** the new permissions before they take effect.

---

## Configure BIMS Site Settings

Once your GitHub App is created, installed, and you have the private key, enter the credentials in the BIMS Django admin.

### Open Site Settings

1. Log in to the BIMS admin panel (e.g. `https://your-bims-site/admin/`).
2. Navigate to **Preferences > Site settings**.
3. Scroll to the **GitHub App** section.

![GitHub App section in BIMS Site Settings admin](<img/github-app-setup-bims-admin.png>)

### Fill in the Fields

| Field | Where to find the value |
|---|---|
| **GitHub App ID** | The numeric ID shown at the top of your app's settings page on GitHub (see step 2 above). |
| **GitHub App private key (PEM)** | The full contents of the `.pem` file downloaded in step 2. Paste the entire key, including the `-----BEGIN RSA PRIVATE KEY-----` and `-----END RSA PRIVATE KEY-----` lines. If pasting as a single line, use `\n` for newlines. |
| **GitHub upload repo** | The repository where upload issues are created, in `owner/repo` format (e.g. `my-org/upload-tracker`). The GitHub App must be installed on this repository. |
| **GitHub upload assignees** | Comma-separated GitHub usernames to assign to newly created issues (e.g. `alice,bob`). All listed users must have access to the repository. Leave blank to create unassigned issues. |

> The private key is **encrypted at rest**. After saving, the field shows `******` and the value is never displayed again. To rotate the key, paste the new PEM content and save.

### Save

Click **Save** at the bottom of the page. BIMS will use these credentials to authenticate as the GitHub App and create issues when users submit uploads.

---

## Troubleshooting

| Problem | Cause | Fix |
|---|---|---|
| `Resource not accessible by integration` | App not installed on target repo | Install the app on the target repo (step 3) |
| `Permission denied` | Missing or insufficient permissions | Update app permissions (step 4.1) and approve the change |
| `JWT token invalid` | Wrong App ID or malformed private key | Check that **GitHub App ID** and **GitHub App private key** in Site Settings are correct |
| App works on one repo but not the target | Installation is scoped to a different repo | Reconfigure installation to include the target repo (step 4.2) |
| Org requires approval for third-party apps | Org policy blocks unapproved apps | Org owner must approve the app under org settings |
