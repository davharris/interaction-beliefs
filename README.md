What do ecologists believe about species interaction matrices?
===================

I'm thinking about how one would design generic priors over possible species interaction matrices.  Of course, natural history and experiments are the best ways to learn about species interactions, but I'm interested in methods that can scale to many thousands of species pairs.

This could eventually become a paper, but for now it's just scribbling.  Please submit pull requests or issues if you have ideas/references/other contributions.

Here are some hypotheses that may or may not be supported by the literature, but which should be falsifiable:

* Similar species (e.g. close relatives or guildmates) are more likely to compete (or at least more likely to interact)
  * Quantitatively: expected interaction strength should decay with phylogenetic/trait/niche distance
* Species with similar resource needs are more likely to compete
  * Quantitatively: expect more negative interaction strengths between species with more similar niches
* Most pairs of [non-sessile?] species interact weakly, if at all
  * Quantitatively: leptokurtic priors, with most interaction terms close to zero compared with the extremes
* Species interactions are strongest at small spatial scales
  * Quantitatively: expect larger magnitudes at small spatial scales
* Generalists mainly interact along a few important resource axes; specialists' interactions are more idiosyncratic
  * Quantitatively: ??
