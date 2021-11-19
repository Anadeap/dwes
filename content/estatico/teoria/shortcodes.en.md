---
title: "Shortcodes"
date: 2021-11-07T20:45:32+01:00
draft: false
weight: 12
---
### EXAMPLES OF SHORTCODES
> A **shortcode** is a snippet of html code that will be rendered inside an md file when the system loads or renders the content page
1. **Buttons**  
_Button that links to hugo_'s website 
{{% button href="https://gohugo.io/" icon="fas fa-download" %}}Web de hugo{{% /button %}}

***
2. **Attachments - download pages**
| Page | Attachments location |
| ------ | ---------------------- |
| md | in directory with the same page name and ending in .files |
| directory | in a nested files directory |   
   
{{%attachments title="Attachments" style="orange" /%}} 
***
3. **Shorten a text with read more ...**
Click on the text to expand
{{% expand "Hugo is one of the most popular open source static site generators." %}} With his incredible speed and flexibility, Hugo makes website building fun again. {{% / expand%}}
***
4. **Highlighted texts**
News
{{% notice note%}}
News
{{% / notice%}}
Information
{{% notice tip%}}
Information
{{% / notice%}}
Notice
{{% notice warning%}}
Notice
{{% / notice%}}
***
5. **Tabs of different elements**
Very useful for providing code snippets for multiple languages ​​or providing settings in different formats
{{<tabs groupId = "config">}}
{{% tab name = "json"%}}
json
{
  "Hello": "World"
}
`` ''
{{% / tab%}}
{{% tab name = "XML"%}}
xml
<Hello> World </Hello>
`` ''
{{% / tab%}}
{{% tab name = "properties"%}}
`` `` properties
Hello = World
`` ''
{{% / tab%}}
{{</ tabs>}}
***
6. **Link to a youtube video**
{{< youtube 6H0jLIKe0uw >}}

