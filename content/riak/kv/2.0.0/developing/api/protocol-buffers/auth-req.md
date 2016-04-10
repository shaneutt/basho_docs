---
title: "PBC Auth Request"
description: ""
project: "riak_kv"
project_version: "2.0.0"
menu:
  riak_kv-2.0.0:
    name: "Auth Request"
    identifier: "pbc_auth_request"
    weight: 125
    parent: "apis_pbc"
toc: true
aliases:
  - /riak/2.1.3/dev/references/protocol-buffers/auth-req
canonical_link: "docs.basho.com/riak/kv/latest/developing/api/protocol-buffers/auth-req.md"
---

Sends a username (`user`) and password (`password`) to Riak as part of
an authentication request. Both values are sent as binaries.

## Request

```protobuf
message RpbAuthReq {
    required bytes user = 1;
    required bytes password = 2;
}
```

For more on authentication, see our documentation on [Authentication and Authorization](/riak/kv/2.0.0/using/security/basics).