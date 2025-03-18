---
title: "Data Flow"
weight: 30
bookFlatSection: true
---

# Data Flow

Sleep App organizes Kubernetes resources in a hierarchical structure:

```
Project
└── Subservice
   └── Resources (Deployment & StatefulSet)
```

## Example Structure

```
chatbot
└── english
   └── rasa-worker-en
   └── rasa-webserver-en
   └── rasa-mysql-en
└── indonesia
   └── rasa-worker-id
   └── rasa-webserver-id
   └── rasa-mysql-id
ai
└── milvus
   └── milvus-postgresql
   └── milvus-webserver
   mindsdb
   └── mindsdb-postgresql
   └── mindsdb-webserver
sleep-app
└── sleep-app-no-subservice
   └── sleep-app
```