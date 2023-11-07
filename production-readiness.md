## General

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
| **Ownership** |  Service owners are identified | Critical | | :heavy_check_mark: | 
|   | Contact information and methods are provided   | Critical | | :heavy_check_mark: | 
| **Onboarding** | Integration instructions for APIs are documented  | Important  | |  | 
| **SLI/SLO/SLA**  | The SLIs and SLOs are documented and accessible  | Critical  | |  | 
|   | If applicable, you’ve also documented the SLAs  | Important | |  | 

## Disaster recovery (DR)

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
| **Disaster recovery**  | DR plans have been documented  | Critical  | | | 
|   | DR plans have been tested (or re-tested) prior to launch  | Critical  | | | 
| **Backups**  | Backups of data occur regularly according to the service tier  | Critical  | | | 
| **Redundancy**  | Services should include at least two instances   |  Critical | | | 
|   | If applicable for the service tier, services are deployed in multiple zones or regions | Critical  | | | 

## Deployment

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
| **Deployment strategy**  | The automated deployment strategy has been documented (for example, blue-green, canary, or others to create safer zero-downtime deployments)  |  Nice to have | | | 
| **Continuous integration**   | When engineers commit their changes, the system kicks off automated builds, tests, and deployment to a lower-level environment  | Important  | | | 
|   | Pipeline failure results in a notification to the responsible team to resolve the issue prompt  | Nice to have  | | | 
| **Continuous delivery**  | Changelogs and release notes indicate what changes exist in each environment | Critical  | | | 
|   | Deploying to production involves nothing more than approval and a button click | Nice to have  | | | 
|  **Static code analysis** | Code is automatically scanned, formatted, or linted according to coding standards  | Important  | | | 

## Operations

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
| **On-call policy**  | The service has an on-call system that pages the owning team for incidents (ideally, this involves tools like PagerDuty or Squadcast)  | Critical  | | | 
| **Incident management**  | The incident management and escalation processes have been documented (this includes processes for postmortem and long-term remediation)  | Critical  | | | 
| **Runbooks**  | Team has written runbooks with known failure scenarios that are easily accessible by others  | Critical  | | | 
|   | Team updates runbooks whenever they uncover a new scenario  | Critical  | | | 
| **Logging**  | The service utilizes centralized logging  |  Critical | | | 
|   | Logs can be accessed easily  | Important  | | | 
|  **Metrics** | At a minimum, the service supports the Four Golden Signals - latency, errors, traffic, and saturation   |  Critical | | | 
| **Tracing**   | The application transactions can be traced, using the appropriate tools and sampling configuration for the service  | Important  | | | 

## Testing

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
|  **Unit tests** | Unit tests execute at every code push, automatically  | Nice to have  | | | 
| **Integration tests**  | If appropriate, automated integration tests execute and pass successfully  |  Nice to have | | | 
| **End-to-end acceptance tests**  | Automated end-to-end or acceptance tests run as part of the Continuous Integration/Continuous Deployment (CI/CD pipeline)  | Nice to have  | | | 
|   | If manual testing is required, test results are documented  | Critical | | | 
| **Broken tests**  | Failing tests break the build  | Critical  | | | 

## Resiliency 

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
| **Load testing**  | Load tests are automated or occur on a regular cadence  | Important  | | | 
|   | Load test results are documented and published  | Important  | | | 
| **Stress testing**  | Stress tests are automated or occur on a regular cadence  | Important  | | | 
|   | Stress test results are documented and published   |  Nice to have  | | | 
| **Chaos engineering**  | Once the applications have proven the ability to stand up to load and stress, the team integrates chaos engineering to identify weak points and opportunities to reduce failures  | Nice to have | | | 

## Security 

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
| **Authentication/authorization**  | Each service or application requires proper authentication and authorization  | Critical  | | | 
| **Secrets management**  | Secrets are secured properly in a vault or secret store  | Critical  | | | 
|   | The build code-scanning tools like truffleHog or git-secrets to identify potential secrets  | Critical  | | | 
|  **Static application security testing (SAST)** | Static code analysis tools like Checkmarx or Snyk monitor code in the CI/CD pipeline  | Important  | | | 
|   | The build breaks any time there are security vulnerabilities above a certain threshold (thresholds are set based on service needs)  | Nice to have  | | | 
| **Dynamic application security testing (DAST)**  | Automated DAST runs at appropriate intervals  | Important  | | | 
|   | Complete manual DAST or pen testing runs according to the security requirements of the service or company | Important  | | | 
| **Dependency scan**  | All dependencies use the latest or patched version  | Important  | | | 

## Governance, Risk, Compliance (GCR)

| Area   | Item  | Priority  | Comments | Done? |
|---|---|---|---|---|
| **GRC documentation**  | GRC checklists have been completed as required  | Critical  | | | 
| **Confidentiality, integrity, availability (CIA) rating**  |  The team has documented and published the CIA rating of the service | Important  | | | 
