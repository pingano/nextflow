#NextFlow installation

##Getting the right version of Java


Need java 11. Use SDKMAN to handle java versions (https://sdkman.io/ )

```
curl -s "https://get.sdkman.io" | bash
```


We recommend that you install Java through SDKMAN!, and that you use the latest LTS version of Corretto or Temurin. See this website for more information. While other Java distros may work at first or even most of the time, many users have experienced issues that are difficult to debug and are usually resolved by using one of the recommended distros.

To install Corretto 17:
```
sdk install java 17.0.6-amzn
```

To install Temurin 17:
```
sdk install java 17.0.6-tem
```


## Installation of nextflow

```
wget -qO- https://get.nextflow.io | bash
```

Set export CAPSULE_LOG=none to make the dependency installation logs less verbose.


nf-core setup


https://nf-co.re/tools/#downloading-pipelines-for-offline-use

```
pip install nf-core
```

```
nf-core download smrnaseq

                                          ,--./,-.
          ___     __   __   __   ___     /,-._.--~\
    |\ | |__  __ /  ` /  \ |__) |__         }  {
    | \| |       \__, \__/ |  \ |___     \`-._,-`-,
                                          `._,._,'

    nf-core/tools version 2.7.2 - https://nf-co.re


? Select release / branch: 2.1.0  [release]

In addition to the pipeline code, this tool can download software containers.
? Download software container images: singularity

Nextflow and nf-core can use an environment variable called $NXF_SINGULARITY_CACHEDIR that is a path to a directory where remote Singularity images are 
stored. This allows downloaded images to be cached in a central location.
? Define $NXF_SINGULARITY_CACHEDIR for a shared Singularity image download folder? [y/n]: n

If transferring the downloaded files to another system, it can be convenient to have everything compressed in a single file.
This is not recommended when downloading Singularity images, as it can take a long time and saves very little space.
? Choose compression type: none
INFO     Saving 'nf-core/smrnaseq'                                                                                                                          
          Pipeline revision: '2.1.0'                                                                                                                        
          Pull containers: 'singularity'                                                                                                                    
          Output directory: 'nf-core-smrnaseq-2.1.0'                                                                                                        
INFO     Downloading workflow files from GitHub                                                                                                             
INFO     Downloading centralised configs from GitHub                                                                                                        
INFO     Found 19 containers                                                                                                                                
Downloading singularity images ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% • 19/19 completed
```

```

```

https://github.com/nf-core/smrnaseq