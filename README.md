Data Replication - Simplified Data Replication Mechanism
This README file provides an overview and instructions for setting up a simplified data replication mechanism for a distributed persistent cache using Kubernetes, Docker, and REST API for data manipulation.

Table of Contents
Introduction
Features
Prerequisites
Usage
Configuration
Introduction
Data replication is an essential concept in distributed systems, particularly when working with a distributed persistent cache. This project aims to provide a simplified and efficient data replication mechanism by leveraging Kubernetes for container orchestration, Docker for containerization, and REST API for manipulation of data between cache nodes.

Features
The simple and efficient data replication mechanism
Utilizes Kubernetes for container orchestration
Uses Docker for containerization of cache nodes
REST API for communication and manipulation of data between cache nodes
Automatic synchronization of data across distributed cache nodes
Prerequisites
Before setting up the data replication mechanism, ensure you have the following prerequisites:

Kubernetes cluster up and running
Docker installed on each node of the cluster
Basic knowledge of Kubernetes, Docker, and REST API concepts

Usage
Once the data replication mechanism is installed and running, you can interact with it using the REST API endpoints for data manipulation. Here are a few example requests:

GET /cache/{key}: Retrieves the value associated with the specified key from the cache.

POST /cache/{key}: Creates or updates a key-value pair in the cache.

DELETE /cache/{key}: Deletes the key-value pair associated with the specified key from the cache.
Configuration
The data replication mechanism can be customized by modifying the configuration files. Here's an overview of the main configuration files:

cache-node.yaml: Defines the Kubernetes deployment and service specifications for the cache nodes.

cache-config.yaml: Contains the configuration parameters for the cache nodes, such as cache size, replication factor, etc.
