---
title: Runtime exceptions
description: Learn about how to work with runtime exceptions in code
keywords: Contributing
author: einari
weight: 7
---
The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”,
“RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be interpreted as described in
[RFC 2119](https://tools.ietf.org/html/rfc2119).

Exceptions should not be considered a way to do program flow. Exceptions should be treated as an exceptional state of the system
often caused by faulty infrastructure. At times there are exceptions that are valid due to developers not using an API right.
As long as it there is no way to recover an exception is fine. You should not throw an exception and let a caller of your API
deal with the recovery of an exception. Exceptions **MUST** be considered unrecoverable.

Naming of exceptions is covered by the [C# Coding Styles](csharp_coding_styles).