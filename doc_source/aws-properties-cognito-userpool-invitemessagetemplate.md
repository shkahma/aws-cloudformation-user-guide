# AWS::Cognito::UserPool InviteMessageTemplate<a name="aws-properties-cognito-userpool-invitemessagetemplate"></a>

`InviteMessageTemplate` is a subproperty of the [AdminCreateUserConfig](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cognito-userpool-admincreateuserconfig.html) property that defines the email and SMS invitation message structure of an Amazon Cognito User Pool\.

See also [Customizing User Invitation Messages](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pool-settings-message-customizations.html#cognito-user-pool-settings-user-invitation-message-customization)\.

## Syntax<a name="aws-properties-cognito-userpool-invitemessagetemplate-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-cognito-userpool-invitemessagetemplate-syntax.json"></a>

```
{
  "[EmailMessage](#cfn-cognito-userpool-invitemessagetemplate-emailmessage)" : String,
  "[EmailSubject](#cfn-cognito-userpool-invitemessagetemplate-emailsubject)" : String,
  "[SMSMessage](#cfn-cognito-userpool-invitemessagetemplate-smsmessage)" : String
}
```

### YAML<a name="aws-properties-cognito-userpool-invitemessagetemplate-syntax.yaml"></a>

```
  [EmailMessage](#cfn-cognito-userpool-invitemessagetemplate-emailmessage): String
  [EmailSubject](#cfn-cognito-userpool-invitemessagetemplate-emailsubject): String
  [SMSMessage](#cfn-cognito-userpool-invitemessagetemplate-smsmessage): String
```

## Properties<a name="aws-properties-cognito-userpool-invitemessagetemplate-properties"></a>

`EmailMessage`  <a name="cfn-cognito-userpool-invitemessagetemplate-emailmessage"></a>
The message template for email messages\.  
*Required*: No  
*Type*: String  
*Minimum*: `6`  
*Maximum*: `20000`  
*Pattern*: `[\p{L}\p{M}\p{S}\p{N}\p{P}\s*]*\{####\}[\p{L}\p{M}\p{S}\p{N}\p{P}\s*]*`  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`EmailSubject`  <a name="cfn-cognito-userpool-invitemessagetemplate-emailsubject"></a>
The subject line for email messages\.  
*Required*: No  
*Type*: String  
*Minimum*: `1`  
*Maximum*: `140`  
*Pattern*: `[\p{L}\p{M}\p{S}\p{N}\p{P}\s]+`  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`SMSMessage`  <a name="cfn-cognito-userpool-invitemessagetemplate-smsmessage"></a>
The message template for SMS messages\.  
*Required*: No  
*Type*: String  
*Minimum*: `6`  
*Maximum*: `140`  
*Pattern*: `.*\{####\}.*`  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)