---
title: "How to Use"
weight: 40
bookFlatSection: true
---

# How to Use

## Adding a Service

To add a service, modify your `Deployment/StatefulSet` configuration by adding labels:

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  labels:
    project: infra          # Add Project
    subservice: exporter    # Add Subservice (Optional)
  name: apz-exporter
```

## Main Functions

- **Activate services** for a set period of time
- **Put services to sleep** manually
- **Enable auto sleep** to automatically manage resources
- **Exclude services** from management
- **Hard refresh** to sync with Kubernetes

## Comparison

Sleep App is simpler than K9S and Kubectl while providing specialized functionality for resource management.