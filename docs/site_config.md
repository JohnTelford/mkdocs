<!-- ## site_config.md -->

## Cloudflare deployment root files

[Cloudflare Pages](https://starfallprojects.co.uk/projects/deploy-host-docs/deploy-mkdocs-material-cloudflare/)

- mkdocs root dir `requirements.txt` 

    - mkdocs-material version  
  
    - pip show mkdocs-material  

    - mkdocs-material==<mkdocs-material version>



- mkdocs root dir `runtime.txt` Python version 3.7  

    3.7

- Environment variables:  
  
    Variable name: ZOLA_VERSION
    
    Value: 0.13.0

## Upgrade Material MkDocs

Upgrade to the latest version with:

`pip install --upgrade --force-reinstall mkdocs-material`

Show the currently installed version with:

`pip show mkdocs-material`
