# Deploy NodeJS Service

This workflow deploys a NodeJS service to D2C.

## Usage

```yaml
  - uses: rollun-lc/shared-workflows/nodejs/deploy@master
    with:
      DOCKER_USER: ${{ secrets.DOCKER_USER }}
      DOCKER_PASS: ${{ secrets.DOCKER_PASS }}
      D2C_USER: ${{ secrets.D2C_USER }}
      D2C_PASSWORD: ${{ secrets.D2C_PASSWORD }}
      SM_USER: ${{ secrets.SM_USER }}
      SM_PASSWORD: ${{ secrets.SM_PASSWORD }}
      SERVICE_CONFIG_PATH: './deployment/d2c-service-config.yml'
```