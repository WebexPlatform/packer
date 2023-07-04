# packer
We met a packer issue on OpenStack platform, which will cause the temporary VM cannot be deleted after packer build.

[A PR](https://github.com/hashicorp/packer-plugin-openstack/pull/94) has been committed to upstream to fix the issue.

But after more than one month, nobody reviews it yet.

So I create this repository and a Jenkins pipeline to build packer binary with this patch.

If a new release of official packer there, we can use the pipeline to build new patched packer binary.

This repository can be archived while the community accepts the PR.

From [packer v1.9.0][https://github.com/hashicorp/packer/releases/tag/v1.9.0], [packer-plugin-openstack](https://github.com/hashicorp/packer-plugin-openstack) has been removed from packer, so I will archive this repo, please use packer-plugin-openstack >= v1.1.0 to fix the issue.
