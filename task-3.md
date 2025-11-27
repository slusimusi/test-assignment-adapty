# Task 3

    Name (and explain) three things you would improve in our documentation. It can be anything – quickstarts, design, structure, specific guides or sections.

## Inconstistency

In the [Migration guide to server-side API v2](https://adapty.io/docs/migration-guide-to-server-side-API-v2), I notice that step descriptions contain at least 4 different structures.

The first structure (2 paragraphs, special mention of version 1, general mention of version 2 without its number, mix of passive and active voices):

    In version 1, you used to use:
    - Prolong/Grant a Subscription for a User request: to record a transaction and grant or shorten access level.
    - Revoke access level request: to immediately revoke access.
        
    They are now replaced with three separate requests to distinguish between adding transactions and managing access levels:

The second structure (1 paragraph with 2 sentences, special mention of version 1, general mention of version 2 without its number, mix of passive and active voices):

    In version 1, the Prolong/grant a subscription for a user request was used to grant access. Now you can grant access with the Grant access level request without providing transaction details.    

The third structure (2 paragraphs, special mentions of versions 1 and 2, passive voice in both paragraphs):

    In version 1, transactions were recorded using the Prolong/Grant a Subscription for a User request, which was limited to subscription transactions.
    
    In version 2, this functionality has been replaced by the Set Transaction request. This request can handle both subscription transactions and one-time purchases.

The fourth structure (1 paragraph with 2 sentences, special mentions of versions 1 and 2, active voice in both sentences):

    In version 1, you could only update user attributes. With version 2, you can modify a wider range of profile fields, such as installation metadata or analytics settings.
 
Also, some steps have no similar descriptions. It's applicable for Step 3 and Step 5.

So, these descriptions are inconsistent. 

Consistency is one of the essential pillars in technical writing. Different structures can distract users.


## Repeated block

In the [API reference](https://adapty.io/docs/api-adapty#/), I notice that the same block about API Key Security repeated in all sections. 

![An example of API Key Security](/img/API%20Key%20Security%20block.png "An example of API Key Security")

It's necessary to create a separate page with this description and to use it further. This page would be a single source of truth for developers. Additionally, technical writers can easily update only one page.

## Images without descriptions

In the documentation, I notice that all images don't contain any descriptions. For example, in [Introduction](https://adapty.io/docs/getting-started-with-server-side-api), the image has neither main nor alternative descriptions. 

The main description is necessary for context.
![An example of the image without the main description](/img/Image%20without%20main%20desciption.png "An example of the picture without the main description")

The alternative text is necessary for accessibility.
![An example of the picture without the alternative text](/img/Image%20without%20alt.png "An example of the image without the alternative text")

## Wrong usage of different list style

In the documentation, I notice numbered lists where they shouldn't be. For example, in [Introduction](https://adapty.io/docs/getting-started-with-server-side-api), a numbered list is used, although it is a feature list without any sequence of actions.

    With the API, you can:

    1. Check a user's subscription status.
    2. Activate a user's subscription with an access level.
    3. Retrieve user attributes.
    4. Set user attributes.
    5. Get and update paywall configurations.

Also, it's actual for the numbered list from the [article](https://adapty.io/docs/export-analytics-api) about exporting analytics with API:
    With the analytics export API, you can, for example:

    1. Analyze MRR from Marketing Campaigns: Measure the impact of last year's marketing campaigns in a specific country to see which ones brought in the highest revenue, with weekly tracking. Use the Retrieve analytics data method for this.

    2. Track Cohort Retention Over Time: Follow retention by cohort to spot drop-off points and compare cohorts over time, revealing trends and key moments where engagement strategies could boost retention. Limited to a specific app store, a specific country, and a particular product. Use the Retrieve cohort data method for this.

    3. Evaluate Conversion Rates Across Channels: Analyze conversion rates for key acquisition channels to see which are most effective in driving first-time purchases. This helps prioritize marketing spending on high-performing channels. Use the Retrieve conversion data method for this.

    4. Review Churn Rate: Monitor how quickly users are unsubscribing to uncover churn patterns or gauge the success of retention efforts, focusing on a specific country and a specific product. Use the Retrieve funnel data method for this.

    5. Assess LTV by User Segment: Identify the lifetime value of different user segments to understand which groups bring in the highest revenue over time. Focus on high-value segments like long-term subscribers, and use the results to refine acquisition strategies. Use the Retrieve LTV data method for this.

    6. Check Retention by Country: Look at retention rates by region to find high-engagement markets and guide localization or regional strategies. Use the Retrieve retention data method for this.

