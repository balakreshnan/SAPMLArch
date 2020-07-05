# Business Data Lake Architecture

## Business Analytic Architecture

## Challenge

One of the biggest challenge for business are there are numerous business systems like SAP, Sales force, Oracle business systems and lot more. Most common is SAP and Sales force, but the idea here is build a data lake independant for any business systems, since it provide lot of value for business as their analytics is not coupled to a product. 

Also provide scalable and value based systems. The other challenge for machine learning/Deep learning are to able to use other external data sources like, Twitter, face book, or any social platforms with weather and economic data and other data providers data sources. Integrating this into SAP and sales force are challenging and time consuming process. Also it has to be conform to source systems schema and other restrictions the platform might have. For example text might be truncated, or date might be specfic format etc.

## Solution

To solve the above challenge we can take a different perspective look and see how we can achieve this. The architecture is not realtime but we can make this realtime. There are few challenges this architecture solves are

- Moving data out of SAP - Batch and Change data capture
- Moving data from legacy and other business Systems

Moving data from SAP and legacy systems are more cumbersome and time consuming and expensive. By using Kagool's Velocity we can move actual business data from ECC, BW and HANA and push that to Azure data lake store. For users who has SAP ECC it might be easy to move data out of ECC to Azure data lake instead HANA since it cost's a lot for HANA. 

Not only that SAP HANA systems doesn't provide Machine learning or deep learning platform choice like Azure Machine learning does. Azure Machine learning products provide access to python and R based programming and also allows us to use Tensorflow, pytorch and other open source programming lanugages while maintaining the data science life cycle across end to end.

![alt text](https://github.com/balakreshnan/SAPMLArch/blob/master/images/SAPMLbusinessarch.png "Business Architecture")