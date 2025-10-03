# [1.38.0] (Date: 2025-08-13)

### Bug Fixes

- **i18n:** correct punctuation in Turkish disclaimer
- **i18n:** Fix Turkish text and translation errors
- **post:** Post detail 404 error resolved
- **ui:** adjust same padding values for post layout consistency

### Features

- **admin:** Implement automatic account follow feature for new users
- **admin:** Force delete user method
- **search** Increase search stability
- **worker** Sidekiq workers were seperated



# [1.35.0] (Date: 2025-07-31)

### Bug Fixes

- **trends:** increase score halflife to 1 hour and adjust trends refresh interval to 45 minutes for better trend management
- **language:** update disclaimer text to include platform name
- **logo:** Resolved logo issue in automatic theme's default dark mode
- **search:** add fuzziness and autocomplete bugfixes 
- **post:** disable navigation to likers page, show count only
- **post:** show likers page only for owner of the post
- **preview:** add missing title and description in link previews on web
- **live-stream:** reduce fetch frequency from every second to once per minute
- **ui:** adjust padding values for post layout consistency
- **media-preview:** prevent rendering SVG files as video previews
- **quote:** show link preview correctly when quoting posts with both video and link
- **i18n:** correct translation error in search and add missing Turkish text
- **repost:** update label to 'Yeniden paylaşmayı geri al' when already shared
- **ui:** allow spaces when commenting on quotes
- **ui:** prevent quote click from opening in new tab
- **embed:** remove title and redirect buttons from live video embeds
- **preferences:** enable functionality of sign-out button in preferences
- **post:** show media content along with link preview in post detail
- **auth:** redirect unauthenticated follow attempts to sign-in page
- **error-page:** remove Mastodon link from error page
- **poll:** correct remaining time display issue
- **post:** redirect to homepage after delete and remove error page logo
- **media:** increase media attachment resolution
- **logs** Detailed logs added for trends
- **logs** sidekiq logging bug fixed
- **webpack:** update webpack plugin configs to prevent env leaks
- **sso:** remove unused links from SSO page
- **badges:** hide badge component when no badge exists
- **post-actions:** resolve hover shift issue in action buttons
- **profile:** fix badge overflow issue in about section
- **deps:** update dependencies


### Features

- **badges:** add badges feature to user profiles
- **badges:** implement badges management API with assign and remove actions
- **badges:** allow multiple badges to wrap on mobile view
- **notifications:** display user badges next to usernames
- **ui:** increase badge icon size to 25px
- **admin:** add badge assignment page for moderators
- **favicon** add favicon to the application
- **i18n:** add Turkish translations for warning messages
- **language:** remove post language support other than en-tr
- **logo:** added separate logos for light and dark mode
- **view-tracking:** trigger API only if post is 30% visible for 2 seconds
- **preview, settings:** show YouTube links as video only for livestreams
- **post-detail:** show quote count and quoted posts in detail view
- **media:** update quote and favorite UI in media posts
- **ranking** optimize status ranking and filtering logic
- **quote:** add link preview display for quote
- **post:** increase count when repost or quote is made
- **quote:** add quote count
- **ui** rocket icon added
- **admin:** add search functionality to admin panel
- **schedule:** show warning for durations shorter than 5 minutes
- **post:** enable sharing posts with both text and image
- **auth:** add auth check for limited federation mode
- **auth:** add public account
- **auth:** add public timeline
- **auth:** add readonly account
- **auth:** remove public ssr pages authentication
- **auth:** redirect unauthenticated users to login on post interaction
- **i18n:** localize time format to Turkish
- **i18n:** make time localization dynamic for all locales
- **ui:** add privacy policy page
- **api:** make feedback API dynamic
- **env:** add favicon URL support via environment variable
- **post:** update UI components for post layout
- **ui:** redesign and improve responsiveness of 404 error page
- **auth:** update mobile Sign Up button URL to use environment variable
- **ui:** add new post creation button to interface
- **ui:** remove Mastodon mascot from homepage in advanced view
- **components/onboarding_modal:** Swipe between pages
- **compose:** More space on mobile devices
- **css:** Remove border radius from WebKit's scrollbars
- **web_push_notifications:** Group notifications 


### Performance Improvements

- **feed:** reduce post fetch limit to 10 on profile and home page
- **streams:** set fetch limit to 10 for local timeline, favorites, and bookmarks
- **comments:** add pagination to post comments
- **follow** add pagination to follower page
- **favorite** add pagination to favorite page
- **settings:** set 'slow mode' checkbox as checked by default


### Base Version
from [mastodon](https://github.com/mastodon/mastodon) #commit [faed9bf9f14f077443374f5eb3075b9878e24214](https://github.com/mastodon/mastodon/commit/faed9bf9f14f077443374f5eb3075b9878e24214)