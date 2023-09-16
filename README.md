<p align="center">
  <img alt="camo purge logo" src="https://imgur.com/Xt2k39E.png" width="210">
</p>
<p align="center">
  Github Action to purge githubusercontent camo cache.
</p>
<p align="center">
  Purge shield badges cache from README.md for githubusercontent camo.
</p>

**Quick Setup:** Simply add a GitHub Action to your workflow.

**Easy:** No arguments required.

**Auto Detect** Just add the action and it will automatically detect the branch and org names.


# Using Action

```yaml
    - uses: kevincobain2000/action-camo-purge@v1
```

# About

Github shields.io badges are cached by camo.
This action purges the cache for the badges or any other images in `README.md`.

Badges from codecov, [coveritup.app](https://coveritup.app), or any other external images in README are cached by Github using camo. This means, that the images are not loaded from the original source, but from a proxy server.

Purging camo cache is necessary on regular basis, in order to show the latest values on the shield badges.

With this action, you can purge the camo cache for the images in `README.md`, whenever there is a change in the repository on `push` or `pull_request` events. It can also be used on a `cron`.

The action picks up the branch names and org names automatically, so no need to pass any arguments.

[Read more about camo](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-anonymized-urls)

## CHANGE LOG

v1.0.0 - Initial release