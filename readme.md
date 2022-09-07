#Serverless Frameworkのサンプル

## インストール手順

```
npm install serverless
npm bin serverless
echo 'export PATH="$HOME/node_modules/.bin/:$PATH"' >> ~/.bash_profile
source ~/.bash_profile
sls --version
mkdir serverlss-sample
cd serverlss-sample
sls create -t aws-python3 -n serverlss-sample
npm install --save-dev serverless-offline
```

## ホットリロード
https://github.com/dherault/serverless-offline/issues/1027

```
npm install nodemon --save-dev
npx nodemon -e py --exec sls offline
```
