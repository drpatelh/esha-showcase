# Add a Pipeline to the Launchpad

The Launchpad allows you to launch and manage Nextflow pipelines and associated compute that your pipelines will be executed on. Using the Launchpad, you can create a curated set of pipelines (including variations of the same pipeline) that are ready to be executed on the associated compute environments, while allowing the user to customize the pipeline-level parameters if needed.

## 1. Add a Pipeline

To add a pipeline, click on the **'Add Pipeline'** button. As an example, we will add the [nf-core/rnaseq](https://github.com/nf-core/rnaseq) pipeline to the Launchpad.

![Adding nf-core/rnaseq pipeline](assets/sp-cloud-add-rnaseq.gif)

Specify a name, description, and click on pre-existing AWS compute environment to execute on.

## 2. Specify a repository URL and revision

In the repository URL, specify the nf-core/rnaseq repository:

```bash
https://github.com/nf-core/rnaseq
```

Additionally, specify a version of the pipeline as the 'Revision number'. You can use `3.14.0`.

## 3. Parameters and Nextflow Configuration

Pipeline parameters and Nextflow configuration settings can also be specified as you add the pipeline to the Launchpad.

For example, a pipeline can be pre-populated to run with specific parameters on the Launchpad.
![Adding pipeline parameters](assets/sp-cloud-pipeline-params.gif)

## 4. Pre-run script and additional options

You can run custom code either before or after the execution of the Nextflow script. These text fields allow you to enter shell commands.

Pre-run scripts allow you to run optional Bash script(s) that executes before pipeline launch in the same environment where Nextflow runs. Pre-run scripts are useful for executor setup (e.g., use a specific version of Nextflow) and troubleshooting.
![Specify NF version in pre-run script](assets/sp-cloud-pre-run-options.gif)
