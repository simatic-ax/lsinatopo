
# @simatic-ax/lsinatopo

## Description

This library contains function blocks to read, write and modify the topology of a Siemens SINAMICS S120 drive system from a SIMATIC S7-1500 runtime.  It is a direct conversion of the functionally identical library LSinaTopo for use inside the TIA Portal.

[https://support.industry.siemens.com/cs/document/109770003/](https://support.industry.siemens.com/cs/document/109770003/simatic-library-lsinatopo-sinamics-topology-modifications-at-runtime)

## Getting started

Install with Apax:

> If not yet done login to the GitHub registry first.
> More information you'll find [here](https://github.com/simatic-ax/.github/blob/main/docs/personalaccesstoken.md)

```cli
apax add @simatic-ax/lsinatopo
```

Add the namespace in your ST code:

```iec-st
Using Simatic.Ax.lsinatopo;
```

This library internally uses the library LAcycCom, which is used to handle the acyclic communication. Since the library LSinaTopo is delivered as a binary library, the library LAcycCom is built-in into the library LSinaTopo. Therefore, if you use this library and wish to also use the library LAcycCom, you should not add the library LAcycCom to your project separately, since this would lead to the library being in your project twice, leading to compile errors.

Since this library contains a large number of functionalities that are functionally identical to the library in TIA Portal, detailed content of this library is not described here. For more information, please refer to the original documentation.


## Contribution

Thanks for your interest in contributing. Anybody is free to report bugs, unclear documentation, and other problems regarding this repository in the Issues section or, even better, is free to propose any changes to this repository using Merge Requests.

## Markdownlint-cli

This workspace will be checked by the [markdownlint-cli](https://github.com/igorshubovych/markdownlint-cli) (there is also documented ho to install the tool) tool in the CI workflow automatically.
To avoid, that the CI workflow fails because of the markdown linter, you can check all markdown files locally by running the markdownlint with:

```sh
markdownlint **/*.md --fix
```

## License and Legal information

Please read the [Legal information](LICENSE.md)
