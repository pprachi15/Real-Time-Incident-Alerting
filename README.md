# Real Time Incident Alerting and SLA Monitoring System  
Applied Business Strategy Challenge – Day 5

A complete operational analysis and TPM strategy for strengthening service reliability, reducing SLA breaches, and improving system performance.  
This work simulates how large financial institutions such as Goldman Sachs, JPMorgan, and Morgan Stanley manage production incidents at scale.

---

## Project Overview

This project analyzes one thousand five hundred simulated system incidents across core financial services.  
The goal is to understand operational bottlenecks and produce actionable insights that help engineering, risk, and operations teams reduce outages and SLA breaches.

The dataset includes severity, root cause, detection time, resolution time, service ownership, and SLA compliance.  
The analysis provides a foundational operational health view that informs reliability improvements and on call strategy.

---

## Key Insights

• Thirty two percent of all incidents breach SLA, indicating elevated operational risk.  
• Database Slowdown and Dependency Failure are the most common root causes.  
• Medium severity incidents dominate volume, highlighting recurring systemic inefficiencies.  
• Auth API, Payments, and Fraud Engine experience the highest SLA breach rates.  
• Mean Time to Detect is approximately fourteen minutes.  
• Mean Time to Resolve is approximately fifty three minutes.

---

## Technical Approach

This project uses a synthetic incident dataset generated entirely in Python.

The analytical workflow includes:

• Loading and validating the simulated incident dataset  
• Exploring severity distribution to identify volume hotspots  
• Visualizing detection and resolution times using histograms  
• Creating a heatmap for Severity versus SLA Breach  
• Computing service reliability ranking based on incident count  
• Breaking down root cause frequency  
• TPM operational metrics  
  • Mean Time to Detect  
  • Mean Time to Resolve  
  • SLA Breach Rate  
• Computing service level SLA breach rate to identify high risk platforms

All visualizations were created using Matplotlib and Seaborn.

---

## TPM Perspective – What Happens Next

If I were in the shoes of a Technical Program Manager overseeing platform reliability, I would focus on the following initiatives.

### Reliability Alignment and Execution  
• Align engineering, SRE, product, and risk teams on the top incident drivers.  
• Define clear reliability goals for the next ninety days.  
• Establish service level objectives for detection and resolution timelines.

### Tooling and Visibility  
• Build operational dashboards for MTTD, MTTR, SLA breaches, and service reliability.  
• Add automated alerts for latency spikes, rising incident volume, and threshold breaches.  
• Enable early warning indicators for potential outage patterns.

### Engineering and Process Improvements  
• Prioritize fixes for database and dependency related failures.  
• Reduce SLA breach rates on Auth API, Payments, and Fraud Engine.  
• Improve runbooks and on call readiness.  
• Reduce average detection and resolution times through automation and playbooks.

### Governance and Communication  
• Host biweekly incident review with clear ownership and follow up remediation.  
• Establish RCA templates and remediation tracking.  
• Report operational health summaries to leadership with actionable recommendations.

---

## Impact Summary

This project demonstrates how operational analytics strengthens reliability, reduces customer impact, and improves incident response.  
The insights support TPM decision making across engineering, SRE, and product by creating visibility into:

• Early failure signals  
• Remediation priorities  
• High risk services  
• SLA compliance performance  
• Engineering workload planning
