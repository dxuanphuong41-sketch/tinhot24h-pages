# TikTok App Review Pages

This folder contains the public website used for the TikTok Developer app review of `tinhot24h`.

Production URL:

`https://dxuanphuong41-sketch.github.io/tinhot24h-pages/`

## URLs to enter in TikTok Developer

- Web/Desktop URL:
  `https://dxuanphuong41-sketch.github.io/tinhot24h-pages/`
- Terms of Service URL:
  `https://dxuanphuong41-sketch.github.io/tinhot24h-pages/terms.html`
- Privacy Policy URL:
  `https://dxuanphuong41-sketch.github.io/tinhot24h-pages/privacy.html`
- Login Kit Redirect URI:
  `https://dxuanphuong41-sketch.github.io/tinhot24h-pages/callback/`

The redirect URI must match exactly, including `https`, trailing slash, and path.

## Review explanation text

Paste this into the TikTok review explanation field:

```text
tinhot24h is a creator-operated desktop and web-assisted publishing workspace for the Vietnamese short-video channel "Lướt Mạng Có Chuyện".

Login Kit is used so the channel owner can authorize their own TikTok account. The scope user.info.basic is used only to confirm the authorized creator account after OAuth login.

The Content Posting API is used with the video.upload scope to upload creator-approved local video files to TikTok as drafts. The creator first renders a video locally, reviews the narration, subtitles, source context, caption and hashtags, then uploads the approved file. The app does not automatically publish public TikTok posts without creator review and does not manage third-party accounts.

The public website at https://dxuanphuong41-sketch.github.io/tinhot24h-pages/ shows the actual TikTok integration flow for review: Login with TikTok, OAuth callback, creator review, and draft upload workflow. The desktop bot performs the secure token exchange and upload operation locally.
```

## Demo video script

Record a fresh demo video. Do not use Telegram Web as the main screen.

1. Open `https://dxuanphuong41-sketch.github.io/tinhot24h-pages/`.
2. Show the visible Privacy Policy and Terms of Service links in the top navigation.
3. Scroll to the TikTok Draft Upload Demo panel.
4. Paste the public TikTok Client Key into the Client Key field.
5. Confirm the Redirect URI field is:
   `https://dxuanphuong41-sketch.github.io/tinhot24h-pages/callback/`
6. Click `Login with TikTok`.
7. Show the TikTok authorization screen and approve the requested scopes.
8. Show the callback page receiving the authorization code.
9. Return to the website and click `Simulate approved draft upload`.
10. Then show the local desktop bot or command window performing the real creator-approved upload/draft flow.

Keep the video under 50 MB. A 60-90 second recording is enough if the text is readable.

## Important configuration notes

- Do not upload or display the TikTok Client Secret on this website.
- The Client Key is public OAuth configuration and may be shown in the demo.
- The selected TikTok products/scopes should be only:
  - Login Kit
  - Content Posting API
  - `user.info.basic`
  - `video.upload`
- If the app has not been approved before, use the TikTok sandbox environment in the demo where TikTok asks for it.
