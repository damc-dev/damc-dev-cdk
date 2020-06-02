# damc-dev-cdk

A monorepo project managed with lerna that builds and publishs CDK construct libraries for multiple languages using JSII

## Packages

### damc-dev-billing-alerts

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

## Build 

Run the following commands from the project root and they will use lerna to run against all packages

### Commands

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
<<<<<<< HEAD

## Contributing

Fork the repository

Make changes

Ensure all tests are passing

```
yarn test
```

Commit changes

```
npx git-cz
```

Create a Github Pull Request

=======
>>>>>>> d5b71daad8aac3b12ceb950ee5481ce7d8ee44d0
