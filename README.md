# Search Menu — a PopClip extension

Search the selected text on several sites, from one button.

Select text in any app, click **Search Menu** in the PopClip bar, and pick a site. The
selection is URL-encoded and opened as a search on that site — in your default browser, or
in a specific browser you name. Because the sites sit in a submenu, eight engines take up
one button in the bar instead of eight.

Included: Google, Reddit, Amazon, Google Shopping, AliExpress, YouTube, Maps, Facebook.

## Browser

By default the search opens in your default browser. To send it somewhere else, put a
bundle identifier in the **Browser** option — `com.google.Chrome`, `com.apple.Safari`,
`com.brave.Browser`. Useful if your default browser is routed through something like
Finicky and you want searches to bypass that routing.

## Making it your own

Every entry in `source/Search Menu.popclipext/Config.yaml` is three lines: a title, an icon
and one line of JavaScript holding the search URL. Copy an entry, change the URL, and put
the selection where `encodeURIComponent(...)` sits.

Icons come from [Iconify](https://icon-sets.iconify.design/) via `iconify:simple-icons:<name>`,
or any SF Symbol via `symbol:<name>`. No image files are bundled.

## Requirements

PopClip 2026.7 (build 5992) or later — that is the release that added action submenus.

## Licence

MIT, see [LICENSE](LICENSE).
