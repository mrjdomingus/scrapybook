# Errata
**Support Query**

Trying to setup the vagrant env when reading the book "Learning Scrapy", but failed to log into the dev container when running "vagrant ssh". I found sth in the log of running "vagrant up --no-parallel" 
==> dev: Starting container...

==> dev: Provisioners will not be run since container doesn't support SSH.


Solution: [https://github.com/scalingexcellence/scrapybook/issues/5#issuecomment-231628448](https://github.com/scalingexcellence/scrapybook/issues/5#issuecomment-231628448)

[https://github.com/scalingexcellence/scrapybook/issues/10](https://github.com/scalingexcellence/scrapybook/issues/10)

**Errata type: Technical l Page no: 21**

This:

• Getting the text of the span under the div with id "firstHeading":
`//h1[@id="firstHeading"]/span/text()`

Should be:

• Getting the text of the span under the h1 with id “firstHeading”.
`//h1[@id="firs`

**Errata Type: Technical |Page: 21**

It is:

To select all the URLs of links under the div element following an element
whose child element contains the text "References":
`//*[text()="References"]/../following-sibling::div//a`

Should be:

To select all the URLs of links under the div element following an element
whose child element contains the text "References":
`//*[test()="References"]/../following-sibling::div//a/@href`
