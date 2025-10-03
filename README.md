# README.md

knowledge base repository using [hugo](https://gohugo.io/) and [hugo book theme](https://hugo-book-demo.netlify.app/)


## Installing latest version of hugo

```bash

export HUGO_VERSION=$(curl --silent "https://api.github.com/repos/gohugoio/hugo/releases/latest" | grep '"tag_name":' | sed -nre 's/^[^0-9]*(([0-9]+\.)*[0-9]+).*/\1/p')

curl --silent -LO "https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_extended_${HUGO_VERSION}_linux-amd64.tar.gz"

tar xfvz "hugo_extended_${HUGO_VERSION}_linux-amd64.tar.gz" hugo

mv hugo ~/bin/

rm  "hugo_extended_${HUGO_VERSION}_linux-amd64.tar.gz"

unset HUGO_VERSION
```


