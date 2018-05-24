Host Redirector
===============

A simple host based redirector module for ProcessWire that's aimed to support ad-hoc redirects for marketing domains etc.

Installation
------------

Do these in your project's composer.json:

1) Add `"AvoineOy/hostredirector": "dev-master"` to your requires

2) Add the repository as follows:

```
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/AvoineOy/hostredirector"
    }
  ],
```

3) Add these scripts:
```
    "scripts": {
      "post-install-cmd": [
        "rm -fr public/site/modules/HostRedirector",
        "mkdir public/site/modules/HostRedirector",
        "cp vendor/AvoineOy/HostRedirector/HostRedirector.module public/site/modules/HostRedirector"
      ],
      "post-update-cmd": [
        "rm -fr public/site/modules/HostRedirector",
        "mkdir public/site/modules/HostRedirector",
        "cp vendor/AvoineOy/HostRedirector/HostRedirector.module public/site/modules/HostRedirector"
      ]
    },
```

4) Add /public/site/modules/HostRedirector to .gitignore
