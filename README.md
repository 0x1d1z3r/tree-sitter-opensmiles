# tree-sitter-opensmiles
This is a [Tree-sitter](https://github.com/tree-sitter/tree-sitter) grammar implementing the [OpenSmiles specification](http://opensmiles.org/opensmiles.html)
# DONT USE RIGHT NOW
It has a fatal flaw , which occurs when bonds are specified e.g. for C=C (Ethylene) and C1C=C1 (Cyclopropene)
## How to run
	git clone https://github.com/0x1d1z3r/tree-sitter-opensmiles
 	cd tree-sitter-opensmiles
  
	npm install --save-dev tree-sitter-cli				# install Tree-sitter
	export PATH=$PATH:./node_modules/.bin 				# set $PATH 
 
	treesitter generate                   				# generate parser 
 
 	tree-sitter build --wasm					# only needed for playground
	treesitter playground                 				# interactive example
     

## Additional Files
A pure BNF (non LL) grammar for [OpenSmiles](http://opensmiles.org/) is included in *grammar.bnf*

It is modified for use in [BNFPlayground](https://github.com/paul-kline/bnf-playground) without EBNF syntax

