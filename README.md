# Fansrite

### What is fansrite?

FansRite is a Flat-File Content Management System concept of mine I've had for years now. This version is currently in alpha.

### What does it do?

- Blog/Updates
  - Archive System
- Page Management
  - Automaticly make links in the menu
- Fanshrines
  - List all fanshrines on one page
    - Categorize by type, favorite, page or site, ect
    - link to each fanshrine
- Fanlistings
  - Joined Fanlistings
    - list in pages, in categories
    - Button management
  - Owned Fanlistings
    - Members list, accessable with a password
      - Sort by Country, Favorite Characters or Types
    - Joining Form
    - Code/Button Sorting
    - Emails on Join
- Gallery System
  - DIsplay any images or scans with ease integrated directly into your websites theme
    - Uses lightbox to enlarge these images without leaving the page
  - Handle sub-galleries
    - link these subgalleries to specific shrines or pages
  - Interpret descriptions from a `desc.txt` in the gallery folder

### What doesn't it do?

- Make descriptions for you

- Have a web-based GUI, everything is still serverside for now.

- Use databases to store data

- Track people.

### File System Skeleton

This is just a rundown on how page structure would look.

```
/ files /
|---    / img /
|---    / fonts /
|---    / js / (if needed)
|---    / css / (if needed)
|---    style.css
|---    webmin.js
|---    header.htm
|---    footer.htm
|---    core.php
|---    info.webmanifest.json
/ content / 
|---    / img /
|---    / news /
|-------    news.processor.php
|-------    newslist.json
|-------    newsdate1.md
|-------    newsdate2.md ect...
|---    / pages /
|-------    / section1 /
|-------    / section2 /
|-------    page.processor.php
|-------    pagelist.json
|-------    page1.md
|-------    page2.md ect...
|---    / galleries /
|-------    / subgallery1 /
|-------    / subgallery2 / ect...
|-------    gallerylist.json
|   index.php
|   section1.php
|   section2.php
```

Currently this github version has a seperate skeleton as im trying to figure things out... 
