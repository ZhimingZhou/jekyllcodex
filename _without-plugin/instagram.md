---
title: Instagram
---

### Introduction

This script displays the instagram feed of a user. The script reads an RSS feed of your instagram account, provided by [Zapier](https://zapier.com).

{% include instagram.html feedUrl="https://zapier.com/engine/rss/2502510/instagramnew" %}

### How it works

This script loads loads an RSS feed from Zapier and requires just one variable: your Zapier feed URL. To obtain the Zapier feed URL, just create a Zapier account and create [this zap](https://zapier.com/apps/instagram/integrations/rss). Set the following fields: 

- Feed Title: {username}
- Max Records: 5
- Item Title: Caption: {Caption}
- Source URL: {Permalink}
- Content: Tags:
- Media URL: {Media URL}
- Media MIME Type: image/jpeg
- Pubdate: {Timestamp}

### Installation

Step 1. Download the file [instagram.html](https://raw.githubusercontent.com/jhvanderschee/jekyllcodex/gh-pages/_includes/instagram.html)
<br />Step 2. Save the file in the '_includes' directory of your project
<br />Step 3. Add the following line to your layout on the place where you want your instagram pictures to appear:

```
{% raw %}{% include instagram.html feedUrl="https://zapier.com/engine/rss/2502510/instagramnew" %}{% endraw %}
```
