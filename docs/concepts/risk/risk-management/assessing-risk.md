# Assessing Risk

## Terminology

### Acronyms

| Acronym | Definition |
| :--- | :--- |
| ALE | Annualized Loss Expectancy |
| ARO | Annual Rate of Occurrence |
| AV | Asset Value |
| EF | Exposure Factor |
| SLE | Single Loss Expectancy |

### Definitions

#### ALE

The annualized loss expectancy is a product of the yearly estimate for the exploit \(ARO\) and the loss in value of an asset after an SLE.

`ALE = SLE * ARO`

#### ARO

The annual rate of occurrence is an estimate of how often a threat will be successful in exploiting a vulnerability over the period of a year.

While previous activity is not a great predictor of future outcomes, historical data can sometimes help you predict the annualized rate of occurrence for a specific loss.

#### AV

The asset value is represented as a dollar value.

#### Delphi Technique

The Delphi technique is a qualitative method of group decision-making that involves successively collating the judgment of the group.

#### EF

The exposure factor is the estimated loss that will result if the risk occurs. The threat vector is the multiplier involved in determining exposure factor.

The exposure factor is represented as a percentage.

#### Impact

Impact includes loss of life, loss of dollars, loss of prestige, loss of market share, and other facets. Unlike risk, impact uses definitions rather than an ordinal scale for measuring.

#### Risk

The probability of a threat materializing; the likelihood an impact will be realized.

- Risk can be reduced but never eliminated.
- Risks arise from the loss of CIA of information or information systems.
- Risks reflect the potential adverse impacts to organizational operations \(mission, functions, image, or reputation\), organizational assets, individuals, or other organizations.

#### SLE

Single-loss expectancy must be calculated to provide an estimate of loss. SLE is defined as the difference between the original value and the remaining value of an asset after a single exploit.

The monetary value of the asset is the most objective, discrete metric possible and the most accurate for the purposes of SLE determination. In the formula below, SLE is a dollar value.

`SLE$ = AV$ * EF%`

#### Threat

Any **circumstance or event with the potential to adversely impact** organizational operations and assets, individuals, other organizations, or the Nation through an information system via unauthorized access, destructions, disclosure, or modification of information, and/or denial-of-service.

Any potential danger that is associated with the exploitation of a vulnerability.

#### Threat Source

Either intent and method targeted at the intentional **exploitation of a vulnerability** or a situation and method that may **accidentally trigger a vulnerability.**

#### Threat Vector

A threat vector is the multiplier involved in determining exposure factor.

#### Vulnerability

An inherent **weakness** in an information system, security procedures, internal controls, or implementation that could be exploited by a threat source.

A lack of a countermeasure or a weakness in a countermeasure that is in place.

## Overview

Risk assessment is the process used to identify, estimate, and prioritize information security risks.

Risks must be communicated in a way that is clear and easy to understand. It may also be important to communicate risk information outside the organization. To be successful in this, the organization must agree to a set of risk-management metrics.

Risk is determined as the by-product of likelihood and impact. For example, if an exploit has a likelihood of 1 \(high\) and an impact of 100 \(high\), the risk would be 100. As a result, 100 would be the highest exploit ranking available.

:::info
No countermeasure should be greater in cost than the risk it mitigates, transfers, or avoids.
:::

The purpose of engaging in risk assessment is to identify:

- Threats to organizations \(i.e., operations, assets, or individuals\) or threats directed through organizations against other organizations.
- Vulnerabilities internal and external to organizations.
- The harm \(i.e., adverse impact\) that may occur given the potential for threats exploiting vulnerabilities.
- The likelihood that harm will occur.

There are additional cloud-specific risk concerns that should also be considered:

- Risk of service failure and associated impact
- Insider threat risk impact
- Risk of compromised customer to other tenants in the cloud environment
- Risk of DoS attacks
- Supply chain risk to the CSP

Identifying these factors helps to determine risk, which includes the likelihood of harm occurring and the potential degree of harm. Using a risk scorecard is recommended. The impact \(consequence\) and probability \(likelihood\) of each risk are assessed separately, and then the results are combined.

![Risk Ranking](/img/risk-ranking.png)

### Threat Categories

- Human
- Natural
- Technical
- Physical
- Environmental
- Operational

## Risk Assessments

:::info
Risk assessments should be performed *periodically*.
:::

### Qualitative Risk Assessments

Qualitative risk assessments typically employ a set of methods, principles, or rules for assessing risk based on **non-numerical** categories or levels \(such as high, medium, or low\). Qualitative risk assessments use subjective analysis to help prioritize probability and impact of risk events.

The opinion of an expert in the field is a prime source for qualitative analysis. Interviews and risk workshops are two ways in which you can work with experts on managing qualitative risk.

#### Characteristics

- Assessors have limited expertise in quantitative assessments \(assessors do not require as much experience when performing a qualitative assessment\)
- The timeframe to complete the assessment is short
- Implementation is easier
- The organization doesn't have enough data for a quantitative assessment
- The assessors are long-term employees who have experience with the *business* and *critical systems*
- Results that are descriptive versus measurable

#### Process

- Management approval is obtained and management is kept informed
- A risk-assessment team can be formed. Members may include staff from senior management, IS, legal or compliance, internal audit, HR, facilities and safety coordination, IT, and business owners, as appropriate.
- The assessment team requests documentation
- The team sets up interviews with organizational members to identify vulnerabilities, threats, and countermeasures. All levels of staff should be represented.
- The analysis of the data gathered can be completed, which typically includes matching the threat to a vulnerability, matching threats to assets, determining how likely the threat is to exploit the vulnerability, and determining the impact to the organization in the event an exploit is successful. Analysis also includes matching of current and planned countermeasures to the threat-vulnerability pair.
- When matching is completed, risk can be calculated. In qualitative analysis, the product of likelihood and impact produces the level of risk.
- Once risk is determined, additional countermeasures can be recommended to minimize, transfer, or avoid the risk.
- When this is completed, the risk that is left over-after countermeasures have been applied to protect against the risk-is also calculated. This is the **residual risk.**

### Quantitative Risk Assessments

Quantitative risk assessments typically employ a set of methods, principles, or rules for assessing risk based on the use of **numbers.** 

The hallmark of a quantitative assessment is the numeric nature of the analysis. Frequency, probability, impact, countermeasure effectiveness, and other aspects of the risk assessment have a discrete mathematical value in a pure quantitative analysis.

#### Characteristics

- Allows the assessor to determine whether the cost of the risk outweighs the cost of the countermeasure
- Requires a lot of time
- Must be performed by assessors with a significant amount of experience and particular skillset
- Subjectivity is introduced because the metrics may need to be applied to qualitative measures
- This type of assessment most effectively supports **cost-benefit analyses**

:::info
Most organizations are not in a position to authorize the level of work required for a quantitative risk assessment.
:::

#### Process

Three steps are undertaken in a quantitative risk assessment:

1. Management approval
2. Define risk assessment team
3. Review information available within the organization

:::info
Quantitative risk assessments often use values such as AV, EF, SLE, ARO, and ALE to quantify risk. Quantitative assessments lead to the proper mitigation strategy by specifying a **dollar value** for risks.
:::

:::info
Often, the risk assessment an organization conducts is a combination of qualitative and quantitative methods. Fully quantitative risk assessment may not be possible because there is always some subjective input present, such as the value of information. Value of information is often one of the most difficult factors to calculate.
:::

## Vulnerability Assessments

Unlike a risk assessment, vulnerability assessments tend to focus on the technology aspects of an organization, such as the network or applications. Data gathering for vulnerability assessments typically includes the use of software tools.