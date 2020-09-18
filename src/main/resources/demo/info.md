## Info

This document contains information regarding the vulnerabilities that are injected in the demo. Each vulnerability is injected at the `package_level` detail and both at the `callable_level` detail if a patch is found and a `fasten_uri` is identified corresponding to the changes made in the patch.

| CVE-ID         | maven coordinate                        | NVD                                                     | Patch                                                                                                                                                         |
|----------------|-----------------------------------------|---------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CVE-2017-18640 | org.yaml:snakeyaml:1.18                 | [link](https://nvd.nist.gov/vuln/detail/CVE-2017-18640) | [link](https://bitbucket.org/asomov/snakeyaml/commits/da11ddbd91c1f8392ea932b37fa48110fa54ed8c)                                                               |
| CVE-2012-2098  | org.apache.commons:commons-compress:1.3 | [link](https://nvd.nist.gov/vuln/detail/CVE-2012-2098)  | [link](https://github.com/apache/commons-compress/commit/6ced422bf5eca3aac05396367bafb33ec21bf74e?branch=6ced422bf5eca3aac05396367bafb33ec21bf74e&diff=split) |
| CVE-2019-17571 | log4j:log4j:1.2.17                      | [link](https://nvd.nist.gov/vuln/detail/CVE-2019-17571) | n/a                                                                                                                                                           |
| CVE-2018-10237 | com.google.guava:guava:20.0             | [link](https://nvd.nist.gov/vuln/detail/CVE-2018-10237) | [link](https://github.com/google/guava/commit/7ec8718f1e6e2814dabaa4b9f96b6b33a813101c)                                                                       |
| CVE-2018-11797 | org.apache.pdfbox:pdfbox:2.0.8          | [link](https://nvd.nist.gov/vuln/detail/CVE-2018-11797) | [link](https://github.com/apache/pdfbox/commit/4fa98533358c106522cd1bfe4cd9be2532af852)                                                                       |
| CVE-2018-8036  | org.apache.pdfbox:fontbox:2.0.8         | [link](https://nvd.nist.gov/vuln/detail/CVE-2018-8036)  | n/a                                                                                                                                                           |

## Vulnerable callables 

| CVE-ID  | fasten_uri |
| ------------- | ------------- |
| CVE-2017-18640  | /org.yaml.snakeyaml.composer/Composer.composeNode(%2Forg.yaml.snakeyaml.nodes%2FNode)%2Forg.yaml.snakeyaml.nodes%2FNode  |
| | /org.yaml.snakeyaml.constructor/Constructor.Constructor()%2Fjava.lang%2FVoidType |
| | /org.yaml.snakeyaml.constructor/BaseConstructor.setComposer(%2Forg.yaml.snakeyaml.composer%2FComposer)%2Fjava.lang%2FVoidType |
| CVE-2012-2098  | /org.apache.commons.compress.compressors.bzip2/BZip2CompressorOutputStream.endBlock()%2Fjava.lang%2FVoidType  |
| CVE-2018-10237  | /com.google.common.util.concurrent/AtomicDoubleArray.writeObject(%2Fjava.io%2FObjectOutputStream)%2Fjava.lang%2FVoidType |
| | /com.google.common.io/ByteStreams.toByteArray(%2Fjava.io%2FInputStream)%2Fjava.lang%2FByteType%5B%5D |
