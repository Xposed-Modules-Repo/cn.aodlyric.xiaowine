# Xposed Modules Repo Example

You may only upload your own modules. If you have explicit permission from a developer to upload their module, it is fine as well, but both of you need to keep in mind that the uploader's name will be mentioned as author.
Obviously, modules must be compliant with the law and must not act in malicious ways. The operator of this site will not take any responsibility (or give support) for uploaded modules.

Only default branches will be processed.

## Informations

### Module name *

The Description of repository details.

### Package *

The repository name.

> The package name of the app - has to be the same for all versions!

### Summary

Contents in [SUMMARY](SUMMARY) file.

> A brief description of the module, will be displayed outside the list, no formatting is supported.
> Leave blank to use trimmed value of full text as the summary.

### Description *

Contents in [README.md](README.md) file.

### Support/Discussion URL *

The Website of repository details.

> Link to a site where users can get support for and discuss about your module. (e.g. your XDA thread)

### Source code URL

Contents in [SOURCE_URL](SOURCE_URL) file, any line breaks (\r & \n) will disappear.

> Link to the source code of your module if you published it.

### Additional authors

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

### Visibility

If you want to hide the module from the repository temporarily, you can change repository to private in Repository Settings.

If you just want the module not to be displayed in the website page or manager, create a [HIDE](HIDE) file.

## Versions

We use GitHub releases as a version update.

### Version name *

The Release Title.

> This is the human-readable version number.

### Version code *

The Release Tag.

> The technical version, used when checking for updates. Newer versions always need to have a higher number than previous versions.

### Release type *

`This is a pre-release` check box.

experimental has been merged with beta

|  Type  |  Type  |
|  ----  |  ----  |
| Stable (low risk of bugs)  | Release |
| Beta (some bugs to be expected)  | Pre-release |
| Experimental (high risk of bugs)  | Pre-release |

> Classification how risky it is for users to install this version. By default, only stable versions will be shown.

### Changes

The Release Description.

> A list of changes (new features, bugfixes) in this particular version.
