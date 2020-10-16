# Go Micro与 Micro分别是什么?

### Micro - a microservices toolkit

Micro是一个微服务工具工具包. 它提供了编写和管控微服务的基础构建块.它由一系列的库和工具组成. 这些库和工具主要面向Golang. 当然Micro也提供了proxy\(曾经为sidecar, 详情见👉[issue](https://github.com/micro/micro/issues/283)\)通过http与其他语言通信.

### Go Micro - A pluggable RPC base library

Go Micro 是一个插件化的基础RPC的库. 它为GO提供了编写微服务的基础构建块. Micro的哲学是包含电池的可拔插架构. 

Go Micro可拔插性体现在提供了一系列基于Go的接口, 这些接口一起提供了编写微服务的构建块. 这些接口可以通过具体实现来满足. 例如Registry接口, 它默认提供了基于MDNS的服务发现的实现, 但是可以被替换成用于etcd, consul, nats等任何满足Registry接口的实现.

可拔插的架构意味着你可以不需要重写代码就可以替换底层实现.





