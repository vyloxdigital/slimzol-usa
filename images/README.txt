Slimzol — image assets
slimzol-usa.vercel.app

Drop these eight files into this folder, keeping the names exactly as
written. The page references them by these names and nothing else.

  slimzol-3-bottles-guarantee.webp   used TWICE: the hero panel and the
                                     three-bottle price tier. It is the LCP
                                     image and the only preloaded one, so
                                     keep it under ~110 KB. It is also the
                                     og:image when the page is shared.
  slimzol-2-bottles-guarantee.webp   two-bottle price tier
  slimzol-6-bottles-guarantee.webp   six-bottle price tier
  slimzol-review-1.webp              reviews section
  slimzol-review-2.webp              reviews section
  slimzol-review-3.webp              reviews section
  slimzol-guarantee.webp             60-day guarantee seal
  favicon.png                        tab icon and web app icon (512 x 512)

Sizes do not need to match anything

  Every image slot has a fixed CSS aspect-ratio with object-fit:contain,
  so Cumulative Layout Shift stays at zero whatever proportions your
  files happen to be. Nothing is stretched and nothing is cropped; a
  file that does not match its slot is centred inside it instead.

  The slots are:
    hero panel        3:2  on a soft blue-to-cream gradient
    price tier images 1:1  transparent
    review images     4:3  on a pale blue tile
    guarantee seal    1:1  on white

  If you want them to fill the slots edge to edge, supply roughly
  900x600, 400x400, 800x600 and 400x400.

Other notes

  * Serve real WebP, not a renamed PNG or JPEG.
  * The hero panel has its own tinted background, so a product shot with
    a transparent background looks best there. A white-background file
    will show as a white rectangle inside the tint.
  * Only slimzol-3-bottles-guarantee.webp is preloaded. Everything else
    is lazy loaded, which is what holds the PageSpeed score. Do not add
    more preloads.
