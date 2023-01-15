<a name="readme-top"></a>
# Genomic Epidemiology of Delta Variant in Houston 

<img align="right" width="100" alt="Texas" src="https://user-images.githubusercontent.com/46392207/211480214-5a6c92b6-ba0a-4268-a118-f55529bf6ba9.png">

[Nextstrain](https://nextstrain.org) uses Auspice to visualize JSON files that are created by Augur. Here we share our instance via [community](https://nextstrain.org/community/) on gitgub.

## Data Description
This instance includes 2664 genomes sampled between March 2021 and November 2021. We only selected samples with high-coverage complete genomes (above 29,000 bp) from GISAID. According to GISAID, high coverage means that only entries with less than 1% of undefined bases (NNNs) and no insertions and deletions unless verified by the submitter are tolerated.

There are 981 samples collected from Texas, 328 of which are focused on Harris county (Houston). Through collaboration with the Houston Health Department, we acquired the detailed metadata of all these Texas samples, including zip code, sex, and race. To investigate when and how did SARS-CoV-2 circulate in Houston, we also collected worldwide samples as 'background'. In total, 987 samples were collected in other US states (except Texas); 99 samples were collected in North America (except the USA); 100 samples were collected in South America; 197 samples were collected in Europe; 101 samples were collected in Asia; 99 samples were collected in Africa; 100 samples were collected in Oceania.

The following plot showed the collection date of all samples.
<p align="center"><img src="https://github.com/leke-lyu/ncov/files/10379414/Date.pdf"></p>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## View the Builds
- [Texas (county view)](https://nextstrain.org/community/leke-lyu/ncov/houston)
- [USA (state view)](https://nextstrain.org/community/leke-lyu/ncov/texas)
- [USA (county view)](https://nextstrain.org/community/leke-lyu/ncov/texas?c=location&r=location)
- [Global (country view)](https://nextstrain.org/community/leke-lyu/ncov/global)
- [Global (state view)](https://nextstrain.org/community/leke-lyu/ncov/global?c=division&r=division)
- [Global (county view)](https://nextstrain.org/community/leke-lyu/ncov/global?c=location&r=location)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Running the Build
You can find the config files that runs this build in [here.](https://github.com/leke-lyu/deltaInGreaterHoustonArea)

To replicate this run, you need to first (1) install Nextstrain components and (2) download the ncov workflow. Please visit [this page](https://docs.nextstrain.org/projects/ncov/en/latest/tutorial/setup.html) if you need more instruction on installation.

Once you can run a basic build of the `ncov` repository, clone [this repository](https://github.com/leke-lyu/deltaInGreaterHoustonArea) into the `ncov` folder. To run locally (without any advanced cluster submission), you could type:

```shell
nextstrain build . --configfile deltaInGreaterHoustonArea/builds.yaml 
```


<p align="right">(<a href="#readme-top">back to top</a>)</p>
