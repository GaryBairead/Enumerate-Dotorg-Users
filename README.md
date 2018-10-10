# Enumerate WordPress Usernames

A bash script to find usernames for self-hosted WordPress sites.

WordPress creates a unique ID for each author sequentially.

This script enumerates through the "ugly" permalink version of author archives to find usernames for ID's 1-100.

The first author on a site usually has an ID of 1. The author archive for that user will exist at https://domain.com/?author=1

Once we have an author archive URL, we can then find the username from the Location header.

For example, if the script is run on WPTavern.com, it'll find a user with an ID of 2 at https://wptavern.com/?author=2

That URL then redirects to https://wptavern.com/author/jeffr0

Based on that author archive URL, we now know that jeffr0 is one the usernames/login names.

## How to use the script ##

Change the site URL from https://domain.com to your own domain.

Copy & paste the [bash one liner](https://github.com/GaryBairead/Enumerate-Dotorg-Users/blob/master/enumerate) into a terminal, then hit Enter.

## Limitations ##

- Won't work for WordPress.com sites. WP.com is essentially a giant multisite
- Some security plugins will prevent usernames from being enumerated
