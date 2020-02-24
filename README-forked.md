# Overview
Local forked repo to be able to define Jenkins agents in a Shared Library.

# Usage
The main goal is to be able to mix and match multiple agents for out pipeline purpose by adding custom agent manifests (yamlFiles in resources/podTemplates). The core remains unchanged and remains maintained by the user.

The following should be considered:
- adapt base to your preference. This is the base agent to build images. Keep name jnlp for consistency with the source.
- 