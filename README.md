# Interactive BPMN Website: Amazon Fulfillment Center

**An interactive process map of how a package moves through an Amazon Fulfillment Center (FC), from the inbound truck to the delivery driver.**

**Live demo:** [fulfillmentcenterjourney.com](https://fulfillmentcenterjourney.com)

[![Amazon FC interactive BPMN website](assets/amazon-fc-fulfillment-dashboard.png)](https://fulfillmentcenterjourney.com)

---

## Overview
I turned a complex warehouse operation into a visual, click-through workflow based on BPMN (Business Process Model and Notation). Each step shows who does the work, what they do, which tools they use, and who they hand off to. That makes the process easy to understand at a glance.

Built for **Extern Project 308**, an analysis of Amazon FC worker feedback. The map gives context for where workload and scheduling pressure show up in the process.

## Features
- **Flow View:** step cards for each role in the workflow
- **Role details:** responsibilities, tools, collaborators, and a RACI breakdown for each step
- **Story Mode:** guided walkthrough with play/pause, step controls, and speed options
- **3D warehouse scene:** animated with Three.js
- **Fast and lightweight:** one self-contained HTML file with no build step, hosted on Cloudflare

## Workflow covered
Truck Driver → Receiving → Water Spider → Stower → Picker → Packer → SLAM → Shipping → Delivery Driver, with **Problem Solver** supporting across the flow.

## Skills demonstrated
| Area | Details |
|---|---|
| Business process analysis | BPMN-style process mapping, RACI, role handoffs |
| Front-end development | HTML, CSS, JavaScript, Three.js |
| Data storytelling | Turning operations into a guided visual narrative |
| Deployment | Cloudflare Workers, custom domain and DNS setup |
| AI-assisted building | Structured prompting with ChatGPT, Claude, and Perplexity |

## Repository structure
```
interactive-bpmn-amazon-fc/
├── site/index.html   # The live website
├── assets/           # Screenshots
└── docs/             # Case study, prompts, and build workflow
```

## Run locally
Download `site/index.html` and open it in any browser.

---

*Educational project. Not affiliated with or endorsed by Amazon.*

**Steve Okyere Oduro-Amoyaw** · Park University · [LinkedIn](https://www.linkedin.com/in/steveoduroamoyaw/) · [GitHub](https://github.com/Steve0a)
