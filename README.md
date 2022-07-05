# selenium-gcloud

## Use Command

```bash
mkdir -p bin/
curl -SL https://github.com/adieuadieu/serverless-chrome/releases/download/v1.0.0-37/stable-headless-chromium-amazonlinux-2017-03.zip > headless-chromium.zip
unzip headless-chromium.zip -d bin/
rm headless-chromium.zip
```

```bash
curl -SL https://chromedriver.storage.googleapis.com/2.37/chromedriver_linux64.zip > chromedriver.zip
unzip chromedriver.zip -d bin/
rm chromedriver.zip
```

```bash
gcloud functions deploy crawler \
--gen2　\
--region asia-northeast1 \
--runtime python39 \
--allow-unauthenticated \
--trigger-http \
--memory 512MB \
--timeout 540s \
```

# 参考記事

https://zenn.dev/kenghaya/articles/bad86052e475e8

https://cloud.google.com/sdk/gcloud/reference/functions/deploy?hl=ja
