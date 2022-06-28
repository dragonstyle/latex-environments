# environments

## Overview

Divs with a class name listed in the in the `environments` key will be emitted in LaTeX as an environment with the provided name (or the class name itself if no name is provided). All of the following are valid:

```yaml
environments: program

environments:
  - program

environments: [program]

environments:
  program: program-env
```

## Example

```markdown
---
title: Test document
environments: [program]
----

:::{.program}
The contents of this div will be output in a `program`
latex environment, but will appear in HTML (and any other output format as a simple div with the class `program`)
:::
```
