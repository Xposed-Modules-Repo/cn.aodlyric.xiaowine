# Xposed Modules Repo Example

Only default branches will be processed.

## Module name *

The Description of repository details.

## Package *

The repository name.

> The package name of the app - has to be the same for all versions!

## Summary

Contents in [SUMMARY](SUMMARY) file.

> A brief description of the module, will be displayed outside the list, no formatting is supported.
> Leave blank to use trimmed value of full text as the summary.

## Description *

Contents in [README.md](README.md) file.

## Support/Discussion URL *

The Website of repository details.

> Link to a site where users can get support for and discuss about your module. (e.g. your XDA thread)

## Source code URL

Contents in [SOURCE_URL](SOURCE_URL) file, any line breaks (\r & \n) will disappear.

> Link to the source code of your module if you published it.

## Additional authors

Json in [ADDITIONAL_AUTHORS](ADDITIONAL_AUTHORS) file.

|  Field  |  Type  |  Description  |  Optional  |
|  ----  |  ----  |  ----  |  ----  |
| `type`  | String |  "add" or "remove"  |  No  |
| `name`  | String |  The name of author  |  No  |
| `link`  | String |  The link of author  |  Yes  |

Example: 
```json
[{
	"type": "add",
	"name": "exampleAuthorA",
	"link": "http://example.author/A/user/link"
}, {
	"type": "add",
	"name": "exampleAuthorB",
	"link": "http://example.author/B/user/link"
}, {
	"type": "add",
	"name": "exampleAuthorC"
}, {
	"type": "remove",
	"name": "someoneInContributorsWillRemove"
}]
```

> In case you have developed the module together with somebody else, but they don't have a GitHub account. You can write their names and links into the file.
> All commited contributors in this repository will be added by default.
