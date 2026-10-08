# critical skin api
just a bunch of skins you can use in your apps instead of your own catalog

use crit launcher 
[![Get Crit](https://img.shields.io/badge/Get-crit%20%launcher-red)](https://critlauncher.xyz)
## HOW TO USE
Get the skin index
const folders = await fetch(
  "https://api.github.com/repos/snigglaberry/critical-skin-api/contents/skin"
).then(r => r.json());

This gives you the a, b, c, etc. folders.

Get skins from a letter
const skins = await fetch(
  "https://api.github.com/repos/snigglaberry/critical-skin-api/contents/skin/g"
).then(r => r.json());
Get the skin

Each result has a download_url:

const skinURL = skins[0].download_url;

Or construct it yourself:

https://raw.githubusercontent.com/snigglaberry/critical-skin-api/main/skin/g/Goku.png
