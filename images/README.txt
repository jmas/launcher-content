Icons and backgrounds for content/ menus (paths like images/icons/foo.jpg in JSON).

Refresh after changing sources in scripts/fetch-content-images.sh:

  ./scripts/fetch-content-images.sh

Menu icons are center-cropped to square (YouTube 16:9 thumbs included), resized, and cached
(PNG, rounded corners) under the OS user cache (e.g. ~/Library/Caches/launcher/menu-icons on macOS)
or $TMPDIR/launcher/menu-icons if user cache is unavailable. Backgrounds use …/menu-backdrops.
Override with LAUNCHER_ICON_CACHE_DIR, LAUNCHER_BG_CACHE_DIR, or LAUNCHER_CACHE_DIR (parent of both).
Local files: cache refreshes when the source image is newer.

Clear all prepared icon/background caches:

  ./scripts/clear-menu-image-cache.sh

Sources: YouTube thumbnails (matching descriptor URLs), game art (itch.io / GitHub),
Blender open-movie posters, Wikimedia Commons (NES console, Big Buck Bunny).
Bundled: content/images/sources/flappy-paratroopa-title.png (Flappy Paratroopa menu icon),
content/images/sources/nova-the-squirrel-screenshot.png (Nova the Squirrel menu icon),
content/images/sources/micro-mages-screenshot.png (Micro Mages menu icon),
content/images/sources/super-tilt-bro-versus.png (Super Tilt Bro menu icon),
content/images/sources/famidash-huge-man-screenshot.png (Famidash Huge Man menu icon),
content/images/sources/nes-menu-background.jpg (NES games menu background).
