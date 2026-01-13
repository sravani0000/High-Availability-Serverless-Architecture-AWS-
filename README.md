Overview
Designed and implemented a cloud-native, serverless data ingestion system on AWS. The architecture focuses on the two most critical pillars of the AWS Well-Architected Framework: Reliability and Cost Optimization. By utilizing event-driven compute and managed storage, the system achieves high availability with minimal operational overhead.

Technical Stack
Compute: AWS Lambda (Event-driven, serverless functions)

Storage: Amazon S3 (Durable object storage)

API Management: AWS API Gateway (Secure entry points)

Strategy: Multi-AZ (Availability Zone) Deployment

Cloud Engineering Highlights
Fault-Tolerant Design: Implemented Multi-AZ deployment strategies to ensure the pipeline remains operational even in the event of a localized data center failure, targeting 99.9% uptime.

Event-Driven ETL: Configured S3 Event Notifications to trigger AWS Lambda functions for real-time data processing, eliminating the need for idle server resources.

Infrastructure Cost Reduction: Achieved a 40% reduction in infrastructure overhead by migrating from traditional EC2-based polling instances to a fully serverless architecture.

Security & Gatekeeping: Utilized AWS API Gateway to establish secure, throttled endpoints for data ingestion, protecting downstream resources from traffic spikes.

Key Lessons Learned
Successfully addressed cross-AZ latency challenges to ensure data consistency.

Managed cost-effectively by implementing S3 lifecycle policies and monitoring Lambda execution times.

Simplified environment configuration through the principles of Infrastructure as Code (IaC).
