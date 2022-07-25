# Host Hugo on Github Pages with Custom Domain

1. Rename publish directory and set base url in [`config.yaml`](/config.yaml)

    ```yaml
    baseURL: https://www.puplakto.com
    ...
    publishDir: docs
    ```

2. Set source to `/docs` and set custom domain to `www.puplakto.com` in https://github.com/puplakto/blog/settings/pages

3. Add a CNAME record in DNS, pointing `www.puplakto.com` to `puplakto.github.io`

4. Run `hugo -D` and push the repo, wait for Github Action workflow to complete.