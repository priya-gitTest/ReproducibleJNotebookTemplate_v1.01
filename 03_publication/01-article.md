---
title: ""
abstract: |
  
acknowledgments: |
 
---

## Introduction
> Start test  with a broad picture of the importance and significance of your chosen field while explaining introductory concepts. State the problem and goals that your research will address. Please cite any referenced literature.

## Materials & Methods

> Describe how you performed your work, referencing methods and procedures of previous research conducted. Focus on the important aspects of your methods and avoid going into too much detail in describing commonly used methods.

### Sample Collection

### Data Analysis

## Results

> Create subsections using repeated `###`s, for example, the results section might have multiple sections.

### Phenotypic Variation Among Populations

Morphological examination of the fruit flies revealed distinct phenotypic variations, particularly in eye color and wing size, across the three sampled populations. The cafeteria population exhibited a higher frequency of red-eyed flies (76%) compared to the biology laboratory (58%) and outdoor green spaces (63%). Similarly, variations in wing size were observed, with larger wings being more prevalent in the outdoor population (68%) compared to the cafeteria (49%) and laboratory populations (53%) [See @tab:phenotypic-variation].

> There are a few ways to create tables, you can use a markdown table or a list-table (see [table documentation](https://mystmd.org/guide/tables)).
> @tab:phenotypic-variation shows a markdown table, which is wrapped in a `:::{table}` directive.

:::{table}
:label: tab:phenotypic-variation

Morphological examination of the fruit flies revealed distinct phenotypic variations across the three sampled populations.
The source for this data can be found in [](.01/data/1_fruit_fly_data.csv).

| Environment          | Red-Eyed Flies (%) | Larger Wings (%) |
| -------------------- | ------------------ | ---------------- |
| Cafeteria            | 76%                | 49%              |
| Biology Laboratory   | 58%                | 53%              |
| Outdoor Green Spaces | 63%                | 68%              |

:::

### Statistical Analysis of Phenotypic Differences

> Math can be included using the ` ```{math} ` directive with a label, and cross-referenced in the same way as figures.
> Math syntax is written in LaTeX, see the [math documentation](https://mystmd.org/guide/math).
> Inline math is surrounded by dollar-signs, for example, $\chi^2$.

Chi-square tests were conducted to evaluate the statistical significance of the observed differences in phenotypic traits between the fruit fly populations from different environments. We used the chi-squared formula @eq:chi-squared to do the analysis.

```{math}
:label: eq:chi-squared
\chi^2=\sum_{i=1}^{n} \frac{(O_i - E_i)^2}{E_i}
```

The analysis for eye color variation yielded a chi-square statistic of 7.66 with a p-value of 0.022 ($\chi^2$ = 7.66, df = 2, p < 0.05), indicating statistically significant differences in eye color distribution across environments. This suggests that the variation in eye color among the populations could indeed be influenced by their respective environmental conditions.

Similarly, the analysis for wing size variation showed a chi-square statistic of 8.17 with a p-value of 0.017 ($\chi^2$ = 8.17, df = 2, p < 0.05). The differences in wing size across populations are also statistically significant. This finding suggests that, like eye color, the variation in wing size is likely influenced by environmental factors, rather than being a result of random variation.

> When including computational results, ensure to link to your original source in your notebooks or other source files.
> This ensures your research is reproducible.

The results prompt a discussion on the role of environmental factors in shaping genetic variation within populations, which can be seen in @fig:environment. The significant variation in eye color across populations suggests a potential adaptive response to different environmental conditions encountered in each habitat. The lack of significant difference in wing size may indicate that this trait is less sensitive to environmental variation or that the sample size and environmental differences were not sufficient to reveal a significant adaptive pattern.

> In this example, we are linking a figure output from our Jupyter Notebook analysis. See the [documentation on linking outputs](https://mystmd.org/guide/reuse-jupyter-outputs). You will see the line `#| label: nb:analysis` in our Jupyter Notebook.

:::{figure} #nb:analysis
:label: fig:environment
Phenotypic variations in [Drosophila melanogaster] across different environments. It compares the percentage of red-eyed flies and flies with larger wings in the cafeteria, biology laboratory, and outdoor green spaces, providing a visual representation of how these traits vary across the sampled populations.
:::

## Discussion

> Demonstrate how your results are statistically significant and address the research questions posed in the introduction. Interpret your results and the implications of your findings with respect to your field and describe their possible applications.


## Conclusion

> Recap briefly what was learned from your research and assess the validity of your conclusions. Consider what questions might still remain to be answered and put them in terms of future work and how your research could act as a foundation in addressing these questions.