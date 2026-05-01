## Chapter 1: What is platform engineering?

- Platform engineering builds internal software systems that give developers self-service access to infrastructure, security tools, and deployment capabilities.

- Effective platforms reduce toil, delays, learning curve, and mental overhead across the software development lifecycle.

## 1.3.1 Product Delivery Model for Platforms

- Platform teams are software engineering teams that deliver internal products to users and stakeholders across the organization.

- Platform engineering requires a product mindset; otherwise, it is just productivity automation rather than a strategic platform capability.

- Treat the internal platform like a real product, not just infrastructure or tooling.

- Platform success depends on focusing on developer experience and developer needs.

- Old corporate IT models were too command-and-control; modern platforms need product thinking.

- Developer needs change over time, so the platform roadmap should evolve from user feedback.

- Product management decides what capabilities matter; engineering principles guide how they are delivered.

- As platforms scale, organize work into product domains so complexity does not hurt quality.

## 1.3.2 Platform Product Domains

- Engineering platform development should follow domain-driven design principles so platform responsibilities are organized around clear product domains.

- Domain-driven design gives platform teams a way to split the platform into clear product areas that can evolve independently.

- Good platform domains help different teams work on separate parts of the platform while keeping the developer experience smooth.

- Domain boundaries should be based on real product/user experience boundaries, not traditional IT functions.

- Teams organized around real domains can own their own backlog, priorities, and delivery responsibilities.

- Domains may still depend on each other, but coordination should mainly happen between product owners and domain architects, not every individual engineer.

- Frequent cross-team communication can be a warning sign that the domain boundaries are wrong or too tightly coupled.

- Platform domain boundaries should be measured and adjusted over time because the first logical split may not be the right one.

- A mature engineering platform can be modeled as several internal product domains with dependency ordering between them.

- Platform domains can have subdomains, but each boundary should stay self-serve, loosely coupled, and low friction.

- Low-friction boundaries do not happen automatically; they must be intentionally designed and maintained.

- The same domain model works for cloud or private data center platforms; “cloud” is just the common context.

- Eight platform domains do not require eight teams; start with the domain model, then add teams only when user demand and business value justify it.

- Some domains depend on others and must be built first, but each domain should gain autonomy once its dependencies exist.

## 1.3.3 Platform Engineering Principles

- Product delivery models and product domains organize the platform at the team and process level.

- Engineering principles shape how every platform capability or feature should be built and delivered.

- “Software-defined” is the core principle because platform capabilities should be managed through software, not manual process.

- The surrounding principles are connected: self-serve, evolutionary architecture, metrics-driven success, secure and compliant, automated governance, and observable.

- Each principle can support or undermine the others, so platform decisions should be evaluated across all of them.

- A self-serve feature without usage data is incomplete because the team cannot measure adoption or impact.

- A compliance requirement handled manually is weaker than one enforced through automation.

- A platform engineering team is a software team, so every platform capability should be deployable from versioned source control through CI/CD.

- Self-service starts with API-first design; the API is the foundation interface, and UIs or developer tools are built on top of it.

- API-first architecture makes self-service more sustainable and creates clearer boundaries between platform teams.

- Evolutionary architecture assumes platform decisions will change, so designs should support small, fast, incremental changes.

- Platform features must be measured against the value they promise, not just their technical health.

- Metrics should be measured across the whole delivery process because improving one team’s workflow can accidentally slow down another team.

- Security and compliance are shared responsibilities: the platform team secures the platform, while developers remain responsible for application security within it.

- The platform should provide tools that help developers detect vulnerabilities and assess the security of their own code.

- Platform resiliency is a security concern because failures should not cause data loss or prolonged service disruption.

- Availability is about routing traffic to healthy infrastructure; resiliency is about a system’s ability to self-correct after failure.

- Automated governance lets teams stay autonomous without making security, compliance, or governance teams a delivery bottleneck.

- Compliance should be made seamless for developers while still giving governance stakeholders proof that required controls happened.

- Separate doing compliant work from verifying compliant work; developers use self-service tools, while the platform control plane verifies compliance.

- Compliance at the point of change means the platform confirms compliance before a change is made.

- Monitoring tracks known health indicators, while observability helps understand the full system state and discover unexpected problems.

- Monitoring is a subset of observability focused on predictable issues.

- True observability connects technical data across applications, infrastructure, cloud services, incidents, and services to business outcomes and user experience.

## 1.4.1 Developer Experience

- Developer experience is the main customer outcome the platform product strategy is designed to improve.

- DevEx overlaps with platform features, so unclear boundaries can cause DevEx teams and platform teams to conflict.

- DevEx can be treated as a platform product services subdomain focused on tools and resources that improve developer speed, consistency, and software quality.

## 1.4.2 DevOps

- DevOps is most effective as a culture that combines development and operations, not as a separate team or job title.

- The same developers who design, build, and test software should also be responsible for deploying, monitoring, and supporting it.

- Platform engineers who build platform capabilities should also run, monitor, and support those capabilities in production.

## 1.4.3 SRE

- SRE should act as a reliability improvement discipline, not another operational silo.

- SREs should temporarily support mature product teams, helping improve their workflows and then carrying those learnings back into the platform.

- If an SRE team owns its own separate codebase, that can be a smell; SREs should usually contribute to the product team’s code while assigned there.

## 1.4.4 Impact of Generative AI in the Platform Engineering Space

- Generative AI can support platform strategy improvement across planning, design, testing, automation, and prediction.

- Generative AI can help platform engineers accelerate repetitive work, analyze observability data, and experiment with architecture faster.

- AI can identify patterns in observability data that may reveal current service disruptions or potential future problems.

- AI can produce convincing but wrong answers, so it must be used by people capable of doing the task without AI.

- AI is most useful as a productivity tool for skilled practitioners, not as a replacement for engineering judgment.
