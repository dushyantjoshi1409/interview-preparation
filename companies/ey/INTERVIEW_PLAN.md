# EY MLOps Engineer Interview Plan

Interview: September 16, 2026, 1:00 PM to 2:00 PM IST, unless the calendar invite says otherwise

Prepared for: Dushyant Joshi

Research date: September 15, 2026

## Read this first

This guide is based on two things:

1. The updated EY resume.
2. The recruiter's gap assessment, because the complete job description is not available.

Anything reconstructed from the assessment is labeled **likely** or **inferred**. It is not confirmed EY job-description text.

Your goal is not to pretend that every gap has disappeared. Your goal is to show that you already operate production AI services, understand the MLOps lifecycle, can reason about the infrastructure layer, and are honest about where your hands-on experience stops.

## Your best positioning in one sentence

> I am a production AI and MLOps-focused engineer who has owned Python services from data ingestion through deployment, monitoring, evaluation, troubleshooting, and cost analysis, and I now want to deepen that experience at the cloud infrastructure and platform level.

## What the role most likely is

### Inferred role profile, not a confirmed JD

The partial assessment points to a consultant-level EY MLOps Engineer role with these likely priorities:

| Area | Likely expectation | Confidence |
|---|---|---:|
| Core engineering | Strong Python and production service development | High |
| Cloud | AWS, Azure, or GCP experience, probably with AWS depth to verify | High |
| Delivery | CI/CD, containers, deployment, testing, troubleshooting | High |
| MLOps | Repeatable ML lifecycle, model deployment, versioning, evaluation, monitoring | High |
| Infrastructure | Scalable and reliable ML infrastructure ownership | High |
| Data | Processing workflows, validation, quality, SQL, distributed data concepts | High |
| Operations | Telemetry, alerts, incident diagnosis, reliability and cloud cost | High |
| Consulting | Client communication, cross-functional work, ownership and delivery | High |
| Beneficial tools | Kubernetes/EKS, EMR, Spark/Hadoop, IaC, model registry, Prometheus/Grafana | Medium to high |
| Experience | At least 3 years of infrastructure engineering | High, but inferred from recruiter assessment |

Do not say that EY confirmed every tool above. A safe phrase is:

> Based on the role discussion, I understand the main need is production MLOps and cloud infrastructure, with technologies such as Kubernetes, IaC, distributed processing, model lifecycle management, and infrastructure monitoring being useful.

## What to expect in this 60-minute round

EY says interview formats vary by role, location, experience level, and service line. Its official material says interviews may be behavioral, case based, or a combination, and that behavioral answers are judged on the relevance of the example, the action taken, and the result. Therefore, this is a preparation estimate, not a promised agenda.

### Likely agenda

| Time | Likely activity | Your objective |
|---:|---|---|
| 0-5 min | Greeting and introduction | Give a focused 60-90 second story |
| 5-15 min | Resume and project depth | Prove ownership with architecture, scale, metrics, and decisions |
| 15-35 min | MLOps, cloud, DevOps, data, monitoring | Explain fundamentals and trade-offs in simple language |
| 35-45 min | Architecture or troubleshooting scenario | Clarify, structure, prioritize safety, then propose a design |
| 45-53 min | Behavioral and consulting questions | Use concise STAR stories and show client awareness |
| 53-58 min | Coding, SQL, or rapid technical checks | Think aloud and test edge cases |
| 58-60 min | Your questions | Ask two strong questions |

EY's current official guidance encourages candidates to be authentic, prepare real stories, understand market trends, and treat the interview as a two-way conversation.

## The first five minutes

### 60-90 second introduction

> Hi, I am Dushyant Joshi. I work as a Generative AI and ML Engineer at Analyttica Datalab. My main strength is taking AI systems beyond a demo and operating them as production services. I build asynchronous Python services using FastAPI, package them with Docker, deploy on AWS, and add monitoring for latency, errors, token usage, cost, and model quality.
>
> One example is a production RAG pipeline and API integration router using LangChain, GPT-4o, and Pinecone. It worked across a corpus of more than 10,000 documents, achieved sub-200 millisecond retrieval, and was associated with a 70 percent increase in customer engagement. I also built cost analytics that showed 20 percent of workloads were consuming 60 percent of compute, which supported better model-routing and optimization decisions.
>
> My experience is strongest at the application and ML service layer. I am actively building deeper knowledge in Kubernetes, Terraform, Spark, Prometheus, and Grafana. This EY role interests me because it connects production ML engineering with cloud platform reliability, governance, and client outcomes.

Do not add years to this answer. If asked, state the exact employment dates.

### Why EY?

> EY interests me for three reasons. First, the work connects technology to real client outcomes, which matches how I like to work: understand the problem, build the system, measure it, and improve it. Second, EY publicly emphasizes building trust and long-term value, which is important in MLOps because a model is only useful when it is reliable, observable, secure, and explainable enough for production. Third, the role would let me contribute my production AI experience while developing deeper cloud and platform engineering skills with multidisciplinary teams.

EY's published values include integrity, respect, teaming, inclusiveness, courage to lead, and building relationships by doing the right thing. Mention only the parts that genuinely connect with you.

### Why MLOps?

> A model in a notebook is like a good engine sitting on a workbench. MLOps builds the car around it: testing, deployment, roads, dashboard, maintenance schedule, safety checks, and a way to replace the engine without stopping the whole service. I enjoy that full problem. I want the model to create reliable value after it reaches users, not only score well during experimentation.

### Why consulting?

> Consulting requires both engineering and translation. A client may say, "We need an AI solution," but the real need could be lower handling time, better accuracy, or stronger compliance. I like turning a broad problem into measurable requirements, explaining trade-offs clearly, and delivering in stages. My enterprise POC work has given me experience taking requirements through deployed, monitored systems. I want to strengthen that skill in a formal consulting environment.

## Resume-to-role match and gap map

| Likely requirement | Truthful resume evidence | Strength | Interview strategy |
|---|---|---|---|
| Strong Python | Python, async Python, FastAPI, and REST microservices; Django in the earlier software developer role | Strong | Explain one service end to end, including errors and tests |
| Cloud | AWS deployment | Relevant, depth needs clarification | Name only AWS services you truly used; distinguish use from ownership |
| Containers | Dockerized AI services | Strong | Explain image, configuration, health checks, and runtime concerns |
| CI/CD | Git and CI/CD exposure; evaluation gating in the Pro-RAG project | Relevant | Walk through a proposed pipeline; separate production work from project evidence |
| ML lifecycle | Production data pipelines, deployment, and monitoring; evaluation gating in the Pro-RAG project | Strong at AI application layer | Use the production RAG system as the main operational example |
| Scale | Production RAG across 10,000+ documents with sub-200ms retrieval; 10M-document Pro-RAG project design at 50 QPS | Strong evidence, but distinguish production from project | Say which numbers were production and which belong to a designed project |
| Model monitoring | OpenTelemetry, Langfuse, latency, errors, tokens, cost, quality | Strong for LLM systems | Explain operational vs data/model metrics |
| Troubleshooting | OpenTelemetry and Langfuse distributed tracing reduced troubleshooting time by 40% | Strong | Give one real incident only if you can describe it accurately |
| Cost optimization | 20% of workloads consumed 60% of compute; routing and optimization | Relevant | Do not call this AWS FinOps unless it actually was |
| Data quality | Pro-RAG project evidence: regression checks, prompt-injection detection, PII guardrails, and relevance/quality gates | Relevant project evidence | Explain schema, freshness, completeness, and semantic checks without calling the project production work |
| Collaboration | 5+ enterprise POCs from requirements through deployed, monitored systems | Relevant | Prepare stakeholder names by role, not confidential identity |
| Kubernetes/EKS | Resume says currently learning | Gap | Explain concepts, no production claim |
| Terraform/IaC | Resume says currently learning | Gap | Explain desired-state workflow, no hands-on production claim |
| Spark/EMR/Hadoop | Resume says currently learning Spark | Gap | Explain when distributed processing is justified |
| Prometheus/Grafana | Resume says currently learning | Gap | Bridge from OpenTelemetry and Langfuse distributed tracing |
| Model registry/feature store | No explicit resume evidence | Gap | Explain concepts and a proposed design, not experience |
| 3+ years infrastructure | Experience shown from Nov 2024 to present, about 22 months, with March 2025 as the shared transition month | Material gap | Give exact dates and scope; never claim 3+ years |

## Accuracy warnings before you rehearse

### Calendar experience mismatch

The resume summary says "2 years," while the listed roles run from November 2024 to the interview date, which is about 22 months. March 2025 is the shared transition month between the two roles, not evidence of a longer overlap. Be ready to explain the actual timeline cleanly.

Safe answer:

> My formal experience shown here begins in November 2024, which is about 22 months by the interview date, so I do not have three full years of infrastructure engineering. March 2025 is the transition month shared by the two role entries. I prefer to be exact about that. Within this period, I have had concentrated production ownership across Python services, AWS deployment, Docker, data pipelines, monitoring, troubleshooting, and cost controls. If the role needs someone who already has three years of dedicated platform ownership, I understand the gap. I can still contribute immediately at the production ML service layer and I am building the deeper platform skills deliberately.

If you have real internships, contracts, freelance work, or infrastructure responsibilities before November 2024, mention them only with exact dates and evidence. Do not count personal learning as professional experience.

### Future-quarter learning label

The resume says "Currently Learning: Kubernetes, Terraform, Apache Spark, Prometheus, Grafana (Q4 2026)," but the interview is in Q3 2026. This may look inconsistent.

Safe answer:

> That label is meant to show my planned learning focus through Q4 2026, not that Q4 has already happened. I should have worded it as "learning roadmap through Q4 2026." Today my knowledge is foundational, and I have not used those tools as a production owner. I can explain the concepts and how they would fit my current systems, while being clear about the practical gap.

### Metric discipline

Use each resume metric only in its proper context:

- 70% higher customer engagement, 10,000+ documents, and sub-200ms retrieval: the production RAG pipelines and API integration router using LangChain, GPT-4o, and Pinecone.
- 40% less troubleshooting time: OpenTelemetry and Langfuse distributed tracing across the five-stage pipeline.
- 20% of workloads using 60% of compute: cost analytics finding.
- 10M documents and 50 QPS: Pro-RAG project architecture, not automatically a production client deployment.
- 60% reduction in query-resolution time: multi-modal project compared with its synchronous baseline.

If asked how a metric was measured, give the measurement method. If you cannot explain it, say what the metric represented and avoid overclaiming precision.

## Four adaptable STAR stories

Use only details you can defend. Replace every [FILL IN] with a true fact tonight.

### Story 1: Observability and faster troubleshooting

**Question:** Tell me about a production problem you improved.

**Situation:**

> Our AI service had a five-stage pipeline: orchestrator, grounding, SQL generation, validation, and response. When something slowed down or failed, the symptom appeared at the API level but the cause could be in any stage.

**Task:**

> I needed to make each stage visible so the team could locate latency, error, token, and cost problems instead of treating the pipeline as one black box.

**Action:**

> I instrumented the five stages with OpenTelemetry traces and Langfuse distributed tracing, capturing latency, error, token, and cost data per stage. My approach was like adding tracking numbers at every station in a parcel network: instead of only knowing that a package was late, we could see where it stopped.

**Result:**

> The resume records a 40% reduction in troubleshooting time. [FILL IN: how the before and after time was measured and one concrete incident.] The bigger result was that we could identify the responsible stage quickly and make optimization decisions using evidence.

### Story 2: Cost analysis and model routing

**Question:** Tell me about a time data changed a technical decision.

**Situation:**

> AI usage was growing, but total spend alone did not explain which workloads were inefficient.

**Task:**

> I owned the usage and cost analytics needed to find waste and support a better routing strategy.

**Action:**

> I built a service with Python, SQL, and FastAPI to meter usage by workload. I compared compute or model consumption across use cases and made the distribution visible. This was like examining an electricity bill room by room instead of only seeing the building total.

**Result:**

> The analysis showed that 20% of workloads consumed 60% of compute. That evidence supported model-routing and cost-optimization decisions. [FILL IN: what change was actually made and what was measured afterward.]

### Story 3: Scalable production RAG

**Question:** Describe a system you owned end to end.

**Situation:**

> An enterprise AI application needed fast, trustworthy retrieval over more than 10,000 documents and an API integration router that could connect the result to the application flow.

**Task:**

> I needed to architect the production RAG pipelines and API integration router while keeping retrieval latency low.

**Action:**

> I used LangChain, GPT-4o, and Pinecone for the production RAG and API-router work. Pinecone supported retrieval over the document corpus, while the router connected the AI result to the wider application flow. The separate Pro-RAG project, not this production system, used Qdrant, hybrid retrieval, reranking, and evaluation gates.

**Result:**

> The resume attributes a 70% increase in customer engagement and sub-200 millisecond retrieval across more than 10,000 documents to this RAG and API-router work. [FILL IN: how engagement and latency were measured, whether the latency was average or a percentile, and your exact contribution.]

### Story 4: Enterprise POC and stakeholder delivery

**Question:** Tell me about working with a non-technical stakeholder.

**Situation:**

> A business team had a broad AI opportunity but needed a practical solution with measurable value.

**Task:**

> I needed to help take the requirement through a deployed, monitored system and explain the result.

**Action:**

> For the interview, use only one POC where these details are true: [FILL IN: how you clarified the user, decision, data, success measure, and constraints], [FILL IN: what you personally delivered], and [FILL IN: how the deployed system was monitored].

**Result:**

> My resume says I delivered more than five enterprise POCs from requirements through deployed, monitored systems. For the interview, select one POC and add [FILL IN: client problem, your exact decisions, stakeholder feedback, and measured outcome].

## Core technical questions and easy-English answers

### 1. What is MLOps?

> MLOps is the engineering system that makes model development repeatable and production use reliable. It covers data and code versioning, training, evaluation, approval, deployment, monitoring, rollback, and retraining. It is similar to a food factory: a good recipe is the model, but the factory also needs approved ingredients, quality checks, batch numbers, safe packaging, monitoring, and recall procedures.

### 2. How is MLOps different from DevOps?

> DevOps manages application code and infrastructure delivery. MLOps includes those practices but adds changing data, experiments, model artifacts, model metrics, and drift. The same code can produce a different model when data changes, so reproducibility requires tracking code, data, parameters, environment, and output model together.

### 3. Describe a complete ML delivery lifecycle

> I would start with a measurable business objective and an offline baseline. Then I would validate and version data, train through a reproducible pipeline, log parameters and metrics, register the approved artifact, package serving code, and run automated tests. I would promote through development and staging with a manual or policy approval for production. Deployment would use canary, blue-green, or shadow traffic depending on risk. In production I would monitor service health, data quality, drift, model quality, business KPIs, and cost. A rollback path and retraining trigger must be defined before release.

Analogy: it is a passport process. Training creates the traveler, evaluation checks identity, the registry stores approved records, deployment is border control, and monitoring confirms continued compliance.

### 4. What belongs in an MLOps CI/CD pipeline?

> On a pull request: formatting, linting, unit tests, dependency and secret scans, data-schema tests, and small model or inference tests. On merge: build an immutable image, generate an SBOM if required, scan the image, run integration and evaluation gates, register the artifact, and deploy to staging. After smoke, load, and security checks, production promotion should require an approval appropriate to risk. After deployment, verify health and quality metrics and roll back automatically or manually when thresholds fail.

Important distinction:

- CI checks code and model changes continuously.
- CD delivers approved artifacts safely.
- CT, continuous training, retrains when new verified data or a trigger justifies it.

### 5. What is a model registry?

> A model registry is a controlled catalog of model versions and metadata. It records which artifact was trained, with what data and code, its metrics, approval state, and where it is deployed. It is like a pharmacy inventory: the label identifies the exact medicine batch, its tests, approval, and allowed use. A registry does not by itself serve the model; serving is a separate runtime concern.

AWS SageMaker Model Registry supports model versions, metadata, lineage, approval status, deployment, and CI/CD automation. MLflow also provides model registration, versioning, aliases, tags, and lifecycle management.

### 6. Batch inference or online inference?

> Use batch when results can be prepared on a schedule and throughput matters more than immediate response, such as nightly customer scores. Use online inference when a request needs a low-latency answer, such as fraud scoring during a transaction. Batch is like delivering newspapers in bulk; online is like answering a phone call immediately. I would compare freshness need, latency SLO, volume pattern, cost, and failure recovery before choosing.

### 7. Blue-green, canary, and shadow deployment

- **Blue-green:** keep old and new environments, switch traffic after validation. Fast rollback, higher temporary cost.
- **Canary:** send a small percentage of real traffic to the new version and expand gradually. Limits blast radius but needs careful metrics.
- **Shadow:** duplicate traffic to the new version but do not use its response. Good for comparison, but adds compute cost and requires privacy care.

Analogy: blue-green opens a fully prepared second restaurant; canary lets a few tables try the new menu; shadow lets the kitchen prepare the new dish without serving it.

### 8. What is data drift versus concept drift?

> Data drift means the input distribution changed, such as customers now using different transaction amounts. Concept drift means the relationship between input and correct output changed, such as fraud behavior changing so the old patterns no longer predict fraud. Data drift can be measured without immediate labels. Concept drift usually needs labels or a good proxy. Neither automatically proves the model is bad, so I would connect drift alerts to model and business performance.

### 9. What would you monitor?

Use four layers:

1. **Service:** availability, request rate, p50/p95/p99 latency, error rate, saturation, queue depth.
2. **Data:** schema, nulls, ranges, category changes, freshness, volume, drift.
3. **Model:** quality by segment, calibration, false-positive/false-negative rates, drift, fallback rate.
4. **Business and cost:** conversion, handling time, manual review, cost per successful prediction, GPU/CPU utilization.

For an LLM system, also monitor token usage, provider errors, retrieval quality, groundedness, hallucination, safety events, and human escalation.

### 10. Prometheus versus Grafana

> Prometheus collects and stores numeric time-series metrics and can evaluate alert rules. Grafana queries sources such as Prometheus and turns metrics, logs, and traces into dashboards and alerts. Prometheus is the thermometer and measurement notebook; Grafana is the control-room screen. They complement rather than replace OpenTelemetry: OpenTelemetry standardizes instrumentation and transport, while a metrics backend stores and queries the results.

Truthful bridge:

> My production hands-on experience is with OpenTelemetry and Langfuse distributed tracing. I am learning Prometheus and Grafana. The concepts transfer: instrument the service, use stable low-cardinality dimensions, build SLO-focused views, and alert on symptoms that require action.

### 11. What is Kubernetes, and why use it for ML services?

> Kubernetes maintains the desired state of containerized workloads. A Deployment manages replicated stateless pods and rolling updates; a Service provides stable access; ConfigMaps and Secrets separate configuration; requests and limits guide scheduling; probes control traffic and restarts; and autoscaling adjusts capacity. It is like an airport operations team that keeps the required number of gates staffed even when a worker leaves.

Use it when the workload needs standardized deployment, scaling, resilience, and multi-service operations. Do not use it automatically for a small service if a managed serverless or container service is simpler.

### 12. Liveness, readiness, and startup probes

- **Startup:** Has the application finished starting? Protects slow-starting applications from early restarts.
- **Readiness:** Can it accept traffic now? A failed readiness probe removes the pod from service endpoints.
- **Liveness:** Is it stuck and should Kubernetes restart it?

Analogy: startup asks whether a shop has opened, readiness asks whether it can accept the next customer, and liveness asks whether the staff are still functioning.

### 13. What would an EKS deployment need?

> I would use an image registry such as ECR, an EKS Deployment and Service, an ingress or load balancer, IAM roles with least privilege, Secrets integration, resource requests and limits, probes, autoscaling, logs, metrics, traces, network policies, and controlled rollout. For GPU inference I would also consider node groups, device plugins, scheduling constraints, batching, and expensive idle capacity.

Be explicit: this is a design answer, not a claim of production EKS ownership.

### 14. What is Infrastructure as Code?

> IaC defines infrastructure in versioned configuration instead of manual console clicks. Terraform uses a write-plan-apply workflow and tracks state; CloudFormation provisions AWS resources from templates and can manage them as a stack. It is like keeping a building blueprint under version control instead of relying on someone's memory. Benefits include repeatability, review, auditability, and consistent environments.

Key risks:

- Secrets in code or state.
- Unreviewed destructive plans.
- State corruption or concurrent writes.
- Environment drift.
- Overly broad permissions.

Safe production process: remote encrypted state, locking, least privilege, pinned modules/providers, plan in CI, policy checks, approval before apply, drift detection, and backup/rollback strategy.

### 15. Terraform versus CloudFormation

> Terraform is multi-provider and useful for a consistent workflow across clouds and SaaS systems. CloudFormation is AWS-native and often gets direct support for AWS resource behavior. The choice depends on existing standards, team skill, cloud scope, governance, and operational support. I would not recommend migration only because one tool is fashionable.

### 16. What are EMR, Spark, and Hadoop?

> Spark is a distributed processing engine that divides large jobs across executors. Hadoop is a broader ecosystem historically centered on HDFS storage and YARN resource management, with MapReduce as a processing model. Amazon EMR is a managed AWS platform for running frameworks such as Spark and Hadoop. EMR can run on EC2, EKS, or serverless options depending on the use case.

Analogy: normal Python processing is one kitchen. Spark splits a large catering order across many coordinated kitchens. EMR hires and manages those kitchens on AWS.

### 17. When is Spark justified?

> Use Spark when data volume, parallel transformations, or distributed joins exceed what one machine and a simpler database or Python job can handle economically. Avoid it for small data because cluster startup, shuffles, serialization, and operations add cost and complexity. Start with the simplest tool that meets the SLO.

Common Spark performance reasoning:

- Filter early and read only needed columns.
- Partition for access patterns, but avoid too many tiny files.
- Broadcast genuinely small lookup data.
- Reduce wide shuffles and skew.
- Cache only reused expensive results.
- Tune executor memory, cores, and dynamic allocation using measurements.
- Use adaptive query execution where appropriate.

### 18. How would you ensure data quality?

> Define a contract at every boundary: schema, type, allowed range, required fields, uniqueness, freshness, volume, and referential integrity. Quarantine bad records instead of silently dropping them. Track lineage and test transformations. For ML, compare training and serving transformations to prevent skew. Data quality is like checking ingredients before cooking: a perfect recipe cannot fix spoiled input.

### 19. How would you optimize cloud cost?

> First make cost visible by team, service, environment, model, and useful business output. Then right-size from real CPU, memory, and GPU utilization; autoscale; stop idle non-production resources; use Spot for interruptible work; use Savings Plans for stable demand; reduce unnecessary data transfer and storage; batch or cache where safe; and choose smaller models when quality allows. Every saving must be checked against reliability and performance.

Your bridge:

> My direct evidence is workload-level AI cost analytics and model-routing strategy, not broad AWS estate ownership. I found a concentrated usage pattern and used it to guide optimization. At infrastructure level I would apply the same measure-first approach to resource utilization and unit cost.

### 20. How do you secure an ML platform?

> I would start with identity and data classification. Use least-privilege IAM, short-lived credentials, secrets management, encryption in transit and at rest, private networking where required, image and dependency scanning, signed and immutable artifacts, audit logs, tenant isolation, data minimization, retention controls, and approval gates. For models, also control who can register, approve, and deploy versions. For LLM systems, protect prompts and retrieved data, test prompt injection, filter sensitive output, and keep a human escalation path for high-risk decisions.

## Architecture scenario

### Prompt

Design a secure AWS MLOps platform for a client that trains a risk model daily, serves low-latency predictions, and needs auditability, rollback, drift monitoring, and cost control.

### Start with clarifying questions

1. What decision does the model support, and what is the cost of a false positive or false negative?
2. What are the traffic pattern, p95 latency, availability, freshness, and recovery requirements?
3. What data is sensitive, where may it be stored, and what retention rules apply?
4. When do labels arrive, and how will actual quality be measured?
5. Is there an existing AWS, CI/CD, registry, Kubernetes, or data platform standard?
6. What level of human approval is required before production?

### Proposed flow

```text
Sources -> encrypted S3 landing -> validation/quarantine -> curated data
                                                    |
                                                    v
Scheduled pipeline -> feature transform -> train -> evaluate -> register
                                                        |          |
                                                        |       approval
                                                        v          v
                                                   reports     deployment
                                                                  |
Client -> API/load balancer -> serving endpoint -> prediction + audit event
                                   |                    |
                                   v                    v
                            service telemetry     drift/quality store
                                   |                    |
                                   +------ alerts ------+
```

### Strong answer

> I would separate the data, training, registry, and serving concerns. Raw data lands encrypted with lineage and access control. A validation step checks schema, freshness, ranges, and volume, and sends failed data to quarantine. A reproducible pipeline creates features, trains, evaluates by important segments, and records code, data, parameters, and artifacts. Only a model passing technical and business thresholds can enter an approved registry stage.
>
> For serving, I would begin with a managed endpoint unless the client's platform standard requires EKS. The endpoint would sit behind authenticated access with least-privilege roles. I would use canary rollout, immutable versions, and a one-step rollback. Every prediction would record model version and request metadata without logging sensitive payloads.
>
> Monitoring covers API health, infrastructure utilization, data drift, model quality after labels arrive, business outcomes, and cost per successful prediction. Alerts should connect to a runbook. IaC would recreate environments consistently, and CI/CD would require tests, scans, evaluation gates, and production approval.

### Follow-up trade-offs

- **SageMaker endpoint vs EKS:** managed endpoint reduces operations; EKS offers platform consistency and control but increases ownership.
- **Feature store vs curated tables:** feature store helps reuse and online/offline consistency; it may be unnecessary for a small first use case.
- **Daily automatic retraining:** do not auto-promote blindly. Retrain can be automatic; production approval depends on risk and test results.
- **Drift response:** alert and investigate first. Drift is evidence, not automatic proof of model failure.
- **Cost:** scale to zero where possible for batch, use Spot for interruptible training, right-size endpoints, and track unit cost.

## Troubleshooting playbooks

### Scenario 1: Latency doubled after deployment

> I would first protect users: stop rollout or shift traffic back if the SLO is materially affected. Then compare old and new versions using the same traffic slice. I would inspect p50/p95/p99 latency by stage, error rate, CPU/memory/GPU utilization, queue depth, dependency latency, model size, batch settings, and cold starts. I would check the deployment diff and trace a slow request end to end. After isolating the cause, I would fix it, validate under representative load, redeploy gradually, and write a prevention test or alert.

Do not begin by restarting everything. Preserve evidence.

### Scenario 2: Model quality drops but service metrics look healthy

> The API can be healthy while predictions are wrong. I would verify labels and metric calculation first, then segment quality by time, geography, customer type, and model version. I would compare training and serving features, check data/schema drift, missing values, pipeline changes, and concept changes. If business risk is high, I would roll back or increase human review while investigating.

### Scenario 3: Kubernetes pod keeps restarting

> Check pod events, previous container logs, exit code, probe failures, OOMKilled status, resource limits, configuration and secret mounts, dependency access, and recent image changes. A failed liveness probe might be the symptom, not the cause. If readiness would be enough, an aggressive liveness probe can create a restart loop.

### Scenario 4: Spark job became slow and expensive

> Compare input volume and execution plan, then check skew, shuffle size, spill, executor memory, failed tasks, small files, joins, partition count, caching, and dynamic allocation. A single hot key can make one executor carry most of the load, like one supermarket checkout receiving nearly every customer.

## Behavioral and consulting questions

### Tell me about a conflict

Structure:

> We disagreed about [FILL IN: technical decision]. I first restated the shared outcome and asked each person to define the risk they were protecting against. I brought [FILL IN: benchmark, trace, test, or small prototype] so we could compare options using evidence. We agreed on [FILL IN: decision], documented the trade-off, and achieved [FILL IN: real result]. I learned [FILL IN: lesson].

Do not turn the other person into the villain.

### A client requests an impossible deadline. What do you do?

> I would not say yes and hide the risk. I would clarify the business deadline, identify the smallest valuable and safe outcome, list assumptions and dependencies, and offer options. For example: a limited POC by the date, a production pilot with fewer integrations, or the full scope later. I would show the impact on quality, security, and support for each option, agree on acceptance criteria, and communicate progress early.

### How do you explain a model to a business stakeholder?

> I start with the decision and consequence, not the algorithm. I explain what information the model uses, what output means, when it can be wrong, how performance was tested, and what a human should do when confidence is low. It is similar to a weather forecast: 70% rain is useful only when the user knows the location, time window, reliability, and action to take.

### What if a client asks you to deploy a model that fails your quality gate?

> I would show the failed criterion and business risk, confirm that the test and data are correct, and propose safe alternatives such as fixing the issue, limiting scope, shadow deployment, or adding human review. I would follow governance and escalation procedures. I would not silently lower the threshold to meet a deadline.

### Tell me about ambiguity

Use the enterprise POC story:

> I convert ambiguity into five things: user, decision, data, measurable success, and constraints. Then I propose a small testable slice. This prevents a broad request such as "build AI" from becoming an unmeasurable technology demo.

### What does ownership mean to you?

> Ownership means caring about the result after the code is merged. I define success, identify dependencies, test failure paths, make the system observable, document operational steps, communicate risk early, and follow the production result. It does not mean making every decision alone.

## Honest gap scripts

### "We need 3+ years. You do not have that."

> That is correct. My listed professional timeline starts in November 2024, which is about 22 months by the interview date, so I do not have three full years of infrastructure engineering. I would not want to misrepresent it. What I do offer is concentrated production ownership across Python services, Docker, AWS deployment, AI data pipelines, OpenTelemetry and Langfuse distributed tracing, troubleshooting, and cost analytics. I can contribute immediately in those areas. For Kubernetes, IaC, Spark, Prometheus, and Grafana, I have foundational knowledge and a structured learning roadmap, but not production ownership. I understand if the experience threshold is strict, and I would be interested in how you weigh depth and demonstrated ownership against calendar years.

### "Have you used Kubernetes in production?"

> No, not as a production owner. I currently deploy containerized services and understand the problems Kubernetes solves. I can explain Deployments, Services, probes, resources, autoscaling, secrets, and rollout strategies, and I am learning through hands-on practice. I would pair with the platform team, follow existing standards, and avoid making unsupervised production changes until I had demonstrated competence.

### "Have you used Terraform?"

> I have not owned Terraform in production. I understand declarative desired state, providers, plan and apply, state, modules, drift, and why remote encrypted state and locking matter. My practical experience is currently at the learning level, so I would not claim more.

### "Have you worked with EMR, Spark, or Hadoop?"

> I have not used EMR or Hadoop in production. Spark is on my current learning roadmap. My existing strength is asynchronous Python data processing, SQL, ingestion, retrieval, and validation. I understand that Spark distributes transformations across executors and that EMR manages frameworks such as Spark and Hadoop on AWS. I would first establish why distributed processing is needed, then learn within the team's existing patterns.

### "Have you used MLflow or a feature store?"

> In my Pro-RAG project, I used prompt and configuration versioning plus evaluation gating. That is project evidence, not a claim of production ownership of MLflow or a feature store. I understand that a registry tracks versioned artifacts, metadata, lineage, approval, and lifecycle, while a feature store aims to provide governed reusable features and training-serving consistency. I can map those concepts onto the project without pretending the tools are the same.

### "Have you used Prometheus and Grafana?"

> My production experience is OpenTelemetry and Langfuse distributed tracing, including latency, errors, token usage, and cost per pipeline stage. I am learning Prometheus and Grafana. Prometheus provides a time-series metrics and alerting backend, while Grafana provides visualization and exploration across telemetry sources. The operational thinking transfers, but I would still need hands-on time with their configuration and production practices.

## Recruiter-screening traps

### Trap: Inflating years

Bad: "I have around three years if projects are included."

Good: State exact professional dates and separate employment, internship, personal project, and learning.

### Trap: Claiming a tool through conceptual knowledge

Bad: "Yes, I know Kubernetes."

Good: "I know the core concepts and am practicing, but I have not owned it in production."

### Trap: Calling application cost analytics cloud FinOps

Bad: "I optimized the AWS estate."

Good: "I built workload and model cost analytics; broader cloud resource optimization is a growth area."

### Trap: Saying "end to end" without boundaries

Define what you owned, what the platform or DevOps team owned, and what you influenced.

### Trap: Confidential details

Do not name clients, expose proprietary data, or describe security weaknesses. Use industry, scale, architecture, and outcome.

### Trap: Memorized definitions

For every concept, add one trade-off, failure mode, or example. Consultants are expected to make context-aware recommendations.

### Trap: Resume metric without measurement

Expect: "How did you measure 70%, 40%, or 200ms?" Prepare a truthful measurement method for each.

## Candidate-reported EY interview themes

These are anecdotes, not EY policy. Reports may be incomplete, unverifiable, role-specific, or influenced by the author's perspective. No sufficiently detailed first-hand report for this exact EY MLOps Engineer consultant role was found during this search.

### Closest useful reports

1. **EY GDS Gen AI Senior, Chennai, posted June 18, 2026:** the candidate described a 45-minute first technical round with introduction, current role and team, project walkthrough, REST methods, FastAPI vs Flask, Python operators, a topological-sort coding question, and design of a resume matching and ranking system. This is the strongest recent adjacent first-hand report.
2. **EY Senior Consultant AI & Data discussion, posted July 5, 2026 with candidate follow-up August 7, 2026:** the original poster said the first round was a 30-minute interview with a data analytics manager and the second with senior directors. The later follow-up said there was no coding in that interview but very broad and deep questioning across data engineering, data analysis, data science, ML, and related tools.
3. **EY Senior Consultant Applied AI Engineer, posted June 30, 2026:** the candidate reported an initial technical plus competency interview with a senior manager, a case-study overview with a director, and a final partner round described by the recruiter as focused on motivation, communication, and team fit, with possible technical questions.
4. **EY OpenShift/DevOps Engineer, authored January 10, 2026:** the author reported deep technical coverage of Linux, Kubernetes, AWS, Terraform, CI/CD, and real-world troubleshooting. It is a DevOps role, not MLOps, but the infrastructure themes overlap with this inferred role.

### Practical conclusion from the anecdotes

Prepare for:

- A deep resume walkthrough with follow-up questions.
- Python and API fundamentals.
- One coding question, but do not assume there will be coding.
- System design or a client scenario.
- Kubernetes, AWS, Terraform, CI/CD, monitoring, and troubleshooting.
- Broad questions across data, ML, and production engineering.
- Behavioral evidence of communication, team fit, ownership, and business impact.

## Likely coding questions

The Python examples below were executed successfully during preparation. The SQL is PostgreSQL-compatible and the Kubernetes YAML is an illustrative interview answer, not production-ready infrastructure.

### 1. Reverse the words in a sentence without slicing

This is a general Python practice question. It was not established as a question from the researched EY candidate reports.

```python
def reverse_words(text: str) -> str:
    words = text.split()
    left, right = 0, len(words) - 1
    while left < right:
        words[left], words[right] = words[right], words[left]
        left += 1
        right -= 1
    return " ".join(words)


assert reverse_words("deploy models safely") == "safely models deploy"
assert reverse_words("  one   service ") == "service one"
assert reverse_words("") == ""
```

Time: O(n), where n is the input size.

Space: O(n) for the words and result.

Think aloud: `split()` normalizes repeated whitespace. Ask whether that is acceptable.

### 2. Topological sort for pipeline dependencies

A recent EY GDS Gen AI Senior candidate explicitly reported a topological-sort question.

```python
from collections import defaultdict, deque


def pipeline_order(tasks: list[str], edges: list[tuple[str, str]]) -> list[str]:
    graph: dict[str, list[str]] = defaultdict(list)
    indegree = {task: 0 for task in tasks}

    for before, after in edges:
        if before not in indegree or after not in indegree:
            raise ValueError("edge contains an unknown task")
        graph[before].append(after)
        indegree[after] += 1

    ready = deque(task for task in tasks if indegree[task] == 0)
    order: list[str] = []

    while ready:
        task = ready.popleft()
        order.append(task)
        for next_task in graph[task]:
            indegree[next_task] -= 1
            if indegree[next_task] == 0:
                ready.append(next_task)

    if len(order) != len(tasks):
        raise ValueError("pipeline contains a cycle")
    return order


tasks = ["validate", "train", "evaluate", "deploy"]
edges = [("validate", "train"), ("train", "evaluate"), ("evaluate", "deploy")]
assert pipeline_order(tasks, edges) == tasks
```

Time: O(V + E).

Space: O(V + E).

Analogy: prerequisites at college. You can take a course only when all required earlier courses are complete.

### 3. Aggregate telemetry and find unhealthy models

```python
from collections import defaultdict


def unhealthy_models(events: list[dict], max_error_rate: float) -> list[tuple[str, float]]:
    totals = defaultdict(lambda: [0, 0])
    for event in events:
        model = event["model_version"]
        totals[model][0] += 1
        totals[model][1] += int(event["status"] == "error")

    result = []
    for model, (requests, errors) in totals.items():
        error_rate = errors / requests
        if error_rate > max_error_rate:
            result.append((model, error_rate))
    return sorted(result, key=lambda item: (-item[1], item[0]))


events = [
    {"model_version": "v1", "status": "ok"},
    {"model_version": "v1", "status": "error"},
    {"model_version": "v2", "status": "ok"},
]
assert unhealthy_models(events, 0.4) == [("v1", 0.5)]
```

Time: O(n + m log m), where m is the number of model versions returned.

Space: O(k), where k is the number of model versions.

Follow-ups: missing fields, streaming input, sliding windows, minimum sample size, and alert noise.

### 4. SQL: latest successful model per model name

```sql
WITH ranked AS (
    SELECT
        model_name,
        model_version,
        deployed_at,
        ROW_NUMBER() OVER (
            PARTITION BY model_name
            ORDER BY deployed_at DESC
        ) AS row_num
    FROM deployments
    WHERE status = 'success'
)
SELECT model_name, model_version, deployed_at
FROM ranked
WHERE row_num = 1;
```

Explain:

> I first filter successful deployments. Then I rank each model's versions from newest to oldest and keep rank one. An index beginning with `status, model_name, deployed_at` may help, but I would inspect actual cardinality and the query plan.

### 5. SQL: seven-day error rate by model version

```sql
SELECT
    model_version,
    COUNT(*) AS request_count,
    SUM(CASE WHEN status = 'error' THEN 1 ELSE 0 END) AS error_count,
    1.0 * SUM(CASE WHEN status = 'error' THEN 1 ELSE 0 END)
        / NULLIF(COUNT(*), 0) AS error_rate
FROM inference_events
WHERE created_at >= CURRENT_TIMESTAMP - INTERVAL '7 days'
GROUP BY model_version
HAVING COUNT(*) >= 100
ORDER BY error_rate DESC;
```

Why `HAVING COUNT(*) >= 100`? A model with one failed request should not automatically look worse than a model with thousands of requests. The threshold is a business and statistical decision, not a universal constant.

### 6. Kubernetes YAML: safe basics for a model API

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: model-api
spec:
  replicas: 3
  selector:
    matchLabels:
      app: model-api
  template:
    metadata:
      labels:
        app: model-api
    spec:
      containers:
        - name: api
          image: example.registry/model-api:1.4.2
          ports:
            - containerPort: 8080
          resources:
            requests:
              cpu: "500m"
              memory: "1Gi"
            limits:
              cpu: "1"
              memory: "2Gi"
          startupProbe:
            httpGet:
              path: /startup
              port: 8080
            failureThreshold: 30
            periodSeconds: 5
          readinessProbe:
            httpGet:
              path: /ready
              port: 8080
            periodSeconds: 5
          livenessProbe:
            httpGet:
              path: /live
              port: 8080
            periodSeconds: 10
```

What is missing for production: Service/Ingress, authentication, TLS, Secrets, pod security context, network policy, autoscaling, disruption budget, topology spread, image policy, telemetry, and environment-specific configuration.

### 7. Pseudocode: safe deployment gate

```text
candidate = train(versioned_data, versioned_code)
metrics = evaluate(candidate, holdout, protected_segments)

if not data_quality_passed:
    reject("invalid evaluation data")
if metrics.primary < approved_threshold:
    reject("quality regression")
if metrics.safety > maximum_allowed_risk:
    reject("safety regression")

register(candidate, metrics, lineage, status="pending")
require_human_approval_for_high_risk_model()
deploy_canary(candidate, traffic_percent=5)
monitor(service, quality_proxies, cost)

if canary_breaks_guardrail:
    rollback()
else:
    expand_gradually()
```

Key answer: never tune the gate only to make the current candidate pass.

## Rapid-fire questions

### Docker image versus container

> An image is the immutable packaged blueprint. A container is a running instance of that image. One image can start many containers.

### Why not store secrets in environment files inside the image?

> The image can be copied, cached, scanned, or shared. Secrets should be injected at runtime from an approved secret manager with least privilege and rotation.

### Idempotency

> Repeating the same operation produces the same intended effect. It matters when retries happen. A payment or training-job request should not create duplicates merely because a network timeout caused a retry.

### At-least-once delivery

> A message may be delivered more than once, so the consumer must be idempotent or deduplicate. It favors not losing work over avoiding duplicates automatically.

### p95 latency

> Ninety-five percent of measured requests completed at or below this time. It shows tail behavior better than only the average.

### Horizontal versus vertical scaling

> Horizontal adds instances; vertical gives an instance more CPU or memory. Horizontal often improves resilience but requires statelessness or coordinated state.

### Feature store

> A governed system for creating, discovering, and serving reusable features, often with offline and online access. Its important promise is consistent feature definitions, not merely another database.

### Training-serving skew

> The model sees features calculated differently in production than during training. Use shared transformations, validation, lineage, and comparison tests.

### SLI, SLO, SLA

> SLI is the measured indicator, such as availability. SLO is the internal target. SLA is the formal commitment and may include consequences.

### Logs, metrics, traces

> Logs describe events, metrics summarize numeric behavior over time, and traces follow one request across components. The detective uses all three: diary, dashboard, and route map.

## Timed 60-minute mock interview

Answer aloud. Use a timer. Do not read the prepared answer during the first attempt.

| Minute | Interviewer prompt | Strong answer must contain |
|---:|---|---|
| 0-3 | Tell me about yourself. | Current role, production ownership, one scale/result, role motivation |
| 3-6 | Why EY and why consulting? | Client outcomes, trust, teamwork, technology translation |
| 6-11 | Walk through your production RAG system. | LangChain, GPT-4o, Pinecone, API router, deployment, monitoring, limits |
| 11-15 | How did you measure sub-200ms and 70% engagement? | Real measurement method, percentile if known, environment, your contribution |
| 15-20 | Design an ML CI/CD pipeline. | Tests, registry, gates, rollout, monitoring, rollback |
| 20-25 | Kubernetes pod latency increased. Diagnose it. | User protection, compare versions, metrics, events, traces, rollback |
| 25-30 | Explain drift and monitoring. | Data vs concept, service vs model vs business, labels |
| 30-36 | Design daily training and online serving on AWS. | Clarify, secure data, pipeline, registry, serving, observability, cost |
| 36-40 | When use Spark or EMR? | Distributed threshold, architecture, cost, trade-off, honest gap |
| 40-44 | You lack three years and key tools. Why hire you? | Direct truth, production depth, learning boundary, value now |
| 44-48 | Client wants a bad model deployed tomorrow. | Evidence, risk, options, governance, escalation |
| 48-52 | Tell me about conflict or ambiguity. | Specific STAR, your action, result, learning |
| 52-56 | Coding: topological sort or telemetry aggregation. | Clarify, approach, complexity, edge cases, tests |
| 56-60 | What questions do you have? | Two role-specific questions |

### Self-score after the mock

Give each item 0, 1, or 2:

- I answered the exact question before adding detail.
- I separated personal ownership from team ownership.
- I used only defensible metrics.
- I gave a trade-off, not just a definition.
- I admitted gaps without sounding defeated.
- I connected technology to client or business value.
- I kept normal answers under two minutes.
- I asked clarifying questions before architecture.

Target: at least 12 out of 16.

## Preparation schedule

### Tonight: 3 hours

**First 30 minutes: accuracy pass**

- Fill the overlap explanation.
- Write how every resume metric was measured.
- Identify exact AWS services and CI/CD tools actually used.
- Separate production systems from personal projects and POCs.

**Next 45 minutes: rehearse the opening and STAR stories**

- Record the introduction twice.
- Practice Why EY, Why MLOps, and Why consulting.
- Complete four STAR stories with true details.

**Next 60 minutes: technical depth**

- Study MLOps lifecycle, deployment strategies, drift, monitoring, and CI/CD.
- Review Kubernetes probes/resources/rollouts, IaC state and plan, Spark shuffles/skew, Prometheus/Grafana roles.
- Draw the AWS architecture once from memory.

**Next 30 minutes: coding**

- Implement topological sort without notes.
- Solve one Python aggregation and one SQL window query.
- Explain complexity and edge cases aloud.

**Final 15 minutes: logistics**

- Confirm invite time, timezone, platform, and interviewer names.
- Test camera, microphone, power, network, and backup hotspot.
- Keep resume, this one-page cheat sheet, notebook, and water ready.

### Tomorrow morning: 75 minutes

- 20 min: one architecture answer.
- 20 min: one STAR and one gap answer.
- 20 min: Python and SQL warm-up.
- 15 min: read EY purpose, role notes, and interviewer background if known.

### 12:15 PM to 12:45 PM IST

- Stop heavy study.
- Eat light, hydrate, and silence notifications.
- Join setup by 12:50 PM.
- Keep the calendar invite authoritative if its time differs from this guide.

## Final cheat sheet

### Your proof points

- Production Python, FastAPI, and async services; Django belongs to the earlier software developer role.
- Docker and AWS deployment exposure.
- Production RAG and API router: LangChain, GPT-4o, Pinecone, 10,000+ documents, sub-200ms retrieval, and 70% higher customer engagement.
- OpenTelemetry and Langfuse distributed tracing across orchestrator, grounding, SQL generation, validation, and response stages.
- Distributed tracing associated with 40% faster troubleshooting.
- Cost analytics: 20% of workloads used 60% of compute.
- Five or more enterprise POCs from requirements through deployed, monitored systems.
- Pro-RAG project evidence: Qdrant, hybrid retrieval, reranking, evaluation gating, regression checks, relevance checks, versioning, multi-tenant quotas, and PostgreSQL metering.

### Your boundaries

- About 22 months from the listed November 2024 start, with March 2025 as the shared transition month.
- No claim of three years of infrastructure engineering.
- No production ownership claim for Kubernetes/EKS, Terraform, Spark/EMR/Hadoop, Prometheus/Grafana, MLflow, or feature stores.
- Q4 2026 means roadmap through Q4, not completed experience.

### Your default answer pattern

1. Direct answer.
2. Simple analogy or concrete example.
3. Trade-off or failure mode.
4. Connection to your real experience.

### Architecture checklist

```text
Business goal and SLO
Data and quality
Reproducibility and lineage
Training and evaluation
Registry and approval
Serving and rollout
Security and governance
Observability and drift
Rollback and incident response
Cost and business outcome
```

### Words to prefer

- "I owned..." only when true.
- "I contributed to..." for team work.
- "I designed..." for a project design.
- "I understand... but have not used it in production" for gaps.
- "I would first clarify..." for scenarios.

## Questions to ask the interviewer

Choose two or three:

1. What would successful delivery in the first 90 days look like for this role?
2. How much of the role is hands-on platform engineering versus architecture, client discovery, and delivery coordination?
3. Which cloud and MLOps platform patterns are already standardized, and where would this person be expected to make design decisions?
4. What are the hardest production problems the team is solving now: reliability, deployment speed, governance, drift, cost, or data quality?
5. How does the team divide ownership among data scientists, ML engineers, platform engineers, security, and client teams?
6. How are models approved, monitored, and rolled back for regulated or high-impact client use cases?
7. The role appears to value both production AI and infrastructure depth. Which area is most important on day one?
8. What learning and mentorship support exists for engineers deepening Kubernetes, IaC, and distributed data-platform experience?

Avoid asking questions answered in the invite or public job posting. Do not lead with salary in a technical round unless the interviewer raises it.

## Sources

All online sources were accessed September 15, 2026.

### Official EY sources

1. EY, "Interview tips" - behavioral interviewing, authentic stories, role fit, and two-way discussion: https://www.ey.com/en_us/careers/interview-tips
2. EY, "How we hire" - interviews may be phone, video, or in person; written assessments and exact structure vary by role, country, and service line: https://www.ey.com/en_us/careers/how-we-hire
3. EY, "Tips for your EY interviews" - behavioral, case-study, or combined format: https://www.ey.com/content/dam/ey-unified-site/ey-com/en-us/careers/documents/ey-interview-tips.pdf
4. EY, "About us" - purpose, long-term value, trust, people, and published values: https://www.ey.com/en_us/about-us
5. EY India, "The exceptional EY experience" - technology-enabled innovation and people experience: https://www.ey.com/en_in/careers/exceptional-ey-experience

### Primary technical sources

6. AWS, "Implement MLOps - Amazon SageMaker AI": https://docs.aws.amazon.com/sagemaker/latest/dg/mlops.html
7. AWS, "Model Registration Deployment with Model Registry": https://docs.aws.amazon.com/sagemaker/latest/dg/model-registry.html
8. AWS, "Amazon EMR Documentation": https://docs.aws.amazon.com/emr/
9. AWS, "What is Amazon EMR on EKS?": https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/emr-eks.html
10. AWS, "Optimize Spark performance": https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-spark-performance.html
11. AWS, "Best Practices for Cost Optimization - Amazon EKS": https://docs.aws.amazon.com/eks/latest/best-practices/cost-opt.html
12. Kubernetes, "Deployments": https://kubernetes.io/docs/concepts/workloads/controllers/deployment/
13. Kubernetes, "Liveness, Readiness, and Startup Probes": https://kubernetes.io/docs/concepts/workloads/pods/probes/
14. HashiCorp, "What is Terraform?": https://developer.hashicorp.com/terraform/intro
15. AWS, "What is CloudFormation?": https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html
16. MLflow, "ML Model Registry": https://mlflow.org/docs/latest/ml/model-registry/
17. MLflow, "ML Model Serving": https://mlflow.org/docs/latest/ml/deployment/
18. Prometheus, "Overview": https://prometheus.io/docs/introduction/overview/
19. Grafana, "About Grafana": https://grafana.com/docs/grafana/latest/introduction/

### Candidate anecdotes, not authoritative EY process sources

20. Reddit, r/EY_GDS, "Interview Experience at EY GDS for Gen AI Senior," posted June 18, 2026: https://www.reddit.com/r/EY_GDS/comments/1u917cd/interview_experience_at_ey_gds_for_gen_ai_senior/
21. Reddit, r/interviews, "EY: Senior Consultant - AI & Data," posted July 5, 2026, with candidate follow-up August 7, 2026: https://www.reddit.com/r/interviews/comments/1uohecn/ey_senior_consultant_ai_data/
22. Reddit, r/ernstandyoung, "Partner Interview - TC FS," posted June 30, 2026: https://www.reddit.com/r/ernstandyoung/comments/1ujkomn/partner_interview_tc_fs/
23. Medium, Tanishq Arora, "EY DevOps Engineer Interview Experience + Questions," published January 10, 2026: https://medium.com/@sre-devops-interview/ey-devops-engineer-interview-experience-questions-8d8a7606082d

## Source and confidence note

- The updated resume was visually inspected in full. Resume claims are treated as candidate-provided evidence, not independently verified outcomes.
- The complete JD was not available. The likely role profile comes only from the recruiter's match/gap assessment and is explicitly marked inferred.
- EY sources own claims about EY purpose and interview guidance.
- Official platform documentation owns technical definitions.
- Candidate reports are used only to identify possible question themes. They do not prove what this interview will contain.
