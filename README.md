# bisu


A "Swiss Army knife" for your /etc/hosts file.

When am working on a project, I usually switch the host entry from development, staging and production e.g.

    127.0.0.1    example.com #devel
    70.85.16.25  example.com #production

As you know, you can only have 1 entry in your host file; so you need to open and edit host file and keep switching. 

Not anymore! Behold **bisu**, a script that add/remove/replace host entry.

## Installation

Just copy the file to `/usr/local/bin/bisu` or any dir that's in your `$PATH`

## Usage

  - `sudo bisu add 127.0.0.1 example.com` - adds `127.0.0.1 example.com` entry in your host file
  - `sudo bisu remove 127.0.0.1 example.com` - removes `127.0.0.1 example.com` entry in your host file
  - `sudo bisu replace 127.0.0.1 example.com 8.8.8.8` - replaces `127.0.0.1 example.com` entry with `8.8.8.8 example.com`
