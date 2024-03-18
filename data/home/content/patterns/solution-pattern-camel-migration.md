+++
author = "Michael Thirion(Red Hat)"
title = "Fuse to Apache Camel migration"
date = "2019-03-05"
description = "An accelerated path to migrating applications from Red Hat Fuse to Red Hat Build of Apache Camel based on templates."
tags = [
    "3scale", "apis"
]
categories = [
    "themes",
    "syntax",
]
series = ["Cloud Native Applications"]
patternurl = "https://redhat-solution-patterns.github.io/solution-pattern-camel-migration"
+++


An accelerated path to migrating applications from Red Hat Fuse to Red Hat Build of Apache Camel based on templates.

<!--more-->

Application Development is evolving as the modern Hybrid Cloud and cloud-native architectures drive new demands on applications. As a part of this continual evolution, we are evolving our product offering from Red Hat Fuse to the Red Hat build of Apache Camel, allowing us to address a broader set of customer deployment use cases.

As Red Hat Fuse approaches product End of Life (EOL) on June 30, 2024, Red Hat build of Apache Camel is the natural go-forward solution for integrations built around Red Hat Fuse which is based on an older version of Apache Camel. Fuse will remain in the maintenance life cycle until its EOL.

The Red Hat build of Apache Camel is the evolution for Red Hat Fuse, and is a powerful, versatile framework for application integration. It also includes running Camel on Quarkus and Spring Boot runtimes in both on-premise and cloud environments, including the Camel K operator which streamlines building, deploying and operating Camel integrations on OpenShift.

Performing such a migration can be scary as the effort is not just limited to migrating the high level Camel routes. Indeed, many other underlying technical components (JDK version, Runtime type, XML format etc.) are involved in the migration.

With this solution pattern you will find a guided way to perform Apache Camel v2 to Camel v3 and v4 migrations in a faster way. This solution pattern proposes an accelerated path to performing such a migration by abstracting all those technical details, leaving it to the migration of the high level integration logic .



Contributors: _Michael Thirion(Red Hat)_

Explore the Solution Pattern: https://redhat-solution-patterns.github.io/solution-pattern-camel-migration