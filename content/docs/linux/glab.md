---
title: "glab"
draft: false
---

# glab

glab is an open-source GitLab CLI tool. It brings GitLab to your terminal: right where you already work with Git and your code, without switching between windows and browser tabs.

Source: https://docs.gitlab.com/editor_extensions/gitlab_cli/

## Sign in

```bash
glab auth login --stdin < token.txt
```

## View a list of issues

```bash
glab issue list
```

## Create merge request for issue 123

```bash
glab mr create 123
```

## Check out the branch for merge request 243

```bash
glab mr checkout 243
```

## Watch the pipeline in progress

```bash
glab pipeline ci view
```

## View, approve, and merge the merge request

```bash
glab mr view
```

```bash
glab mr approve
```

```bash
glab mr merge
```
