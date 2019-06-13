# Azure Load Testing Guide

## Summary

[Locust](https://docs.locust.io/en/stable/index.html) is a powerful load testing tool that can be deployed and distributed across a cluster, allowing you to configure your load test for your specific application. User test scenarios are written in python and can be used to test almost any system.

In order to load test your application, you must complete the following steps:
1. Follow the Bedrock steps to deploy an [azure-simple](https://github.com/microsoft/bedrock/tree/master/cluster/environments/azure-simple) cluster that will be your distributed Locust cluster.
2. Update the `locustfile.py` file in this directory to match your desired tests
3. Deploy a docker image to your registry
4. Update yaml files
5. Deploy locust yaml files
