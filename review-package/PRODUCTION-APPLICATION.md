# Wright Drafts - production review draft

**Status:** Draft for owner review. Do not submit until the finished hosted app and demo match every statement below.

## Public app description (120-character field)
Prepare, review, schedule, and publish original educational photo carousels to your own TikTok account.

## Proposed category
Education

## Platform
Web

## Product and scope explanation (1000-character field)
Wright Drafts is a web app that helps creators prepare and publish original educational photo carousels to their own TikTok accounts. Login Kit and `user.info.basic` connect the creator and show the authorized TikTok identity. Content Posting API uses `video.publish` to retrieve current creator posting options, display each final carousel preview, let the creator edit the caption, manually choose privacy and interaction settings, declare commercial content, review TikTok's required music and policy notice, and expressly approve each exact post before it is sent. Creators may review several finished posts in one queue, but each post has its own preview, metadata, schedule, and approval checkbox. The app checks that approved content has not changed before publishing, submits each post separately at its approved time, and displays processing and publish status. `video.upload` is retained as a creator-selected fallback to TikTok's in-app editing flow. Creators can disconnect and revoke access.

## Products and scopes requested
- Login Kit
- Content Posting API with Direct Post and Upload to TikTok
- `user.info.basic`
- `video.publish`
- `video.upload`

## Claims that must be true before submission
- The public website is a finished creator tool, not a landing page or a private uploader.
- Any creator in the supported audience can connect their own TikTok account.
- The app shows current creator info and only privacy options returned by TikTok.
- No privacy or interaction choice is preselected.
- Every post has a preview, editable caption, disclosure controls, TikTok declaration, and exact consent before transfer.
- Batch review requires a separate approval checkbox for every immutable post version.
- The service displays status and supports revocation/deletion.
