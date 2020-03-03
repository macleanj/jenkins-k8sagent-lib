# Overview
Local forked repo to be able to define Jenkins agents in a Shared Library.

# Usage
The main goal is to be able to mix and match multiple agents for out pipeline purpose by adding custom agent manifests (yamlFiles in resources/podTemplates). The core remains unchanged and remains maintained by the user.

The following should be considered:
- adapt resources/podTemplates/base.yaml to your preference (base.yaml should be always loaded in the Jenkinsfile).
- base (base.yaml) should be explicitly included (bug in source code)
- Keep container-name "jnlp" for consistency with the source.
- Do not use "-" or "+" in the k8sagent call as this is the user delimiter.

Example:
```

```

# Changes
- This file
- vars/k8sagent.groovy (fixed comps = comps.plus(0, 'base') issue)
- resources/podTemplate all (self managed)
- 