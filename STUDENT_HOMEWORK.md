# bongoDev — Student submission checklist (Ubuntu EC2 manual deployment)

Read [step-by-step.md](step-by-step.md) and deploy the app **without Docker**.

**Evidence and explanations for the checker: [SUBMISSION.md](SUBMISSION.md)** (screenshots in [`submission/screenshots/`](submission/screenshots/)).

- [x] Ubuntu 24.04 EC2 running, SSH access from my own IP only (SUBMISSION.md #01, #03)
- [x] Security group: SSH 22 from my IP; HTTP 80 from everyone; ports 5000/5432 not public (#02)
- [x] Node.js 24, PostgreSQL and Nginx installed natively (#04, #05)
- [x] PostgreSQL application DB and role created using `scripts/setup-database.sh` (#07, #08)
- [x] Backend managed by `incident-backend` systemd service (#06, #07)
- [x] Public URL loads Incident Command Center (#09)
- [x] I created an incident, changed its status and confirmed persistence after refresh (#08, #09)
- [x] I changed the UI heading and redeployed manually using `scripts/deploy-ubuntu.sh` (#09)
- [x] Screenshots and architecture explanation submitted (no secrets) — [SUBMISSION.md](SUBMISSION.md)
- [x] *(Optional)* GitHub Actions self-hosted runner deploys on `git push` (#10–#14)
- [ ] EC2 instance terminated when homework is complete

**Optional follow-up:** Use the included `.github/workflows/deploy.yml` and [docs/GITHUB_ACTIONS.md](docs/GITHUB_ACTIONS.md) to deploy later application changes to the existing Ubuntu server on a Git push.
