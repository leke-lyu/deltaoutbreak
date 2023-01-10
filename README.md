# Genomic Epidemiology of Delta Variant in Houston
[Nextstrain](https://nextstrain.org) uses Auspice to visualize JSON files that are created by Augur. Here we share our instance via [community](https://nextstrain.org/community/) on gitgub.

## Data Description
This instance includes 2664 genomes sampled between Jun 2021 and Aug 2021. We only selected samples with high-coverage complete genomes (above 29,000 bp) from GISAID. According to GISAID, high coverage means that only entries with less than 1% of undefined bases (NNNs) and no insertions and deletions unless verified by the submitter are tolerated.

There are 981 samples collected from Texas, 328 of which are focused on Harris county (Houston). Through collaboration with the Houston Health Department, we acquired the detailed metadata of all these Texas samples, including zip code, sex, and race. To investigate when and how did SARS-CoV-2 circulate in Houston, we also collected worldwide samples as 'background'. In total, 987 samples were collected in other US states (except Texas); 99 samples were collected in North America (except USA); 100 samples were collected in South America; 197 samples were collected in Europe; 101 samples were collected in Asia; 99 samples were collected in Africa; 100 samples were collected in Oceania.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## View the Builds
- [Texas (county view)](https://nextstrain.org/community/leke-lyu/ncov/houston)
- [USA (state view)](https://nextstrain.org/community/leke-lyu/ncov/texas)
- [USA (county view)](https://nextstrain.org/community/leke-lyu/ncov/texas?r=location)
- [Global (country view)](https://nextstrain.org/community/leke-lyu/ncov/global)
- [Global (state view)](https://nextstrain.org/community/leke-lyu/ncov/global?r=division)
- [Global (county view)](https://nextstrain.org/community/leke-lyu/ncov/global?r=location)

## Running the Build
You can find the config files that runs this build in [here.](https://github.com/leke-lyu/deltaInGreaterHoustonArea)

To run this repository, you need to have a copy or version of the [ncov]() Nextstrain repository running, as this repository builds on that base, and just does a more 'specific' run with the same data. Visit the `ncov` repository above for a guide on getting this run going.

Once you're able to run a basic build of the `ncov` repository, clone this repository into a folder which sits in the same directory as the `ncov` repository. Currently, the profile given here is specified to run on Emma's local compute cluster. You may need to change these settings to match your own cluster or local setup.

To run locally (without any advanced cluster submission) comment out line 20 in `profiles/south-central/config.yaml`, which specifies the cluster submission options (`cluster: "sbatch --time=....`) before trying to run the pipeline.
You can run the entire 'South-Central' profile (which includes Texas, Louisiana, & South-Central builds) by running
