# Nanopubs for FDOs: Demo

---

This demo gives you a quick hands-on introduction into the work-in-progress solution of using [nanopublications](https://nanopub.net) to implement [FAIR Digital Objects (FDOs)](https://fairdo.org/).

You might also want to check out [this general demo about nanopublications](.).

--- 

## 1. Login to Nanodash

To try out the steps below on your own, you'll need to login to the [Nanodash](https://nanodash.knowledgepixels.com/) interface with your [ORCID](https://orcid.org/) account.

[Register](https://orcid.org/register) to get such an ORCID account for free, if you don't have one already.


## 2. Defining FDOs with nanopublications via Nanodash

Publish one or more nanopublications from these templates:

- [Defining an FDO](https://nanodash.knowledgepixels.com/publish?template=https://w3id.org/np/RAei7xbeufZtrwog4_xImDCX5wrSZspYKZeUIx_EComBw&template-version=latest)
- [Defining a new class (FDO types could be defined similarly in the future)](https://nanodash.knowledgepixels.com/publish?template=https://w3id.org/np/RAxfD9wQMHU4DmWta5uRpo723ZgKpizglley4gtcxG0hg&template-version=latest)

(You can find more templates on other topics [here](https://nanodash.knowledgepixels.com/publish).)


## 3. Check out published nanopublications/FDOs

All nanopublications are published to a [decentralized network of services](https://monitor.knowledgepixels.com/).

We can access this knowledge with pre-defined queries like these:

- [See all FDOs defined in nanopublications](https://nanodash.knowledgepixels.com/resulttable?query=RAZgtM7Kzb0aTBlH4coOzlfgzBOoofqROCIMZTW3KliLQ/get-fdos)
- [Latest nanopublications (without example nanopublications)](https://nanodash.knowledgepixels.com/resulttable?query=RAAq7D8hWYXL-XTflG1u19maDe7nSJy6Iun5wa_KadOqg/get-latest-nanopubs)
- [Latest example nanopublications](https://nanodash.knowledgepixels.com/resulttable?query=RAlmS9Sp0Cjxv6vyiJff6TWWqNfJXj7LmkdoLNy6ZSeJ8/get-latest-example-nanopubs)

You can also access these nanopublications through custom queries via the technical SPARQL interfaces:

- [SPARQL endpoint with all nanopublications](https://query.knowledgepixels.com/tools/full/yasgui.html)
- [SPARQL endpoint with FDO nanopublications only](https://query.knowledgepixels.com/tools/type/f82fa5e467e6ba40c5d14402c3590f2ad8ed9a13e982133ab26ef1a889b34ebd/yasgui.html)

## 4. HTTP access of FDO metadata/content

Get FDO metadata as TriG:

    $ curl -L \
        -H 'FDO: metadata' \
        -H 'Accept: application/trig' \
        'https://w3id.org/np/RAwToTy-lTyJDU9SkYryUp9yjrQx-rokX_M4sz85MQpmA#abc-table'

The header `FDO: metadata` is optional, as the metadata is returned by default. You can also try `application/ld+json` or `application/trix` as format in the Accept header.

Get FDO content in specified format:

    $ curl -L \
        -H 'FDO: object' \
        -H 'Accept: text/csv' \
        'https://w3id.org/np/RAwToTy-lTyJDU9SkYryUp9yjrQx-rokX_M4sz85MQpmA#abc-table'

In this particular example, the Accept header can be set to `application/vnd.ms-excel` to get the same table in Excel format.

---
