# ajax-github-api-to-add-multiple-issues
Using GitHub API to POST multiple issues via loop and ajax
[Create Issue via API](https://developer.github.com/v3/issues/#create-an-issue)

## I had some 180 tasks back-logged on Asana.
I wanted them in github 'under' a repo.
Example only shows two; and not from an external file

## You will have to turn on CORS; I did it with a chrome-extension.
- I'm sure there is another way, I prefer to do it this way.
 -- Doing so, allows me to trouble shoot without wasting API calls

Using Brackets, I started new from template; to include jQuery.
Used postman to configure my auth-key and test POST(ing) one single issue.
***
Exported my tasks from Asana into csv.
Used =concatenate to get the information I wanted from that file.
Saved that information to a file; which I called later to init the loop.
***
THINGS TO NOTE BECAUSE YOU WILL NEED TO CHANGE THEM:
```
"url": "https://api.github.com/repos/:org/:repo/issues",
```
[Help On This Topic](https://developer.github.com/v3/issues/#create-an-issue)
```
"authorization": "Bearer YOURCUSTOMTOKEN HERE",
```
[Help On This Topic](https://github.com/settings/developers)
