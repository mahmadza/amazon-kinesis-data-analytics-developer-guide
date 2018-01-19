# ReferenceDataSource<a name="API_ReferenceDataSource"></a>

Describes the reference data source by providing the source information \(S3 bucket name and object key name\), the resulting in\-application table name that is created, and the necessary schema to map the data elements in the Amazon S3 object to the in\-application table\.

## Contents<a name="API_ReferenceDataSource_Contents"></a>

 **ReferenceSchema**   
Describes the format of the data in the streaming source, and how each data element maps to corresponding columns created in the in\-application stream\.  
Type: [SourceSchema](API_SourceSchema.md) object  
Required: Yes

 **S3ReferenceDataSource**   
Identifies the S3 bucket and object that contains the reference data\. Also identifies the IAM role Amazon Kinesis Analytics can assume to read this object on your behalf\. An Amazon Kinesis Analytics application loads reference data only once\. If the data changes, you call the [UpdateApplication](API_UpdateApplication.md) operation to trigger reloading of data into your application\.   
Type: [S3ReferenceDataSource](API_S3ReferenceDataSource.md) object  
Required: No

 **TableName**   
Name of the in\-application table to create\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 32\.  
Pattern: `[a-zA-Z][a-zA-Z0-9_]+`   
Required: Yes

## See Also<a name="API_ReferenceDataSource_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:

+  [AWS SDK for C\+\+](http://docs.aws.amazon.com/goto/SdkForCpp/kinesisanalytics-2015-08-14/ReferenceDataSource) 

+  [AWS SDK for Go](http://docs.aws.amazon.com/goto/SdkForGoV1/kinesisanalytics-2015-08-14/ReferenceDataSource) 

+  [AWS SDK for Java](http://docs.aws.amazon.com/goto/SdkForJava/kinesisanalytics-2015-08-14/ReferenceDataSource) 

+  [AWS SDK for Ruby V2](http://docs.aws.amazon.com/goto/SdkForRubyV2/kinesisanalytics-2015-08-14/ReferenceDataSource) 