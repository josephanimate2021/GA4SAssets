# GoAnimate For Schools Remastered 1.0 Asset Server

## What Is It?
This asset server will be for a project known as GoAnimate For Schools Remastered 1.0 which looks alot like GoAnimate Remastered. while not worth using, some people like myself love to experiment with out of date lvm projects especially like this one to see what it was really like back then because of this "Memory Moment" that my development team at GoNexus brought up.

## How Does An LVM Asset Server Work?

The LVM (Legacy Video Maker) fetches all content from a website that it is assigned to grab stuff from. to give you an example, here is how the LVM Would load:
1. An html tag called object would grab a swf file (go_full.swf) from a website it's assigned to.
2. After a few minutes, you will notice the LVM start to load something known as client theme files. it does this by using a variable in the flashvars known as clientThemePath to grab all contents from the assigned website. Please note that the website needs to be the same while it loads everything. i'll explain later.
3. After all of the client theme files are loaded, the LVM will load something known as the stage. from there, it will call an api to load everything the LVM needs to work. a few seconds later, the LVM will start to load store files for the selected theme using an assigned website that needs to be the same as both the client theme and lvm.

## Why Does The LVM Need To Load Everything From The Same Website?

While this is true for both the swf file (go_full.swf) and client theme files, strangely enough you can assign the lvm to load store files from a completely different website if you wanted. Here is why it is very important that both the swf file (go_full.swf) and client theme files are loaded from the same website:
* If both the swf file (go_full.swf) and client theme files are loaded from the same website, everything should work file.
* if both the swf file (go_full.swf) and client theme files are not loaded from the same website, there will be some messy concerquences for the LVM. one of them includes the LVM not even loading despite good WI-FI connection. You do not want to know other concerquences for not loading both the swf file (go_full.swf) and client theme files are loaded from the same website.

## How do i add this asset server to a config file in an lvm project i downloaded?

In the folder of an LVM project you downloaded, you will add the following to the `config.json` file:
```
{
        "SWF_URL": "https://josephanimate2021.github.io/GA4SAssets/animation/414827163ad4eb60",
        "STORE_URL": "https://josephanimate2021.github.io/GA4SAssets/store/3a981f5cb2739137",
        "CLIENT_URL": "https://josephanimate2021.github.io/GA4SAssets/static/ad44370a650793d9"
}
```
That's pretty much it. Please report any issues in the Issues panel if you are experiencing bugs with this asset server (that is to be expected)
