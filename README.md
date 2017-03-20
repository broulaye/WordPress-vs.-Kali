# Project 7 - WordPress Pentesting

Time spent: 8 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Stored Cross-Site Scripting (XSS)
  - [x] Summary:
    - Vulnerability types: XSS
    - Tested in version: WordPress 4.2.2
    - Fixed in version: 4.2.11
  - [x] GIF Walkthrough: http://i.imgur.com/KmUzh1M.png
  - [x] Steps to recreate: Download a theme file and modify the name so it contains some JavaScript code then zip the theme file under the name theme.zip and upload it to WordPress
  - [x] Affected source code:
    - https://github.com/WordPress/WordPress/commit/ce7fb2934dd111e6353784852de8aea2a938b359
1. User Enumeration
  - [x] Summary: 
    - Vulnerability types: User Enumeration
    - Tested in version: WordPress 4.2.2
    - Fixed in version: WordPress 4.2.11
  - [x] GIF Walkthrough: http://i.imgur.com/DqK4F63.png
  - [x] Steps to recreate: -	Attacker can get the list of users, by just entering various user name. enter a random user name, error message will tell you if the username is valid or not.
  - [x] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. Authenticated Stored Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2
    - Fixed in version: 4.2.3
  - [x] GIF Walkthrough: http://i.imgur.com/959oNEl.png
  - [x] Steps to recreate: -	The following code “<a href="[caption code=">]</a><a title=" onmouseover=alert(document.cookie)">link</a>” passed in as a post can allow a user to run JavaScript code on WordPress.
  - [x] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types: 
    - Tested in version: 
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
