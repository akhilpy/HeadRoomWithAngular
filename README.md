# HeadRoomModuleWithAngular

# What is HeadRoom.

Headroom.js is a lightweight, high-performance JS widget (with no dependencies!) that allows you to react to the user's scroll. 
HeadRoom.js works with plainJS and Jquery too. But here we implement with AngularJS.

# Whats Need to include.
1.Angular main JS file.

2.HeadRoom main JS file.

3.angular.HeadRoom JS file. 

All files are included with this repository. You may include these  with any CDN services.


# How to include HeadRoom module.

`angular.module('app', ['app',
'headroom'
]);` 

And  use directive "headroom" as element or attribute in your HTML code.

`<header headroom></header>
<!-- or -->
<headroom></headroom>
<!-- or with options -->
<headroom tolerance="0" offset="0" scroller=".my-scroller" classes={pinned:'headroom--pinned',unpinned:'headroom--unpinned',initial:'headroom'}></headroom>`

# How to manage CSS.
This means you will need some CSS to achieve the effect you want. For example, you could hide the header on scroll down, and reveal it again on scroll up. The most basic CSS for this would be:

headroom--pinned {
    display: block;
}

.headroom--unpinned {
    display: none;
}

.headroom {
    will-change: transform;
    transition: transform 200ms linear;
}
.headroom--pinned {
    transform: translateY(0%);
}
.headroom--unpinned {
    transform: translateY(-100%);
}

PS- This repository created for only educational purpose with the help of HeadRoomJS's official page.  
