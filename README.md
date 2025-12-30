# aws-architectures

# AWS Architecture Diagrams

This repository contains simple AWS architecture diagrams demonstrating cloud fundamentals, security best practices, and operational thinking.

## Static Website Hosting on AWS

![Static Website Architecture](diagrams/static-website-architecture.png)

**Purpose**  
Host a static website with low cost, high availability, and global performance.

**Key services**  
Amazon S3 stores static files. CloudFront provides HTTPS and caching. Route 53 manages DNS. Access to S3 is restricted using CloudFront Origin Access Control (OAC) and an S3 bucket policy.

**Trade-off**  
This design does not support server-side logic but keeps operational complexity very low.
