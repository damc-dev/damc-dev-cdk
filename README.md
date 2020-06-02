# damc-dev-cdk

# Packages

## damc-dev-billing-alerts

Construct for creating alerts once AWS Billing Estimated Charges is greater then the configured threshold

```
  const app = new cdk.App();
  const stack = new cdk.Stack(app, "TestStack");

  // Creates an email alert to test@example.com that is triggered once the estimated charges is greater then 5 US Dollars
  new BillingAlert(stack, 'MyBillingAlert', {
    alarmThreshold: 5,
    emailSubscriptions: [
      'test@example.com'
    ]
  });
```

# Commands

Install package dependencies

```
yarn bootstrap
```

Build packages

```
yarn build
```

Test packages

```
yarn test
```