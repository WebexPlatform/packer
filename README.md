# packer
We met a packer issue on OCP platform, which will cause the temporary VM cannot be deleted after packer build.

[A PR](https://github.com/hashicorp/packer-plugin-openstack/pull/94) has been committed to upstream to fix the issue.

But after more than one month, nobody reviews it.

So I create this repository and a Jenkins pipeline to build packer binary with this patch.

If a new release of official packer there, we can use the pipeline to build new patched packer binary.

This repository can be archived while the community accepts the PR.
