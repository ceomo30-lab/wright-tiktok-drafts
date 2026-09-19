# Direct Post review UI

Prepared but not deployed. It implements TikTok's required per-post preview and control surface. The current carousel is marked demo-only because it has already been posted.

Deployment requires a same-domain HTTPS backend, TikTok production approval, new OAuth consent for `video.publish`, environment secrets, KV/session storage, and a new approved post manifest. Do not place TikTok tokens or client secrets in GitHub Pages or browser JavaScript.

## Batch review

`queue.html` is the lowest-friction compliant batch flow: one review session, one explicit approval checkbox per immutable post/version, visible settings and schedule for every post, then one final confirmation. The backend rejects changed versions. This is not blanket authority for future work.

TikTok's photo Direct Post request is one post per `/content/init/` call and has no scheduled-time field. Scheduling must remain app-side; at the approved time, the backend refreshes creator info and submits each exact approved post separately.
