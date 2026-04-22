# Ceiba

Ceiba is a lightweight API access and monetization layer for modern APIs.

It sits in front of your APIs to enforce access, limits, and usage.

More at: https://useceiba.com

Ceiba helps developers protect endpoints, issue and manage access keys, enforce limits, track usage, and monetize API access without building the full access stack from scratch. It is part of the production-inspired Aluna-Platform designed to explore infrastructure, observability, and workload operations.

This repository contains the product source code for 

Ceiba is not just an API key generator.

It is an API access layer with three main responsibilities:

control access to protected endpoints
enforce plans, policies, limits, and usage rules
make API monetization easier for developers and startups


Product surfaces

1. Control plane
Human-facing dashboard and management UI.

creating projects
viewing and managing keys
viewing usage summaries
defining policies
selecting or upgrading plans


2. Runtime
Machine-facing authorization and enforcement service.

validating presented access keys
checking project entitlements
enforcing policies
enforcing rate limits
recording usage


3. SDK
Developer integration surface.

drop-in Express middleware
drop-in Fastify integration
programmatic key lifecycle management
calling runtime safely from customer backends


Core principle
A developer should be able to protect an endpoint and integrate the product in minutes.

Project secret
Server-side credential used by the customer backend / SDK to call Aletheos runtime and management APIs.