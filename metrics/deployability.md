# Deployability
Ability system to be deployed and maintained by a DevOps team. A good example is continues delivery.

###Deployment frequency
In Accelerate, the authors state “Therefore, we settled on deployment frequency as a proxy for batch size since it is
easy to measure and typically has low variability. By “deployment” we mean a software deployment to production or
to an app store.” The reason the frequency of production deployments matters is because it tells you how often you’re
delivering something of value to end users and/or getting feedback from users.
 
The other essential point with any of these metrics is that they are all based on production.
Not staging, or “what we’d intended to deploy to production”: only production.
Production is the only thing that matters because it’s only in production that value can be realized.
The value usually comes in the form of revenue, feedback, or a combination of both.

With an AWS-native approach we can obtain this number by getting the time at which CodePipeline successfully
completes its last action in the pipeline and track how many times per time period deployments to production are occurring.

According to the DORA 2018 Report, Elite performers have a deployment frequency of multiple times per day and Low
performers have a deployment frequency that is between 1 week and 1 month.

### Lead time for changes
In the book, they describe lead time for change as “the time it takes to go from code committed to code successfully
running in production”. 

You can obtain this metric by capturing the time at which each revision was initiated in CodePipeline and then updating
the row with the time at which that same revision successfully runs the last action of the deployment pipeline.
By comparing these numbers, you get the lead time for changes. By averaging these numbers over a period of time,
you obtain the mean time lead for changes to production.

According to the DORA 2018 Report, Elite performers have a lead time for changes of less than 1 hour and
Low performers have a lead time for changes that is between 1 month and 6 months.

### Time to restore service
The time to restore service or mean time to recover (MTTR) metric calculates the average time it takes to restore service.

One way of instrumenting this data in an AWS-native world is to run automated synthetic tests in production that test
key scenarios in production. If there are any failures, we capture the time at which the failure was discovered and
enter it as a row in a database – such as DynamoDB – and then update that row once our synthetic tests begin reporting
success again. This information can be reported back to CodePipeline so that we know when a failure occurs and what kind
of test produced this failure.

According to the DORA 2018 Report, Elite performers have an MTTR that is less than 1 hour and Low performers have an
MTTR that is between 1 week and 1 month.

### Change failure rate
The change failure rate is a measure of how often deployment failures occur in production that require immediate remedy
(particularity, rollbacks).

To obtain this information in an AWS-native manner, you track each deployment and indicate whether it was successful or
not. Then, you track the ratio of successful to unsuccessful deployments to production over time.

According to the DORA 2018 Report, Elite performers have a change failure rate between 0-15% and Low performers have a
rate from 46-60%.  

### Continuous Improvement
While we have captured some of these and other metrics with some of our customers, we’ve not acquired them in a
consistent manner over the years. We even open sourced a CloudWatch Dashboard for deployment pipelines that use
CodePipeline that captures some of these metrics along with some others. It’s called pipeline-dashboard.

A way to obtain these metrics is through brief surveys and by instrumenting the deployment pipelines for certain
applications/services. This way you can ensure teams are seeing improvements and, if they are not, identify ways to
remedy this. Then, you might anonymize this data and make it available across an enterprise.
This helps ensure you are accelerating the speed and confidence of feedback between end users and developers.

# Metrics

- Deployment downtime: secs/mins
- Deployment frequency: High(Between once per hour and once per day)/
  Medium(Between once per week and once per month)/
  Low(Between once per week and once per month)
- Lead time for changes: High(Between one day and one week)/Medium(Between one week and once month)/
  Low(Between one month and 6 months)
- Time to restore service:  High(Less than one day)/Medium(Less than one day)/Low(Between one week and one month)
- Change failure rate: %
- Continuous Improvement