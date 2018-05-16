## Troubleshooting / FAQ

### Using GoSublime, the autocompletion is showing cached methods

The issue is GoSublime uses your GOPATH/pkg/ dir for autocompletion.  This means, if you haven't "go install" in awhile, you will have very old values.  The easiest way to update is to run something like `go install github.com/SYNQfm/helpers/common` to update the library you want and have it available in the autocomplete!