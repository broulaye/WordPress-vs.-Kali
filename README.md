# Project 7 - WordPress Pentesting

Time spent: 8 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Authenticated Stored Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2.2
    - Fixed in version: 4.2.3
  - [x] GIF Walkthrough: <img src='http://i.imgur.com/MiScZgQ.gif' title='Video Walkthrough' width='' alt='Vulnerability 1' />
  - [x] Steps to recreate: -	The following code “<a href="[caption code=">]</a><a title=" onmouseover=alert(document.cookie)">link</a>” passed in as a post can allow a user to run JavaScript code on WordPress.
  - [x] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
2. Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: WordPress 4.2.2
    - Fixed in version: WordPress 4.2.3
  - [x] GIF Walkthrough: <img src='http://i.imgur.com/nwT2XZe.gif' title='Video Walkthrough' width='' alt='Vulnerability 2' />
  - [x] Steps to recreate: -	Embed the following "[embed src='https://youtube.com/embed/1234\x3csvg onload=alert(1)\x3e']  [/embed]" into a post
  - [x] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)
3. Authenticated Cross-Site Scripting (XSS) via Media File Metadata
  - [x] Summary:
    - Vulnerability types: XSS
    - Tested in version: WordPress 4.2.2
    - Fixed in version: 4.2.13
  - [x] GIF Walkthrough: <img src='http://i.imgur.com/Vtj01cD.gif' title='Video Walkthrough' width='' alt='Vulnerability 3' />
  - [x] Steps to recreate: Create an MP3 file with javascript inserted in the meta information, upload MP3 file to the Media Library and and insert an Audio Playlist in a Post containing this MP3
  - [x] Affected source code:
    - https://github.com/WordPress/WordPress/commit/28f838ca3ee205b6f39cd2bf23eb4e5f52796bd7
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

    Copyright 2017 Broulaye Doumbia

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
