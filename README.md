# Odds-ratio-calculation-in-excel

1) odds ratio (OR) calculation:

The odds ratio tells us the ratio of the odds of an event occuring in a treatment group to the odds of an event occuring in a control group.
For example:

                     non-durable_responders       durable_responders            total
NOTCH1_mutation               5                           4                       9
NOTCH1_wildtype               7                           38                      45
total                         12                          42                      54

so the odds ratio of NOTCH1 mutation in non-durable_responders vs durable_responders is: OR = (5/7)/(4/38) = 6.7857

2) The standard error of the log odds ratio being:
SE{ln(OR)}= SQRT(1/5 + 1/4 + 1/7 + 1/38) = 0.786875


3) 95% confidential interval (CI) calculation:

95% CI = exp ( ln(OR) - 1.96 * SE{ln(OR)} ) to exp ( ln(OR) + 1.96 * SE{ln(OR)} )


4) z statistic

A standard normal deviate (z-value) is calculated as ln(OR) / SE{ln(OR)}

