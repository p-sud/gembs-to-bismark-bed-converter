# gembs-to-bismark-bed-converter

Simple script to convert [`gemBS`-style CpG BED files](http://statgen.cnag.cat/gemBS/UserGuide/_build/html/pipelineExtract.html#gembs-style-output-files) produced by `gemBS extract` to [Bismark coverage style BED files](https://github.com/FelixKrueger/Bismark/tree/master/Docs#the-coverage-output-looks-like-this-tab-delimited-1-based-genomic-coords). Mainly, we just need to get rid of most of the fields and compute the methylation percentage from the converted and non-converted counts.

Takes about 33.6s to process 45 million records on my machine.

To build from source, clone this repo and run `cargo build --release`.
