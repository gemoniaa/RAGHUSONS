RAGHUSONS INFRA - cinematic scroll-film website
index.html   the page (Tailwind + fonts load from CDN, so open it with internet on)
frames/      180 frames f001.webp ... f180.webp (1920x1080, JCB exploded view)
extras/      the earlier live Three.js crane version (standalone file)

Run: open index.html, or upload this whole folder to GitHub Pages / Netlify / any host.

How it works: the page is one long pinned scroll. Scroll position drives (1) which frame plays,
(2) a virtual camera that zooms into the bucket, cab, engine and axle, and (3) the text chapters.
Edit the camera in "const K" (p, focus x, focus y, zoom, screen x), the frame timing in "const FM",
and chapter text/ranges in the .ch blocks (data-a / data-b are scroll start/end from 0 to 1).
If you swap the film for a different frame count, change 180 in "F?F.length:180".
