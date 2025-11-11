# Git File Storage Datastore

This idea is to quickly turn a `git` repository into a version-controlled file
storage facility without spinning a new type of file servers (e.g. `samba`). It
is specficially designed for non-tech users to use the same `git version
control system` (GVCS) platform alongside the tech users who actually uses the
`git` itself for sane data warehouse maintenances especially in self-hosting
environments.

Useful data to store would be:

* photo albums.
* binary files and etc.
* CAD design files.
* Non-text files.
* Anything when you have no idea how to use `git`.

> [!IMPORTANT]
>
> This is a file storage datastore control repository. If you are NOT asked to
> create or maintain one, **you are likely looking for the contents files in the
> `Releases` section**.
>
> On GitHub:
>
> ![gihub-release-section](/.internals/screenshots/github-release-section.jpg)
>
> On Forgejo:
>
> ![gihub-release-section](/.internals/screenshots/forgejo-release-section.jpg)
>
> On Gitea:
>
> ![gitea-release-section](/.internals/screenshots/gitea-release-section.jpg)
>
>
> Please head over there and ignore anything below. Thank you.




## For Creators & Maintainers

[![chewkeanho-template](/.internals/icons/animated-banner_1200x100.svg)](#)

This section is for non-technical users who wanted to spawn a new repository
without using `git` and command line.

They are arranged in a "learn all" curriculum chronological depending chapters.
However, each task is independent from one another.

* [Creating New Repostory](#creating-new-repository)
* [Making A Release Version](#making-a-release-version)
* [Updating A Release Contents](#updating-a-release-contents)



### Creating New Repository

To create a new repository, simply select the **`Use This Template`** on your
GCVS web terminal.

On GitHub:

![github-press-use-this-template-button](/.internals/screenshots/github-press-use-template-button.jpg)

On Forgejo:

![forgejo-press-use-this-template-button](/.internals/screenshots/forgejo-press-use-template-button.jpg)

On Gitea:

![gitea-press-use-this-template-button](/.internals/screenshots/gitea-press-use-template-button.jpg)



### Making A Release Version

[![chewkeanho-template](/.internals/icons/animated-banner_1200x100.svg)](#)

To create a new release version, first edit the `VERSION` file on the web UI:

On GitHub:

![github-edit-VERSION](/.internals/screenshots/github-edit-VERSION.jpg)

On Forgejo:

![forgejo-edit-VERSION](/.internals/screenshots/forgejo-edit-VERSION.jpg)

On Gitea:

![gitea-edit-VERSION](/.internals/screenshots/gitea-edit-VERSION.jpg)

Then edit the file value with a different version ID. For examples:

```
v[MAJOR].[MINOR].[PATCH]

Examples:
v0.0.1
v1.2.1
...
```

> **GUIDELINES**
>
> * `[MAJOR]` - usually means breaking changes (non-backward compatible)
> * `[MINOR]` - usually means non-breaking changes (backward compatible)
> * `[PATCH]` - usually means minor non-essential stuffs (e.g. docs' typo)

Once done, commit your changes as below, this will create a new timestamp
entry (commit ID).

On GitHub (Note that you need to press the *Create new tag* button after viewing
the *Tag* panel insides and then fill in your label):

![github-commit-VERSION](/.internals/screenshots/github-commit-VERSION.jpg)

On Forgejo:

![forgejo-commit-VERSION](/.internals/screenshots/forgejo-commit-VERSION.jpg)

On Gitea:

![gitea-commit-VERSION](/.internals/screenshots/gitea-commit-VERSION.jpg)

Lastly, head over to `Release Sections` and press the **`Create a New Release`**
button. **For `tag` and `Title`, use the same value (e.g. `v1.0.0`)**. `Tag` is
like *Bookmark when reading a thick book where you note certain pages*. Title is
presenting the title of the web page.

Once done, drag and drop your files into the *"Upload Dropzone"*. That's how
you upload files. Note that the limits (e.g. max size) are ultimately depend on
the platform provider.

On GitHub:

![github-new-release](/.internals/screenshots/github-new-release.jpg)

On Forgejo:

![forgejo-new-release](/.internals/screenshots/forgejo-new-release.jpg)

On Gitea:

![gitea-new-release](/.internals/screenshots/gitea-new-release.jpg)



### Updating A Release Contents

To update a versioned release content, simply head to your release version and
select `Edit` button. Then upload/remove your files accordingly before pressing
the `Publish Release` or `Update Release` button again.

On GitHub:

![github-new-release](/.internals/screenshots/github-edit-release.jpg)

On Forgejo:

![forgejo-new-release](/.internals/screenshots/forgejo-edit-release.jpg)

On Gitea:

![gitea-new-release](/.internals/screenshots/gitea-edit-release.jpg)




## License

[![chewkeanho-template](/.internals/icons/animated-banner_1200x100.svg)](#)

This template repository is licensed under [BSD 1-Clause License](/LICENSE.txt).
The following are the product details:

```
Title           : (Holloway) Chew, Kean Ho's File Storage Datastores Template
Contact         : hello@chewkeanho.com
UUID            : B5F5091C-81E1-4D01-B886-BC3F82A83537
SKU             : chewkeanho-datastores-file-storage
Trademark Holder: Chew Kean Ho (natural person)
License         : BSD 1-Clause License
Made On         : 2025-11-30
Procure         : https://github.com/ChewKeanHo/datastores-file-storage
```
