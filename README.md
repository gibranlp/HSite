# Helgen Technologies [Website](https://helgen.tech)

## Develop

Clone this repo:

```bash
git clone ssh://git.helgen.dev:6611/helgen_website
```

Go into the Website folder and run:

```bash
cd Website
hugo -D server --disableFastRender
```

Now you can check on your browser on **localhost:1313** to view current changes.

## Deploy

## Testing Site

To deploy the changes to testing:

 - You can use **rsync** to upload the files:

 ```bash
rsync -rtvzP ~/Helgen/Website/public/  gibranlp.dev:~/helgen.gibranlp.dev/
```


### Production

To deploy the changes to production:

 - You can use **rsync** to upload the files:

 ```bash
 rsync -rtvzP ~/Helgen/Website/public/ helgen50@192.254.189.34:~/public_html/
 ```

*Your ssh key mut be uploaded first to hostgator and have authorization so it can rsync the files.

