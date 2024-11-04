# Instagram-Saved-Links-Dump
A browser console script to dump Instagram saved reels links for easy download ;)


```js
(async () => {
    for (let i = 0; i < 10; i++) {
        window.scrollTo(0, document.body.scrollHeight);
        await new Promise(resolve => setTimeout(resolve, 1000))
    }
    const links = Array.from(document.querySelectorAll("a.x1i10hfl.xjbqb8w.x1ejq31n.xd10rxx.x1sy0etr.x17r0tee.x972fbf.xcfux6l.x1qhh985.xm0m39n.x9f619.x1ypdohk.xt0psk2.xe8uvvx.xdj266r.x11i5rnm.xat24cr.x1mh8g0r.xexx8yu.x4uap5.x18d9i69.xkhd6sd.x16tdsg8.x1hl2dhg.xggy1nq.x1a2a7pz._a6hd"))
        .map(element => element.href)
        .filter(href => href.includes("/p/"));
    console.log(links);
    return links;
})();

```
# Usage
* Goto your instagram saved posts
* Press F12 and click console
* Paste the above script and hit enter
* After its done running your links will be logged in the console
