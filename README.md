# Kin-relationship estimation for ancient DNA

## Backgroud information

Archaeogenomic research has proven to be a valuable tool to trace migrations of historic and prehistoric individuals and groups, whereas relationships within a group or burial site have not been investigated to a large extent. Knowing the genetic kinship of historic and prehistoric individuals would give important insights into social structures of ancient and historic cultures. Most archaeogenetic research concerning kinship has been restricted to uniparental markers, while studies using genome-wide information were mainly focused on comparisons between populations. Applications which infer the degree of relationship based on modern-day DNA information typically require diploid genotype data. Low concentration of endogenous DNA, fragmentation and other post-mortem damage to ancient DNA (aDNA) makes the application of such tools unfeasible for most archaeological samples. 

Reference:[Jose Manuel Monroy Kuhn et.al., PLoS One 2018](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0195491)

## Identity by Descent & Identity by	State

The identity by state definition refers to the fact that at some point two individuals, even if they are not related to each other, present the same allele at a specific locus. Because of their un-relatedness this similarity probably arose from a similar mutational event.On the other side, with IBD two individuals happen to share the same allele because of their coancestry.Alleles that are identical by descent are also identical by state. But the opposite is not true. 

A DNA segment is identical by state (IBS) in two or more individuals if they have identical nucleotide sequences in this segment. An IBS segment is identical by descent (IBD) in two or more individuals if they have inherited it from a common ancestor without recombination, that is, the segment has the same ancestral origin in these individuals. DNA segments that are IBD are IBS per definition, but segments that are not IBD can still be IBS due to the same mutations in different individuals or recombinations that do not alter the segment.

The	measurement of SNPs by high	density	microarrays	can	provide	information	about the genotypes among	many loci. SNP genotypes of	two individuals can be compared in terms of	IBS, in which two individuals	are	observed	to	have	identical	0, 1, or 2	alleles	at a given	location.	These	alleles	could	also be IDB	if	0, 1,	or 2 alleles	are	inherited	from a	recent	common	ancestor,	or they	may	be identical	by chance because	the	allele is	very frequent in the	population.

## Related programs

There are many methods for estimating relationship levels implemented in [PLINK](https://www.cog-genomics.org/plink2/), [SNPduo](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0006711), [ERSA](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3083094/), [KING](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3025716/), [REAP](https://www.ncbi.nlm.nih.gov/pmc/articles/pmid/22748210/) and [GRAB](https://www.ncbi.nlm.nih.gov/pmc/articles/pmid/24586241/).

**Note:**

**SNPduo** and **ERSA** may be not suitable for ancient DNA because they require high coverage, diploid genotype data as input.I personally tried [KING](http://people.virginia.edu/~wc9c/KING/manual.html), and it is very easy to work with. And [Martin Sikora et.al. Nature 2019](https://www.nature.com/articles/s41586-019-1279-z) used this program in their paper. However, my kin relationship results on psuedo-haploid SNPs data from [KING](http://people.virginia.edu/~wc9c/KING/manual.html) are different from [READ](https://bitbucket.org/tguenther/read). READ might work better for ancient DNA, in my opinion, see [their paper](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0195491). Or you need diploid data to work with KING. I also tried PLINK using psuedo-haploid SNPs data, it can't predict the relationship, in my opinion, it also need diploid genotype.
