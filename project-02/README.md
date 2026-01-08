# Flagship Project 02 — Containerized Application Platform (ECS/EKS)

## Overview

This project demonstrates a production-grade containerized application platform on AWS,
designed to showcase scalable service deployment, secure image management, and operational
best practices using managed container services.

## Problem Statement

Many organizations struggle to deploy and operate containerized applications in a way
that is scalable, secure, and operationally manageable.

This project addresses that challenge by demonstrating a managed AWS container platform
that supports consistent deployments, secure container images, and controlled scaling
without managing underlying infrastructure.

## High-Level Architecture

1. A containerized application image is built and stored securely.
2. The image is hosted in Amazon Elastic Container Registry (ECR).
3. The application is deployed using a managed container service.
4. Traffic is routed to running containers through a load balancer.
5. Logs and metrics are collected for monitoring and operations.

## AWS Services Used

- Docker
- Amazon Elastic Container Registry (ECR)
- Amazon ECS or Amazon EKS
- Application Load Balancer
- AWS IAM
- Amazon CloudWatch

## Key Design Decisions

- Use of managed container services to reduce operational overhead
- Centralized container image management with ECR
- Secure access control using IAM roles
- Scalable traffic handling through a load balancer
- Centralized logging and monitoring with CloudWatch

## Architecture Components

- User
- Application Load Balancer
- Container Service (Amazon ECS or Amazon EKS)
- Amazon Elastic Container Registry (ECR)
- Amazon CloudWatch

## Request Flow

1. A user sends a request to the application endpoint.
2. The Application Load Balancer receives the request.
3. Traffic is routed to running containers.
4. Containers retrieve images from ECR during deployment.
5. Logs and metrics are sent to CloudWatch.

![Architecture Diagram](architecture/diagram.png)
