# Cookbook Demo Path Manifests

This is a demo web project showing how to use bundlr cli to upload path manifests.

```sh
cd ..
npm i arweave
node -e "require('arweave').init({}).wallets.generate().then(JSON.stringify).then(console.log.bind(console))" > wallet.json
```

```sh
npm i -g @bundlr-network/client
```

```sh
bundlr upload-dir dist -c arweave -h https://node2.bundlr.network -w ../wallet.json --index-file index.html
```