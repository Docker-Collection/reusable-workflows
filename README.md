# Reusable Workflows

This workflow is maintained for all Docker-Collection repo use.

It will be less, and focus on depend version or main version update, not action update.

- [`docker-build.yml`](.github/workflows/docker-build.yml)

Simple docker build action.

| ID | Type | Description | Required |
| --- | --- | --- | --- |
| repo_name | String | Summary generate name, default will use repo name | false |
| docker_name | String | ghcr.io push name | true |
| publish | Boolean | Push Image to ghcr.io, default is always push | false |
| dockerfile | String | Docker file name, default is ``Dockerfile`` | false |
| platforms | String | Image support platforms, Default is ``linux/amd64,linux/arm64`` | false |
| docker_label_author | String | Docker Label: Author | true |
| docker_label_title | String | Docker Label: Title | false |
| docker_label_description | String | Docker Label: Description | false |
| version_detecter | Boolean | Enable version detecter, default ``false`` | false |
| version_detecter_var | String | Placeholder of detect | false |
| version_detecter_cut | String | Cut number, Default is ``2`` | false |
| build_args | String | Build Args | false |
| special_build | Boolean | Special step for generate buildtime from docker meta step | false |
| special_build_args | String | Special step of the build time var name | false |
