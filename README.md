# IIQ Emails Bookmarklet

Make it easy to copy the email for an IncidentIQ ticket to CC or forward email threads.

## Install

Drag the link below up to your bookmarks bar:

<a style="border: solid 0.25px darkgray; border-radius: 0.5em; padding: 0.5em; background: lightgray;color: black; text-shadow: 1px 1px white; box-shadow: 1px 1px darkgray;" href="javascript:(function(){var jsCode = document.createElement('script');jsCode.setAttribute('src', 'https://groton-school.github.io/iiq-emails-bookmarklet/iiq-emails-source.js');document.body.appendChild(jsCode);}());">IIQ Emails</a>

## Use

When viewing any list of tickets in IncidentIQ, click the bookmarklet to enable the copy email links.

| Before                          | After                     |
| ------------------------------- | ------------------------- |
| ![Without](/images/without.png) | ![With](/images/with.png) |

## Known Limitations

-   Zero attention is paid to whether or not the page affected is IIQ or not
-   Repeated invocations will just keep adding more email links to the page
-   The email links block access to the actual ticket details
-   The page must be refreshed to get rid of the email links (and block on details)
-   No text-escaping is done, to prevent double-quotes in the ticket title from breaking the email address format `"Name" <email@example.com>`
