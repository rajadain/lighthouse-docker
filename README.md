# Lightroom Docker

Simple setup to run Lightroom with Headless Chrome for any URL.

## Usage

```
./scripts/run https://azavea.com
```

This will run and save an HTML report in the `reports/` folder. Replace
`https://azavea.com` with whatever URL you need to test.

## Credits

This uses @justinribeiro's [Lighthouse Dockerfile][dockerfile] as the base
image, and @jessfraz's [seccomp][seccomp] for setting Docker security options
to run Lighthouse without sys-admin privileges.

[dockerfile]: https://github.com/justinribeiro/dockerfiles/blob/master/lighthouse/Dockerfile#L18
[seccomp]: https://github.com/jessfraz/dotfiles/blob/master/etc/docker/seccomp/chrome.json
