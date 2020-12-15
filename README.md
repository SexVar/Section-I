This is Section I of an incomplete multi-part project. The introduction is [here](https://github.com/SexVar/Intro).

This section is incomplete: figures 2-4 are not yet inserted.

# Section I: Simulation Studies

Researchers have previously observed that larger samples are needed to reliably detect typical group differences in variability than in central tendency, and that random sampling error can easily cancel or reverse sex differences in variance (Feingold, 1992, p. 80; Fraser Roberts, 1945, p. 727; Jensen, 1980, pp. 627f.). Results of three simulation studies will be presented to emphasize and delineate this issue.

Levene’s (1960) test is widely used to test the null hypothesis of homogeneity of variance between two groups. His original version used the mean as the centering parameter but the median-based variant, also known as the Brown-Forsythe test, is among the most robust procedures, with higher power and better control of type I error than many other tests across diverse distributions (Brown & Forsythe, 1974; Conover et al., 1981, 2018; Lim & Loh, 1996; Rosopa et al., 2013; Sharma & Kibria, 2013).

The “real VR” will be shorthand for the expected value of an observed VR when sampling from a given pair of distributions. Figure 2 displays sample sizes and their associated levels of power for the median-based Levene’s test. Each power estimate is the result of performing the test on ten million simulated samples using the “car” package (Fox & Weisberg, 2019). Figure 2a presents the procedure’s power in balanced samples up to 15,000. How many participants are needed to detect unequal variances between two equally numerous, normally distributed groups at the 5% significance level with 95% power? When the real VR=1.40, a total of about 1,060 participants; when the real VR=1.30, about 1,730; when the real VR=1.20, roughly 3,580; and when the real VR=1.10, about 13,080. Figure 2b zooms in on sample sizes up to 1,000, a range which encompasses a vast majority of studies of cognitive sex differences. Power for samples with 100 total participants ranges from 5.5% to 18% across the different VRs shown. With 300 participants, power is at 8.2% for VR=1.10 and still less than 50% for VR=1.40. Even with 1,000 participants, there is 17% power to detect a difference when VR=1.10, and only VR=1.40 exceeds 80% power.

[Figure 2 here]

As will be shown later, sex differences in variance are often small and usually do not exceed 30%. Researchers analyzing samples of typical sizes should not view a nonsignificant result from Levene’s test as strong evidence for homogeneity of variance, although some have done so (e.g., Merel Bakker et al., 2019; Kersey et al., 2018; Vista & Care, 2011). For instance, Kersey and colleagues (2018) performed Levene’s procedure on cognitive test scores in slightly unbalanced samples ranging in size from 80 to 275. They reported power analyses for mean differences but did not mention the low power for Levene’s test. Although they found homogeneous variance in every sample, it is clear from Figure 2b that their sample sizes made this conclusion nearly inevitable. And naturally, small samples do not merely render Levene’s test impotent. They also cannot generate a reliably accurate estimate of the VR.

Figure 3 serves as a quantitative illustration of deviations from the real VR due to random sampling error. The main indicator is the directional error rate: the percentage of observed VRs that are less than 1. All real VRs are greater than 1 here, so observed VRs < 1 are qualitatively incorrect. Balanced samples ranging in size from 20 to 3,000 were drawn from normal distributions with real VRs ranging from 1.10 to 1.40. For each data point, this was done ten million times. The directional error rate is higher when the real VR is closer to 1 and when the spread of observed VRs is wider, as in smaller samples. Thus, samples of 20 taken from a population with a real VR of 1.10 show the highest rate of directional error: 44.5%, compared to a random baseline of 50%. With 1,000 participants and a real VR of 1.10, the rate is about 1 in 7. It sinks below 1% at about n=4,800 (not shown in plot). For real VRs of 1.30 and 1.40, directional error rates eventually fall to (nearly) zero, in which none of the simulated VRs were less than 1.

[Figure 3 here]

Figure 4 illustrates the same concept for observed TPRs, with cut-points of 1% and 10% and real TPRs of 1.10, 1.20, and 1.50. Tail size refers to the number of data points beyond the cut-point, and it ranges from 10 to 1,000. For instance, the tail size beyond a 10% cut-point in a sample of 300 is 30. Unlimited combinations of mean and variance differences could produce a given TPR beyond a given cut-point. In actual data the highest TPRs are produced by concordant contributions from mean and variance differences (e.g., Hedges & Nowell, 1995). For clarity, in Fig. 3 simulations the real TPRs depart from 1 due only to differences in variance; there are no mean differences between the two groups. Due to the symmetry in these simulations, the bottom and top of the distributions have the same TPRs, so the cut-points refer to both tails (e.g., top and bottom 1%).

A far more extensive display, Table S4, is provided in the supplement with mean differences and higher TPRs. The results in Fig. 4 and Table S4 show that the directional error rate is determined almost entirely by the real TPR and the tail size. Results are barely swayed by modulating combinations of mean and variance differences to produce the same real TPR, or by modulating combinations of sample size and cut-point to produce the same tail size. For instance, with a real TPR of 1.10, it hardly matters whether there is a sample of 7,000 and a cut-point of 1% or a sample of 700 and a cut-point of 10%, because the tail size is 70 in both cases. Although the sample sizes and cut-points differ by a factor of ten, the directional error rates are similar: 34.4% in the former case and 33.3% in the latter case. The values for Fig. 4 and Table S4 were computed by simulating ten million observed TPRs per data point.

[Figure 4 here]

It should be remembered that the real VR or TPR is always unknown — we can access only the observed values — and that the data reflect patterns in samples drawn from perfectly normal populations with no systematic error, unlike data from real samples (Dykiert et al., 2009; Lynn & Kanazawa, 2011; Madhyastha et al., 2009). They also do not account for random measurement error. Perhaps even more importantly, these results apply to simple random samples. Complex sample designs are common among those considered in this article, because they are generally a practical requirement to collect large samples. Three features primarily distinguish a complex sample from a simple random sample: clustering, weighting, and stratification. Relative to simple random designs, cluster sampling increases uncertainty of estimates because observations within each cluster are correlated, and thus provide less information than independent observations. Various factors in complex sample designs lead to differential weighting of observations, which strongly tends to expand uncertainty of estimates. Stratification tempers these effects if executed properly, but in general complex samples are less efficient than simple random samples.

For any estimate, a “design effect” expresses the factor by which the actual sample size should be divided to give the “effective sample size”, which is the sample size required to reach the same precision with a simple random design (Heeringa et al., 2010). A sample of 4,000 with a design effect of 2 for a particular estimate has an effective sample size of 2,000. The large-scale international assessments analyzed in section IV are exemplars of clustered, stratified sampling. To provide a relevant sense of magnitude, I computed design effects for sex differences in TIMSS 2015 math scores in all 47 countries with grade 4 samples (Mullis et al., 2016).<sup>1</sup> For variance differences, they ranged from 1.2 to 7.6 with a median of 2.5. Design effects for mean differences were somewhat larger: they ranged from 1.7 to 11.9 with a median of 3.7. So the distinction between actual and effective sample sizes can be considerable. Throughout this article I will report actual sample sizes only, because it is not possible to determine the design effect for a summary statistic unless it is accompanied by an expression of its uncertainty. Nevertheless, there are two valuable implications. First, many samples will be discussed throughout this article, most of which were collected with complex sampling designs. It should be kept in mind that the effective sample sizes of their estimates are likely to be smaller than the actual sample sizes. Second, the effective sample size is how a complex sample should be viewed when consulting these simulations.

Later I will argue that apparent inconsistencies in this literature are partly the product of overconfidence in small samples. There is reason to believe that psychologists do not always perceive the limitations of small samples. Marjan Bakker and colleagues (2016) found that most psychological researchers in their sample overestimated the power of their own published tests, most did not conduct power analyses for these tests, and a vast majority overestimated the power of a small-sample t-test. 95% of the respondents underestimated the number of participants needed to achieve 80% power for a given small effect. Schmidt and Hunter (2015, p. 12) attested that researchers were shocked by the results of their study which drew small subsamples from a large data set and demonstrated the wide variation which springs purely from random sampling error (Schmidt et al., 1985). These misunderstandings accord with decades of documentation of underpowered studies in psychology (e.g., Sedlmeier & Gigerenzer, 1989).

It is hopefully clear that sample sizes which are impressive for many purposes can constitute weak evidence on the matter of group differences in variability. Complex sampling designs tend to yield lower precision than expected from their sample size, so very large samples are needed to achieve adequate effective sample sizes. An inclusion threshold of 1,000 will therefore be enforced for the sample sizes of all assessments considered in this study. Because this is a prerequisite for inclusion but not a mark of high reliability, occasional distinctions will also be made using 5,000 as a threshold. Aside from diminishing the formidable problem of random sampling error, large studies are more likely to engage in deliberately representative sampling. They arguably inhibit publication bias, because many were not conducted with the purpose of examining sex differences — especially not in variability — and it seems less likely that massive efforts to collect many participants would be discarded without publication. Self-selected or otherwise non-representative samples, such as the International Mathematical Olympiad, are unsuitable for examining population-level sex differences. Despite these standards, a great deal of evidence remains.

&nbsp;

<sup>1</sup> The international assessments like TIMSS use planned missing data designs because the number of items is too high for any single student to answer. The total design effects, conceived more broadly, are therefore larger than calculated here, because they include imputation variance as well as sampling variance. Imputation variance was ignored here because this was a demonstration of the effects of sampling design rather than test design.

&nbsp;

## References

Bakker, M. [Marjan], Hartgerink, C. H., Wicherts, J. M., & van der Maas, H. L. (2016). Researchers’ intuitions about power in psychological research. _Psychological Science_, _27_(8), 1069-1077.

Bakker, M. [Merel], Torbeyns, J., Wijns, N., Verschaffel, L., & De Smedt, B. (2019). Gender equality in 4‐to 5‐year‐old preschoolers’ early numerical competencies. Developmental Science, 22(1), e12718.

Kersey, A. J., Braham, E. J., Csumitta, K. D., Libertus, M. E., & Cantlon, J. F. (2018). No intrinsic gender differences in children’s earliest numerical abilities. _npj Science of Learning_, 3, 12.

Brown, M. B. & Forsythe, A. B. (1974). Robust tests for the equality of variances. _Journal of the American Statistical Association_, _69_(346), 364-367.

Conover, W. J., Johnson, M. E., & Johnson, M. M. (1981). A comparative study of tests for homogeneity of variances, with applications to the outer continental shelf bidding data. _Technometrics_, _23_(4), 351-361.

Conover, W. J., Guerrero-Serrano, A. J., & Tercero-Gómez, V. G. (2018). An update on ‘a comparative study of tests for homogeneity of variance’. _Journal of Statistical Computation and Simulation_, _88_(8), 1454-1469.

Dykiert, D., Gale, C. R., & Deary, I. J. (2009). Are apparent sex differences in mean IQ scores created in part by sample restriction and increased male variance?. _Intelligence_, _37_(1), 42-47.

Feingold, A. (1992). Sex differences in variability in intellectual abilities: A new look at an old controversy. _Review of Educational Research_, _62_(1), 61-84.

Feingold, A. (1994). Gender differences in variability in intellectual abilities: A cross-cultural perspective. _Sex Roles_, _30_(1-2), 81-92.

Fox, J. & Weisberg, S. (2019). _An R companion to applied regression_. SAGE Publications.

Fraser Roberts, J. A. (1945). On the difference between the sexes in dispersion of intelligence. _British Medical Journal_, _1_(4403), 727-730.

Hedges, L. V. & Nowell, A. (1995). Sex differences in mental test scores, variability, and numbers of high-scoring individuals. _Science_, _269_(5220), 41-45.

Heeringa, S. G., West, B. T., & Berglund, P. A. (2010). Getting to know the complex sample design. In _Applied survey data analysis_ (pp. 13-51). CRC Press.

Jensen, A. R. (1980). _Bias in mental testing_. New York, NY: Macmillan.

Levene, H. (1960). Robust tests for equality of variances. In I. Olkin, S. G. Ghurye, W. Hoeffding, W. G. Madow, & H. B. Mann (Eds.), _Contributions to probability and statistics: Essays in honor of Harold Hotelling_ (pp. 278-292). Stanford, CA: Stanford University Press.

Lim, T. S., & Loh, W. Y. (1996). A comparison of tests of equality of variances. _Computational Statistics & Data Analysis_, _22_(3), 287-301.

Lynn, R. & Kanazawa, S. (2011). A longitudinal study of sex differences in intelligence at ages 7, 11 and 16 years. _Personality and Individual Differences_, _51_(3), 321-324.

Madhyastha, T. M., Hunt, E., Deary, I. J., Gale, C. R., & Dykiert, D. (2009). Recruitment modeling applied to longitudinal studies of group differences in intelligence. _Intelligence_, _37_(4), 422-427.

Mullis, I. V. S., Martin, M. O., Foy, P., & Hooper, M. (2016). _TIMSS 2015 international results in mathematics_. Chestnut Hill, MA: Boston College.

Rosopa, P. J., Schaffer, M. M., & Schroeder, A. N. (2013). Managing heteroscedasticity in general linear models. _Psychological Methods_, _18_(3), 335-351.

Schmidt, F. L., & Hunter, J. E. (2015). _Methods of meta-analysis: Correcting error and bias in research synthesis_ (3rd ed.). SAGE Publications.

Schmidt, F. L., Ocasio, B. P., Hillery, J. M., & Hunter, J. E. (1985). Further within‐setting empirical tests of the situational specificity hypothesis in personnel selection. _Personnel Psychology_, _38_(3), 509-524.

Sedlmeier, P. & Gigerenzer, G. (1989). Do studies of statistical power have an effect on the power of studies?. _Psychological Bulletin_, _105_(2), 309-316.

Sharma, D. & Kibria, B. M. G. (2013). On some test statistics for testing homogeneity of variances: a comparative study. _Journal of Statistical Computation and Simulation_, _83_(10), 1944-1963.

Vista, A. & Care, E. (2011). Gender differences in variance and means on the Naglieri Non‐verbal Ability Test: Data from the Philippines. _British Journal of Educational Psychology_, _81_(2), 292-308.
