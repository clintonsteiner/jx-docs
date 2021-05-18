---
title: jx pipeline effective
linktitle: effective
type: docs
description: "Displays the effective tekton pipeline ***Aliases**: dump*"
aliases:
  - jx-pipeline_effective
---

### Usage

```
jx pipeline effective
```

### Synopsis

Displays the effective tekton pipeline

### Examples

  ```bash
  # View the effective pipeline
  jx pipeline effective
  
  # View the effective pipeline in VS Code
  jx pipeline effective -e code
  
  # View the effective pipeline in IDEA
  jx pipeline effective -e idea
  
  # Enable open in VS Code
  export JX_EDITOR="code"
  jx pipeline effective

  ```
### Options

```
      --add-defaults           Adds default parameters to the effective pipeline
  -b, --batch-mode             Runs in batch mode without prompting for user input
      --catalog-owner string   The github owner for the default catalog (default "jenkins-x")
      --catalog-repo string    The github repository name for the default catalog (default "jx3-pipeline-catalog")
  -d, --dir string             The directory to look for the .lighthouse and/or .git folders (default ".")
  -e, --editor string          The editor to open the effective pipeline inside. e.g. use 'idea' or 'code'
  -f, --file string            The pipeline file to render
      --git-kind string        the kind of git server to connect to
      --git-server string      the git server URL to create the scm client
      --git-token string       the git token used to operate on the git repository. If not specified it's loaded from the git credentials file
      --git-username string    the git username used to operate on the git repository. If not specified it's loaded from the git credentials file
  -h, --help                   help for effective
      --line string            The line number to open the editor at
      --log-level string       Sets the logging level. If not specified defaults to $JX_LOG_LEVEL
  -o, --out string             The output file to write the effective pipeline to. If not specified output to the terminal
  -p, --pipeline string        The pipeline kind and name. e.g. 'presubmit/pr' or 'postsubmit/release'. If not specified you will be prompted to choose one
  -r, --recursive              Recurisvely find all '.lighthouse' folders such as if linting a Pipeline Catalog
  -t, --trigger string         The path to the trigger file. If not specified you will be prompted to choose one
      --verbose                Enables verbose output. The environment variable JX_LOG_LEVEL has precedence over this flag and allows setting the logging level to any value of: panic, fatal, error, warn, info, debug, trace
```



### Source

[jenkins-x-plugins/jx-pipeline](https://github.com/jenkins-x-plugins/jx-pipeline)