---
title: Remove YouTube Shorts from your YouTube feed.
---

As you may know, YouTube has added a new feature called "Shorts", which is basically a TikTok clone, and it's addictive and annoying as hell.

Prerequisite:<br>uBlock Origin extension installed on your browser.

1. Open uBlock Origin dashboard.
2. Navigate to 'My filters' tab.
3. Paste this filters from [letsBlock.it](https://letsblock.it/filters/youtube-shorts):
```
! YouTube Short Remover
www.youtube.com##ytd-guide-renderer a.yt-simple-endpoint path[d^="M10 14.65v-5.3L15 12l-5 2.65zm7.77-4.33"]:upward(ytd-guide-entry-renderer)
www.youtube.com##ytd-mini-guide-renderer a.yt-simple-endpoint path[d^="M10 14.65v-5.3L15 12l-5 2.65zm7.77-4.33"]:upward(ytd-mini-guide-entry-renderer)
www.youtube.com##ytd-browse #dismissible ytd-rich-grid-slim-media[is-short]:upward(ytd-rich-section-renderer)
www.youtube.com##ytd-browse[page-subtype="home"] .ytd-thumbnail[href^="/shorts/"]:upward(ytd-rich-item-renderer)
www.youtube.com##ytd-browse[page-subtype="subscriptions"] .ytd-thumbnail[href^="/shorts/"]:upward(ytd-grid-video-renderer,ytd-rich-item-renderer)
www.youtube.com##ytd-search .ytd-thumbnail[href^="/shorts/"]:upward(ytd-video-renderer)
www.youtube.com##ytd-watch-next-secondary-results-renderer .ytd-thumbnail[href^="/shorts/"]:upward(ytd-compact-video-renderer,ytd-shelf-renderer)
www.youtube.com##ytd-watch-next-secondary-results-renderer ytd-reel-shelf-renderer
www.youtube.com##ytd-browse[page-subtype="subscriptions"] ytd-video-renderer .ytd-thumbnail[href^="/shorts/"]:upward(ytd-item-section-renderer)
www.youtube.com##ytd-browse[page-subtype="channels"] #contents.ytd-reel-shelf-renderer:upward(ytd-item-section-renderer)
www.youtube.com##ytd-browse[page-subtype="trending"] .ytd-thumbnail[href^="/shorts/"]:upward(ytd-video-renderer)
www.youtube.com##ytd-search #contents ytd-reel-shelf-renderer
m.youtube.com##ytm-reel-shelf-renderer
m.youtube.com##ytm-pivot-bar-renderer div.pivot-shorts:upward(ytm-pivot-bar-item-renderer)
m.youtube.com##ytm-browse ytm-item-section-renderer ytm-thumbnail-overlay-time-status-renderer[data-style="SHORTS"]:upward(ytm-video-with-context-renderer)
m.youtube.com##ytm-browse ytm-item-section-renderer ytm-thumbnail-overlay-time-status-renderer[data-style="SHORTS"]:upward(ytm-compact-video-renderer)
m.youtube.com##ytm-search ytm-thumbnail-overlay-time-status-renderer[data-style="SHORTS"]:upward(ytm-compact-video-renderer,ytm-video-with-context-renderer)
m.youtube.com##ytm-single-column-watch-next-results-renderer ytm-thumbnail-overlay-time-status-renderer span:has-text(/^(0:\d\d|1:0\d)$/):upward(ytm-video-with-context-renderer)
youtube.com##ytd-rich-grid-row, #contents.ytd-rich-grid-row:style(display:contents !important;)
```
4. Click 'Apply changes' and you're done.
5. Enjoy your Shorts-less YouTube feed. (:


!!!info "Credits & More Filters"
    This filters are not mine, I just found it on [letsBlock.it](https://letsblock.it/) and thought it would be useful to share it here.<br>
    More filters can be found on their website.