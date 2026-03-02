# sharp-aws-lambda-layer-heif
Aws Lambda layer with Sharp for Nodejs compatibility with heif files

1.- Download zip file
2.- Go to AWS Console
3.- Lambda -> Layers
4.- Create Layer
5.- Wirte a name, Upload zip file, select x86_64 architecture, select Node.js Runtimes
6.- Create
7.- Copy arn
8.- Go to your Lambda function -> layers -> add layer -> specify an ARN -> paste your arn -> add

You can use it using "import sharp from 'sharp';"
IMPORTANT: Make sure you have not any folder /sharp inside node_modules/, if so delete it and delete also instructions from package.json file to avoid install it from console. If you have this folder you can have problems to use it, Lambda will load first from folder and will not use the layer. 

Enjoy it! ;-)
