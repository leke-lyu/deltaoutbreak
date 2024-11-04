# The Genomic Surveillance of Delta outbreak in Texas

<img align="right" width="100" alt="Texas" src="https://user-images.githubusercontent.com/46392207/212571616-83689300-e02e-42d7-a288-e1706c82df3f.png">

[Nextstrain](https://nextstrain.org) uses Auspice to visualize JSON files that are created by Augur. Here we share our instance via [community](https://nextstrain.org/community/) on gitgub.

## Data Description

We conducted a comprehensive phylogeographic analysis of 12,048 SARS-CoV-2 Delta genomes sampled from March 27, 2021, to October 24, 2021, to investigate the timing of virus introduction into Texas and the dynamics of the resulting local transmission lineages. These genomes were selected to ensure a roughly 1:1 ratio between Texas sequences and globally contextual sequences. 

## View the Builds

- [Texas build](https://nextstrain.org/community/leke-lyu/deltaoutbreak/texas)

## Running the Build
You can find the config files that runs this build in [here.](https://github.com/leke-lyu/surveillanceInTexas)

To replicate this run, you need to first (1) install Nextstrain components and (2) download the ncov workflow. Please visit [this page](https://docs.nextstrain.org/projects/ncov/en/latest/tutorial/setup.html) if you need more instruction on installation.

Once you can run a basic build of the `ncov` repository, clone [this repository](https://github.com/leke-lyu/deltaInGreaterHoustonArea) into the `ncov` folder. To run locally (without any advanced cluster submission), you could type:

```shell
nextstrain build . --configfile surveillanceInTexas/builds.yaml
```

