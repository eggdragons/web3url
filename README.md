This repository is a repository for experiencing web3URL.
Static HTML created using Nextjs is a lot of data, and it costs a lot of gas!
The exact same site created using only html will be index2.html.

| folder / file | volume | gas     |
| ------------- | ------ | ------- |
| out           | 300kB  | 6.38ETH |
| index2.html   | 3kB    | 0.06ETH |

## Getting Started

```
npm i
```

## Create static HTML

```
npm run export
```

## Create Upload contract

```
npx ethfs-uploader --create --privateKey {privateKey} --chainId 5
```

## Upload file

Single file

```
npx ethfs-uploader {~/web3url/index2.html} gor:{FlatDirectory Address} --privateKey {privateKey}
```

Multiple files

```

npx ethfs-uploader {~/web3url/out} gor:{FlatDirectory Address} --privateKey {privateKey}
```
