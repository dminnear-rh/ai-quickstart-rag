# ai-quickstart-rag

This pattern is currently intended to be run on AWS where it will automatically create the GPU machineset (g6.2xlarge) that the pattern needs.

## Installing this pattern

* log into a fresh openshift cluster on AWS (no need to add GPU nodes manually, the pattern does it)
* copy [`values-secret.yaml.template`](./values-secret.yaml.template) to `~/values-secret-ai-quickstart-rag.yaml`
  * update the hf token secret with an api key that has access to the models used by [the quickstart](https://github.com/rh-ai-quickstart/rag)
* run `./pattern.sh make install`
