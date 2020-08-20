# Wordpress Redirection plugin configuration for `www.openactive.io`
This repository contains version-controlled configuration for the [Redirection Plugin](https://redirection.me/) within the www.openactive.io Wordpress website.

- [JSON Configuration](/redirection.json)

## Contribution

To make changes to the redirect configuration of www.openactive.io, simply propose a PR for the proposed change.

The `master` branch represents the current state of redirects on the live website.

## Deployment

To deploy updates to the website redirection configuration, follow the steps below:

1. Download [redirection.json](/redirection.json) from the `master` branch.
2. Delete the "https://github.com/openactive/website-redirection/" group from within the [Groups page of the Wordpress Redirection Plugin](https://www.openactive.io/wp-admin/tools.php?page=redirection.php&sub=groups).

![Delete existing redirections](guide-images/delete-group.png)

3. Import `redirection.json` in the [Import/Export page of the Wordpress Redirection Plugin](https://www.openactive.io/wp-admin/tools.php?page=redirection.php&sub=io)

![Import redirections from GitHub](guide-images/import.png)

4. Click "Purge All Caches" in the [WP Engine General Settings page](https://www.openactive.io/wp-admin/admin.php?page=wpengine-common).

![Clear Cache](guide-images/clear-cache.png)
