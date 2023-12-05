# Twinpack Package Registry

This repository contains a [list](https://github.com/Zeugwerk/Twinpack-Registry/blob/main/repositories.txt) of GitHub repositories that are automatically published to the [Twinpack Package Manager](https://github.com/Zeugwerk/Twinpack).

## Adding a package

If you would like to make a TwinCAT library available for installation via [Twinpack](https://github.com/Zeugwerk/Twinpack), please submit a 
[pull request](https://docs.github.com/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests)
that adds the URL of your repository to [repositories.txt](repositories.txt). You are welcome to add multiple libraries at once.

See the instructions below for detailed instructions on how to do this via the GitHub web interface.

### Instructions

1. **Create a new fork** by clicking [https://github.com/Zeugwerk/Twinpack-Registry/fork](https://github.com/Zeugwerk/Twinpack-Registry/fork) <br />
   The new page page will open.
1. Click the <kbd>Create fork</kbd> button in the "**Create a new fork**" page.
1. Wait for the "Forking" process to finish.<br />
   The home page of your [fork](https://docs.github.com/get-started/quickstart/fork-a-repo) of the **Twinpack-Registry** repository will open.
1. Click on the file `repositories.txt` under the list of files you see in that page.
1. Click the pencil icon ("Edit this file") at the right side of the toolbar<br />
   The `repositories.txt` file will open in the online text editor.
1. Add your repository's URL to the list (it doesn't matter where in the list). This should be the URL of the repository home page. For example:
   `https://github.com/stefanbesler/struckig`
1. Click the <kbd>Commit changes...</kbd> button located near the top right corner of the page.<br />
   The "**Commit changes**" dialog will open.
1. Click the <kbd>Commit changes</kbd> button in the "**Commit changes**" dialog.<br />
   The "**Twinpack-Registry/repositories.txt**" page will open.
1. Click the "**Twinpack-Registry**" link at the top of the "**library-registry/repositories.txt**" page.<br />
   The home page of your fork of the **Twinpack-Registry** repository will open.
1. Click the "**Contribute**" link near the right side of that banner.<br />
   A menu will open.
1. Click the <kbd>Open pull request</kbd> button in the menu.<br />
   The "**Open a pull request**" page will open.
1. In the **"Open a pull request"** window that opens, click the <kbd>Create pull request</kbd> button.

At the moment PR are processed by somebody of our team. We will check if
your repositories releases qualify to be put on the list, we will check that
- Your repository has at least 1 release,
- your release(s) are published having a .library file in their assets,
- the .library files contains the meta information Twinpack requires, the bare minimum is "Library Name", "Company Name" (Distributor name) and "Version".
- If we see an icon in your repository that makes sense to use, we'll ask you for permission to link it with the package

If any problems are found, we'll respond in the pull request. The problem may be either
with your pull request or your repository.

#### If the problem is with the pull request:

Edit the file in the
[branch](https://docs.github.com/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches)
you submitted the pull request from in your fork of the `Zeugwerk/Twinpack-Registry` repository, then commit.


#### If the problem is with the repository:

1. Make the necessary fix in the repository.
1. Increment the `version` of your [TwinCAT library](https://infosys.beckhoff.com/english.php?content=../content/1033/tc3_plc_intro/3260045067.html)
1. Create a [release](https://docs.github.com/repositories/releasing-projects-on-github/managing-releases-in-a-repository)
   or [tag](https://git-scm.com/docs/git-tag) and include your library in the assets of the release. Alternatively, you can redo the existing release/tag if you prefer.
1. Comment on your pull request here in the `Twinpack/Twinpack-Registry` repository

## Changing the URL of a library already in Library Manager

Submit a pull request that changes the URL as desired in [repositories.txt](repositories.txt). This can be done by
following [the instructions above](#instructions).

## Removing a library from Library Manager

Submit a pull request that removes the URL from [repositories.txt](repositories.txt). This can be done by following
[the instructions above](#instructions).

## Report a problem with Library Manager

Please submit an issue report [here](https://github.com/Zeugwerk/Twinpack-Registry/issues/new)
