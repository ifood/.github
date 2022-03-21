# Security Policy

Before a project be opened inside the iFood Open Source community, the internal security team scans the code to identify possible existent vulnerabilities, that need to be corrected until the launch. With the security team giving the "OK", the project will be published in iFood GitHub without the previous git history, to prevent exposed keys.

All new source code received by pull request will be scanned by a security pipeline that will detect vulnerabilities, sensitive data, exposed secrets, vulnerable dependencies, etc.. All issues identified by the pipeline need to be solved to be able to merge.

The project also will be followed by a security champion during all your life cycle, that will be a support for security reports analysis, and a required pull request reviewer.

## Reporting a Vulnerability

We're extremely grateful for all that report vulnerabilities to the iFood Open Source Community. All reports are thoroughly investigated by a set of community volunteers.

To make a report, email your vulnerability to oss-security@ifood.com.br. This allows triage and handling of the vulnerability with standardized response times.

# Development

Security is one of the most important checks performed within the code, and it is a required step for any code that is included in the project. 

## Shifting security left

A good preventive practice is to bring the security checks to the start of the development pipeline, to find vulnerabilities and security issues during the planning and coding phases. The goal is to ensure that the codebase is designed to be secure from the start with rapid feedback, rather than checking for security issues at the end of the process.

It can be done with some practices, like planning all security requirements along with functionalities, using tools during the coding process directly in the developer machine, that can be integrated with the IDE or not, and writing tests to prevent software misuse.

## Security Pipeline

All iFood projects needs to run to all pull requests a security pipeline that statically scans for vulnerabilities, scans secrets, and vulnerabilities in dependencies. For security reasons, it is not automatically executed on every pull request change, and needs an approval from the project maintainer. If the maintainer understands that the security pipeline can be skipped, he can request the merge to the project owner, that is the only one that has this permission.

Besides this validation, the project use the snyk GitHub app, that will check some vulnerabilitie, and a manual review done by an iFood internal security champion, and it's a required reviewer, and is required to prevent security issues that cannot be caught by automated tools, and give all project users and maintainers a guarantee that the project is safe to use.