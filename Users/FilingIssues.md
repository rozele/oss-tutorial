# Filing Issues for Bugs and Feature Requests

Issue management is a primary cause of OSS fatigue for maintainers.

- [ ] Check for related issues
- [ ] Validate existing issues
- [ ] Ensure feature requests belong in *Issues*
- [ ] Complete the issue template *entirely*
- [ ] Capture environment details
- [ ] Include a minimal repro

Remember, ***be respectful of maintainers time*** by being as detailed and thorough as possible when filing issues. If it's going to take a maintainer a few hours to do a root cause analysis, create a patch, submit a pull request, and follow through on code reviews, you can spare 30 minutes when filing.

## Checking for related issues

Search the repo for related issues.
![searchbar](../img/GitHubSearch.png)

## Validate existing issues

If you find someone has already reported an issue, validate any repros provided in the existing issue, or include your own if none were provided. Remember, ***code is not the only currency***.

## Example issue template

Issue template from [Azure/azure-service-bus](https://github.com/Azure/azure-service-bus)

```markdown
# Description
<!-- 
If you have an issue or a feature request for a specific client library, see the following:
* [.NET Standard](https://github.com/azure/azure-service-bus-dotnet)
* [Java](https://github.com/azure/azure-service-bus-java)

If you think your request is more specific to the Service Bus service, please fill out the following template.
-->

## Actual Behavior
1. 
2. 

## Expected Behavior
1. 
2. 
```

## Common environment details

- [ ] Project Release Version
- [ ] Development Operating System
- [ ] Target Deployment Platform
- [ ] Related CLI Tools Versions (NPM, Docker, etc.)
- [ ] IDE Version

## Include a minimal repro

If a contributor can't reproduce your bug, they are less likely to fix it. If possible, include a screen grab of the issue, or even a video.

- [ ] Code
- [ ] Screenshots
- [ ] Video
