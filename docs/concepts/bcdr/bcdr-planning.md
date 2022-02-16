# BCDR Planning

## 1. Define Scope

## 2. Gather Requirements

In migrating to a cloud service architecture, your organization will want to review its existing BIA and consider a new BIA, or at least a partial assessment, for cloud-specific concerns and the new risks and opportunities offered by the cloud.

[BIA](../business/business-requirements/bia.md)

Potential emergent BIA concerns include, but are not limited to, the following:

- New Dependencies
- Regulatory Failure
- Data Breach/Inadvertent Disclosure
- Vendor Lock-In/Lock-Out

## 3. Analyze

Will our plan meet the metrics specified in the previous step?

## 4. Assess

[Assessing Risk](../risk/risk-management/assessing-risk.md)

## 5. Design

Should address technical alternatives, procedures, workflow, staff, other business necessities.

## 6. Implement

Implement plan, exercising, assessing, and maintaining the plan.

## 7. Test

Any BCDR plan should be tested at **regular intervals.**

- Tabletop Exercise
- Walk-Through Drill
- Functional Drill
- Full-Interruption

There are two reasons to conduct a test of the organization's recovery from backup in an environment other than the primary production environment:

- You want to approximate contingency conditions, which includes not operating in the primary location. Assuming your facility is not available during contingency operations allows you to better simulate an emergency situation, which adds realism to the test.
- The risk of negative impact to both production and backup is too high. A recovery from backup into the *production* environment carries the risk of failure of both data sets \(the production and the backup set\).

### Tabletop Exercise

Essential participants work together at a scheduled time to describe how they would perform their tasks in a given BCDR scenario.

:::info
This has the **least impact** on production of the testing alternatives, but is also the **least thorough.**
:::

### Walk-Through Drill

Simulates a disaster scenario but only includes operational and support personnel. It is more complicated than a tabletop exercise. Attendees practice certain functional steps to ensure that they have the knowledge and skills needed to complete them. Acting out the critical steps, recognizing difficulties, and resolving problems is critical for this type of test.

Moves beyond the involvement of a tabletop exercise. Chooses a specific event scenario and applies the BCP to it.

Specific characteristics include:

- Practice and validation of specific functional response capabilities
- Demonstration of knowledge as well as team interaction
- Role playing with simulated response at alternate locations
- Mobilization of the crisis management and response team
- Actual resource mobilization to reinforce the content of the plan

### Functional Drill

Involves moving personnel to the recovery site\(s\) to attempt to establish communications and perform real recovery processing. The drill will help the organization determine whether following the BCP will successfully recover critical systems at an alternate processing site. Because a functional drive fully tests the BCP, all employees are involved. It demonstrates emergency management capabilities and tests procedures for evacuation, medical response, and warnings.

This test is also sometimes considered a "parallel" test. Parallel tests indicate that both the DR site and the production site are processing transactions, which results in heightened risk. 

### Full-Interruption Test

The entire organization takes part in an unscheduled, unannounced practice scenario, performing their full BCDR activities.

Provides the highest level of simulation, including notification and resource mobilization. A real-life emergency is simulated as closely as possible. It is important to properly plan this type of test to ensure that business operations are not negatively affected. This usually includes processing data and transactions using backup media at the recovery site. All employees must participate in this type of test, and all response teams must be involved.

:::info
As this could include system failover and facility evacuation, this test is the most useful for detecting shortcomings in the plan, but it has the greatest impact on productivity.
:::

## 8. Report

## 9. Revise