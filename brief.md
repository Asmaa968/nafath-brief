Version: NAFATH-V3
Your track: Software

## Overview
A government entity aims to launch an application that allows individuals to interact with artificial intelligence (AI) to ask questions and obtain information about citizen services. This application relies on several interconnected fields. Software provides the foundation for developing and operating the application. AI analyzes information and generates relevant responses to users' inquiries. Mobile phones allow individuals to access the application and communicate with AI. Networks connect devices to the internet and enable data exchange. Cybersecurity protects the application, networks, and users' information from cyberattacks and unauthorized access. Finally, data consists of the information stored and processed by the application, which AI uses to provide accurate and useful answers while maintaining user privacy.

## Software

In the government application, Semantic Versioning (SemVer) helps manage updates to the public API. The MAJOR version increases when incompatible changes occur, such as removing an existing method for accessing citizen services. The MINOR version increases when new features are added, such as introducing a new government service, while maintaining backward compatibility. The PATCH version increases when bugs are fixed, such as correcting errors in AI responses, without affecting existing functionality. This approach ensures reliable updates and maintains service continuity for citizens.

Resource: [Semantic versioning and impact of breaking changes in the Maven repository] - [[Full URL](https://www.sciencedirect.com/science/article/abs/pii/S0164121216300243)]

## AI

Retrieval-Augmented Generation (RAG) combines information retrieval with large language models (LLMs) to generate accurate responses. It retrieves relevant information from external sources, such as databases and official documents, to help the AI generate answers. RAG reduces incorrect responses by grounding answers in reliable information rather than relying only on the model’s learned knowledge. In a government application, RAG can retrieve official service requirements to answer citizens’ questions accurately. However, its effectiveness depends on the quality of the retrieved information. 

Resource: [Retrieval-Augmented Generation for AI-Generated] - [[Full URL](https://link.springer.com/article/10.1007/s41019-025-00335-5)]

## Mobile

App Transport Security (ATS) in iOS enforces secure network connections by requiring HTTPS and appropriate Transport Layer Security (TLS) standards. It helps protect data transmitted between applications and servers from interception and unauthorized access. If an application attempts to connect to a regular HTTP endpoint, iOS blocks the connection by default unless an appropriate exception is configured. In the government application, ATS helps protect citizens’ personal information and inquiries during transmission, improving data security and ensuring safer communication between the application and government servers.

Resource: [Preventing Insecure Network Connections] - [[Full URL](https://developer.apple.com/documentation/security/preventing-insecure-network-connections)]

## Networking

IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses, providing a much larger address space. This is important as more smartphones and connected devices access online government services. IPv6 can support future growth by allowing more devices to connect without the same limitations of IPv4 address availability. Government applications should ensure their network infrastructure supports IPv6 correctly to maintain reliable connectivity as the number of users and connected devices increases. 
Resource: [A Comparison of Internet Protocol (IPv6) Security Guidelines] - [[Full URL](https://www.mdpi.com/1999-5903/6/1/1)]

## Cybersecurity

Prompt injection occurs when malicious instructions manipulate an AI assistant into ignoring its intended rules or producing unsafe responses. Direct injection comes from a user’s message, while indirect injection is hidden in external content, such as documents or webpages. For a government service assistant, risks can be reduced by separating untrusted content from system instructions and restricting the assistant’s access to sensitive data and privileged functions.

Resource: [A Systematic Review of Prompt Injection Attacks on Large Language Models: Trends, Taxonomy, Evaluation, Defenses, and Opportunities] - [[Full URL](https://ieeexplore.ieee.org/abstract/document/11359704)]

## Data

Anonymization removes identifying information so individuals can no longer reasonably be identified, while pseudonymization replaces personal identifiers with codes that can be linked back to a person using additional information. When storing government AI chat logs, anonymization can help protect citizens’ privacy. Under the GDPR, effectively anonymized data falls outside data protection law, whereas pseudonymized data remains personal data and must still comply with data protection requirements. 

Resource: [Introduction to anonymisation - Information Commissioner's Office] - [[Full URL](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/data-sharing/anonymisation/introduction-to-anonymisation/)]

## Misconception in My Track

A common misconception about Semantic Versioning is that every software update requires a MAJOR version increase. However, the version number depends on the type of change and its compatibility with the existing public API. Incompatible public API changes require a MAJOR version increase, new backward-compatible functionality requires a MINOR version increase, and backward-compatible bug fixes require a PATCH version increase. The official Semantic Versioning specification explains these rules in Sections 6, 7, and 8. Understanding these distinctions helps developers manage software updates and maintain compatibility.

## Open Question

How can developers determine whether a public API change is backward-compatible when deciding which Semantic Versioning number to increase?

