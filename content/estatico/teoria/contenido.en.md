---
title: "Add content"
date: 2021-11-07T20:44:12+01:00
draft: false
weight: 11
---
**Add content to pages**
> To add content you have to generate text pages with ** markdown ** format
```
Creating content pages
```
**It is important to establish well the organization of the contents**
+ Create chapter or section directories. You can include a _index.md file
+ Create content files with the command `hugo new section_name / file_name.md`
+ The files are created in the ** content ** folder of the site's root directory
+ Sections or chapters have a default content specified in `archetypes / chapter.md`
+ The files have a default content specified in `archetypes / default.md`
+ Each file created has the **front matter** at the beginning, enclosed between two blocks of 3 lines - - -
+ **Taxonomies** allow you to classify content. By default, hugo adds the taxonomies **categories** and **tags**

