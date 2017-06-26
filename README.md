# vrops-custom-group-creation
Automatically create custom dynamic groups in vROps server as per vCenter Tags

Purpose:

Do you want to create custom dynamic groups in vROps which matches the tags created in vCenter server? You can do this manually, but you have large number of tags created. How to tackle that programmatically? This post covers the exact point. Read on to know how you can automatically create custom dynamic groups in vROps server. These groups will match the tags created in vCenter server.
Introduction:

Last week I got a request from my friend Sunny Dua about a script which will automatically create custom groups in vROps server as per vCenter server tags. This started me thinking. If you have a large environment and you want to keep it organized, then tags in vCenter server is a must. Also creating dynamic custom groups in vROps matching to these vCenter Tags makes sense. So I created scripts to achieve this. Provided below are details of the scripts.
Purpose of the scripts:

The purpose of the script is two-fold.

    First, it should gather the tag names and tag category names from vCenter
    Second, it would create custom groups in vROps server with matches the following criteria's
        The name of the group is same as the tag names.
        Also the membership of the group is dynamic in nature. Those VM's will be part of a group for which "vSphere Tag" is equal to or contains the tag name/group name
        If a "Group Type" is created in vROps server which is

So essentially you get custom groups in vROps server with names equal to tag names in vCenter server. The members of the group are the respective VM's tagged with tagname.

For more details check the blog at http://vtechguru.com/2017/06/automatically-create-custom-groups-vrops-per-vcenter-tags.html 
