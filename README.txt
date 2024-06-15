Basic Operators

    site:
        Usage: site:example.com
        Description: Restrict results to a specific site or domain.

    intitle:
        Usage: intitle:"login"
        Description: Find pages with a specific word in the title.

    allintitle:
        Usage: allintitle:login password
        Description: Find pages with all the specified words in the title.

    inurl:
        Usage: inurl:admin
        Description: Find pages with a specific word in the URL.

    allinurl:
        Usage: allinurl:admin login
        Description: Find pages with all the specified words in the URL.

    intext:
        Usage: intext:"confidential"
        Description: Find pages with a specific word in the text.

    allintext:
        Usage: allintext:username password
        Description: Find pages with all the specified words in the text.

    filetype:
        Usage: filetype:pdf
        Description: Search for files of a specific type.

    ext:
        Usage: ext:txt
        Description: Search for files with a specific extension.

Advanced Operators

    cache:
        Usage: cache:example.com
        Description: View Google's cached version of a page.

    link:
        Usage: link:example.com
        Description: Find pages that link to a specific URL.

    related:
        Usage: related:example.com
        Description: Find pages similar to a specified URL.

    info:
        Usage: info:example.com
        Description: Get information about a specific URL.

    define:
        Usage: define:cybersecurity
        Description: Find definitions of words.

    * (Wildcard)
        Usage: "security * testing"
        Description: Acts as a placeholder for any word or phrase.

Combining Operators

    Quotes (" "):
        Usage: "error message"
        Description: Search for an exact phrase.

    Minus (-):
        Usage: password -example
        Description: Exclude results containing a specific word or phrase.

    OR:
        Usage: login OR register
        Description: Search for one or more terms.

    Range (..):
        Usage: 2000..2024
        Description: Search within a range of numbers.

Specific Dorking Commands for Security Searches

    Login Pages:
        Usage: site:example.com inurl:login
        Description: Find login pages on a specific site.

    SQL Files:
        Usage: filetype:sql "insert into"
        Description: Find SQL files containing the phrase "insert into".

    Admin Pages:
        Usage: inurl:admin filetype:php
        Description: Find PHP admin pages.

    Directory Listings:
        Usage: intitle:"index of" "parent directory"
        Description: Find directory listings.

    Confidential Documents:
        Usage: intext:"confidential" filetype:pdf
        Description: Find confidential PDF documents.

    Backup Files:
        Usage: filetype:bak
        Description: Search for backup files.

    Configuration Files:
        Usage: filetype:cfg intext:password
        Description: Find configuration files with passwords.

    Database Dumps:
        Usage: intitle:"index of" "database.sql"
        Description: Find directory listings of database dumps.

Practical Use Cases

    Finding Login Portals:
        Usage: inurl:login
        Description: Locate login pages.

    Discovering Vulnerable Files:
        Usage: filetype:log
        Description: Search for log files.

    Searching for Specific Data in Files:
        Usage: filetype:xls intext:"password"
        Description: Find Excel files containing "password".

    Exploring Directory Listings:
        Usage: intitle:"index of /"
        Description: Locate directory listings.

Miscellaneous Useful Dorks

    WordPress Admin:
        Usage: inurl:wp-admin
        Description: Find WordPress admin pages.

    Sitemaps:
        Usage: filetype:xml sitemap
        Description: Find XML sitemaps.

    Sign Up Pages:
        Usage: inurl:signup
        Description: Locate signup pages.

    Error Messages:
        Usage: intitle:"Error" "SQL syntax"
        Description: Find SQL error pages.

    phpMyAdmin:
        Usage: inurl:"/phpmyadmin"
        Description: Find phpMyAdmin pages.
