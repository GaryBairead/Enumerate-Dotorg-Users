# Enumerate-Dotorg-Users

A bash script to find usernames for self-hosted WordPress sites.

WordPress creates a unique ID for each author sequentially.

This script enumerates through the "ugly" permalink version of author archives to find usernames for ID's 1-20.

For example, the first author on a site usually has an ID of 1. The author archive for that user will exist at https://domain.com/?author=1

Once we have an author archive URL, we can find the username.

## How to use the script ##

Change the site URL from https://domain.com to your own domain.

Copy & paste the [bash one liner](https://github.com/GaryBairead/Enumerate-Dotorg-Users/blob/master/enumerate) into a terminal, then hit Enter.

## Limitations ##

Not really suitable for multisite networks or WordPress.com

Some security plugins prevent usernames from being enumerated.
