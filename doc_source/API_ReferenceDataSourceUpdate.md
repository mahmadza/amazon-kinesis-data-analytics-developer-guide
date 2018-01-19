# ReferenceDataSourceUpdate<a name="API_ReferenceDataSourceUpdate"></a>

When you update a reference data source configuration for an application, this object provides all the updated values \(such as the source bucket name and object key name\), the in\-application table name that is created, and updated mapping information that maps the data in the Amazon S3 object to the in\-application reference table that is created\.

## Contents<a name="API_ReferenceDataSourceUpdate_Contents"></a>

 **ReferenceId**   
ID of the reference data source being updated\. You can use the [DescribeApplication](API_DescribeApplication.md) operation to get this value\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 50\.  
Pattern: `[a-zA-Z0-9_.-]+`   
Required: Yes

 **ReferenceSchemaUpdate**   
Describes the format of the data in the streaming source, and how each data element maps to corresponding columns created in the in\-application stream\.   
Type: [SourceSchema](API_SourceSchema.md) object  
Required: No

 **S3ReferenceDataSourceUpdate**   
Describes the S3 bucket name, object key name, and IAM role that Amazon Kinesis Analytics can assume to read the Amazon S3 object on your behalf and populate the in\-application reference table\.  
Type: [S3ReferenceDataSourceUpdate](API_S3ReferenceDataSourceUpdate.md) object  
Required: No

 **TableNameUpdate**   
In\-application table name that is created by this update\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 32\.  
Pattern: `[a-zA-Z][a-zA-Z0-9_]+`   
Required: No

## See Also<a name="API_ReferenceDataSourceUpdate_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:

+  [AWS SDK for C\+\+](http://docs.aws.amazon.com/goto/SdkForCpp/kinesisanalytics-2015-08-14/ReferenceDataSourceUpdate) 

+  [AWS SDK for Go](http://docs.aws.amazon.com/goto/SdkForGoV1/kinesisanalytics-2015-08-14/ReferenceDataSourceUpdate) 

+  [AWS SDK for Java](http://docs.aws.amazon.com/goto/SdkForJava/kinesisanalytics-2015-08-14/ReferenceDataSourceUpdate) 

+  [AWS SDK for Ruby V2](http://docs.aws.amazon.com/goto/SdkForRubyV2/kinesisanalytics-2015-08-14/ReferenceDataSourceUpdate) 