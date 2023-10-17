# VulnPatchPairs

## Setup

The json files are stored with git-lfs. Install git-lfs using the official [tutorial](https://git-lfs.com) and run the following command from the root directory of this repository:

`git lfs pull`

## General Information

```
.
├── VulnPatchPairs-Train........... Training Dataset
├── VulnPatchPairs-Valid........... Validation Dataset
├── VulnPatchPairs-Test............ Testing Dataset
├── how_to_prepare.py.............. Script for preparing VulnPatchPairs for model training.
└── README.md
```

## Structure

Below is an annotated map of the JSON structure of VulnPatchPairs.

```
.
├── project........................ Source project (either Qemu or Ffmpeg).
├── vulnerable_func................ Code snippet with security vulnerability.
├── vulnerable_filepath............ File path of the vulnerable code snippet in source project.
├── vulnerable_commit_id........... Commit ID before the patch.
├── patched_func................... Patched version of the vulnerable code snippet.
├── patched_filepath............... File path of the patched code snippet in source project.
├── patched_commit_id.............. Commit ID of the patch.
├── patch_commit_message........... Commit message of the patch.
└── patch_diff_delta............... Git diff between the vulnerable code snippet and the patch.
```
