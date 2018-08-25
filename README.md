# LambdaMessenger iOS

LambdaMessenger is a chat app that works with the [LambdaMessenger API](https://github.com/JohnRbk/lambda-messenger-api). It features realtime updates using AppSync subscriptions.

## Getting Started

1. Follow the instructions for the [LambdaMessenger API](https://github.com/JohnRbk/lambda-messenger-api) to configure FireBase, AWS AppSync, and deploy the API services for LambdaMessenger.
2. Follow the [FirebaseAuth](https://firebase.google.com/docs/auth/ios/phone-auth?authuser=0) instructions for enabling SMS notifications and for generating a GoogleService-Info.plist file.
3. Run Carthage to download project dependencies
4. Because AWS AppSync does not support Carthage, you need to download that separetely. Additionally, a quirk with the AWS AppSync SDK makes it difficult to use it with OpenID tokens. As a workaround, navigate to the `LambdaMessenger/Frameworks` directory and `git clone https://github.com/JohnRbk/aws-mobile-appsync-sdk-ios` a copy of a patched AWS AppSync SDK. See this [pull request](https://github.com/awslabs/aws-mobile-appsync-sdk-ios/pull/53) for more details.

## Built With

* [AWS AppSync](https://docs.aws.amazon.com/appsync)
* [AWS Lambda](https://aws.amazon.com/documentation/lambda/)
* [AWS DynamoDB](https://aws.amazon.com/documentation/dynamodb/)
* [Firebase](https://firebase.google.com/)
* [Feather Icons](https://feathericons.com/)

## Authors

* John Robokos

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details
