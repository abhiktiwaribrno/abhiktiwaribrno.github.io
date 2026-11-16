Here is your complete, self-contained index.html portfolio file tailored to your SAP Technical Program Management and cloud transformation background. It features a clean, executive light-corporate aesthetic with deep sapphire blue (#0284c7) and slate accents, semantic HTML5, smooth scroll animations, and responsive navigation.

Complete index.html

html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Abhishek Tiwari | SAP Technical Project Manager</title>
  <meta name="description" content="Portfolio of Abhishek Tiwari — SAP Technical Project Manager at MSD with 20+ years of experience in SAP S/4HANA, RISE with SAP cloud migrations, ZDO upgrades, and regulated CSV/SOX delivery." />
  
  <!-- Open Graph / Social Meta Tags -->
  <meta property="og:type" content="website" />
  <meta property="og:title" content="Abhishek Tiwari | SAP Technical Project Manager" />
  <meta property="og:description" content="Technical Project Manager and former SAP Basis Lead delivering global SAP S/4HANA implementations, RISE with SAP cloud migrations, and zero-downtime upgrades across regulated environments." />
  <meta property="og:locale" content="en_US" />

  <!-- Google Fonts: Plus Jakarta Sans & Inter -->
  <link rel="preconnect" href="https://googleapis.com">
  <link rel="preconnect" href="https://gstatic.com" crossorigin>
  <link href="https://googleapis.com/css2?family=Inter:wght@400;500;600&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg-page: #f8fafc;
      --bg-surface: #ffffff;
      --bg-subtle: #f1f5f9;
      --text-primary: #0f172a;
      --text-secondary: #475569;
      --text-muted: #64748b;
      --accent: #0284c7;
      --accent-dark: #0369a1;
      --accent-soft: #e0f2fe;
      --accent-border: #bae6fd;
      --success-bg: #dcfce7;
      --success-text: #15803d;
      --border: #e2e8f0;
      --shadow-sm: 0 1px 3px rgba(15, 23, 42, 0.05), 0 1px 2px rgba(15, 23, 42, 0.03);
      --shadow-md: 0 10px 25px -5px rgba(15, 23, 42, 0.06), 0 8px 10px -6px rgba(15, 23, 42, 0.04);
      --radius-md: 12px;
      --radius-lg: 18px;
      --max-width: 1100px;
      --nav-height: 70px;
    }

    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
      scroll-padding-top: calc(var(--nav-height) + 24px);
    }

    @media (prefers-reduced-motion: reduce) {
      html {
        scroll-behavior: auto;
      }
      .reveal {
        opacity: 1 !important;
        transform: none !important;
        transition: none !important;
      }
    }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      background-color: var(--bg-page);
      color: var(--text-primary);
      line-height: 1.65;
      -webkit-font-smoothing: antialiased;
    }

    h1, h2, h3, h4, .monogram {
      font-family: 'Plus Jakarta Sans', sans-serif;
      letter-spacing: -0.02em;
      line-height: 1.25;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: 100%;
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 0 24px;
    }

    /* Sticky Top Navigation */
    .navbar {
      position: sticky;
      top: 0;
      z-index: 1000;
      height: var(--nav-height);
      background: rgba(255, 255, 255, 0.9);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
    }

    .nav-inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 100%;
    }

    .monogram {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 42px;
      height: 42px;
      border-radius: 10px;
      background: var(--text-primary);
      color: #ffffff;
      font-weight: 800;
      font-size: 1rem;
      letter-spacing: 0.04em;
      transition: background-color 0.2s ease, transform 0.2s ease;
    }

    .monogram:hover, .monogram:focus-visible {
      background: var(--accent);
      transform: translateY(-1px);
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 24px;
      list-style: none;
    }

    .nav-links a {
      font-size: 0.875rem;
      font-weight: 500;
      color: var(--text-secondary);
      transition: color 0.2s ease;
      padding: 6px 2px;
    }

    .nav-links a:hover, .nav-links a:focus-visible {
      color: var(--accent);
    }

    .hamburger {
      display: none;
      background: none;
      border: 1px solid var(--border);
      border-radius: 8px;
      padding: 8px 10px;
      cursor: pointer;
      color: var(--text-primary);
    }

    /* Hero Section */
    .hero {
      padding: 72px 0 48px;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.45fr 0.75fr;
      gap: 48px;
      align-items: center;
    }

    .availability-badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: var(--success-bg);
      color: var(--success-text);
      font-size: 0.8125rem;
      font-weight: 600;
      padding: 6px 14px;
      border-radius: 999px;
      margin-bottom: 20px;
    }

    .status-dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: #16a34a;
      box-shadow: 0 0 0 3px rgba(22, 163, 74, 0.2);
    }

    .hero h1 {
      font-size: clamp(2.25rem, 4.5vw, 3.25rem);
      font-weight: 800;
      color: var(--text-primary);
      margin-bottom: 10px;
    }

    .hero-subtitle {
      font-size: 1.15rem;
      font-weight: 600;
      color: var(--accent-dark);
      margin-bottom: 20px;
    }

    .hero-summary {
      font-size: 1.02rem;
      color: var(--text-secondary);
      margin-bottom: 24px;
      max-width: 65ch;
    }

    .chip-row {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 30px;
    }

    .chip {
      font-size: 0.8rem;
      font-weight: 500;
      background: var(--bg-surface);
      color: var(--text-secondary);
      border: 1px solid var(--border);
      padding: 5px 12px;
      border-radius: 999px;
    }

    .btn-group {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      padding: 11px 20px;
      border-radius: 10px;
      font-size: 0.9rem;
      font-weight: 600;
      transition: all 0.2s ease;
      cursor: pointer;
    }

    .btn-primary {
      background: var(--accent);
      color: #ffffff;
      border: 1px solid var(--accent);
      box-shadow: 0 4px 12px rgba(2, 132, 199, 0.22);
    }

    .btn-primary:hover {
      background: var(--accent-dark);
      border-color: var(--accent-dark);
      transform: translateY(-1px);
    }

    .btn-secondary {
      background: var(--bg-surface);
      color: var(--text-primary);
      border: 1px solid var(--border);
    }

    .btn-secondary:hover {
      border-color: var(--accent);
      color: var(--accent);
      background: var(--accent-soft);
    }

    /* Photo / Monogram Card in Hero */
    .hero-visual {
      display: flex;
      justify-content: center;
    }

    .photo-frame {
      width: 100%;
      max-width: 300px;
      aspect-ratio: 1 / 1;
      border-radius: 24px;
      background: linear-gradient(145deg, #0f172a 0%, #1e293b 60%, #0369a1 100%);
      border: 1px solid var(--border);
      box-shadow: var(--shadow-md);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      color: #ffffff;
      position: relative;
      overflow: hidden;
      padding: 24px;
      text-align: center;
    }

    .photo-frame img {
      position: absolute;
      inset: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .photo-initials {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: 4rem;
      font-weight: 800;
      letter-spacing: 0.05em;
      color: #38bdf8;
      margin-bottom: 8px;
    }

    .photo-caption {
      font-size: 0.85rem;
      color: #cbd5e1;
      font-weight: 500;
    }

    /* Profile Card & Stats */
    .profile-card {
      background: var(--bg-surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-lg);
      padding: 32px;
      box-shadow: var(--shadow-md);
      margin-bottom: 64px;
    }

    .profile-top {
      display: grid;
      grid-template-columns: 1fr 1.2fr;
      gap: 32px;
      padding-bottom: 28px;
      border-bottom: 1px solid var(--border);
      align-items: start;
    }

    .profile-identity h2 {
      font-size: 1.4rem;
      margin-bottom: 4px;
    }

    .profile-identity p {
      color: var(--text-secondary);
      font-size: 0.95rem;
      font-weight: 500;
    }

    .profile-bullets {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .profile-bullets li {
      position: relative;
      padding-left: 20px;
      font-size: 0.94rem;
      color: var(--text-secondary);
    }

    .profile-bullets li::before {
      content: "✓";
      position: absolute;
      left: 0;
      color: var(--accent);
      font-weight: 700;
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
      padding-top: 28px;
    }

    .stat-item {
      padding: 12px 16px;
      background: var(--bg-page);
      border-radius: var(--radius-md);
      border: 1px solid var(--border);
    }

    .stat-number {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: 1.75rem;
      font-weight: 800;
      color: var(--accent-dark);
      line-height: 1.15;
      margin-bottom: 4px;
    }

    .stat-label {
      font-size: 0.82rem;
      font-weight: 500;
      color: var(--text-secondary);
      line-height: 1.4;
    }

    /* Section Styling */
    section.content-section {
      padding: 56px 0;
      border-top: 1px solid var(--border);
    }

    .section-kicker {
      display: inline-block;
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: 0.8rem;
Use code with caution.
font-weight: 700;
text-transform: uppercase;
letter-spacing: 0.1em;
color: var(--accent);
margin-bottom: 8px;
}
.section-title {
font-size: clamp(1.65rem, 3vw, 2.1rem);
font-weight: 700;
color: var(--text-primary);
margin-bottom: 28px;
}
/* 01 About */
.about-grid {
display: grid;
grid-template-columns: 1.2fr 1fr;
gap: 40px;
align-items: start;
}
.about-text p {
color: var(--text-secondary);
margin-bottom: 18px;
font-size: 0.98rem;
}
.tag-cloud {
display: flex;
flex-wrap: wrap;
gap: 8px;
margin-top: 20px;
}
.tag-accent {
background: var(--accent-soft);
color: var(--accent-dark);
border: 1px solid var(--accent-border);
font-size: 0.82rem;
font-weight: 600;
padding: 6px 13px;
border-radius: 999px;
}
.working-style-card {
background: var(--bg-surface);
border: 1px solid var(--border);
border-radius: var(--radius-lg);
padding: 28px;
box-shadow: var(--shadow-sm);
}
.working-style-card h3 {
font-size: 1.15rem;
margin-bottom: 18px;
}
.style-list {
list-style: none;
display: flex;
flex-direction: column;
gap: 16px;
}
.style-list li {
font-size: 0.92rem;
color: var(--text-secondary);
padding-left: 14px;
border-left: 3px solid var(--accent);
}
.style-list strong {
color: var(--text-primary);
display: block;
margin-bottom: 2px;
}
/* 02 Expertise & Case Studies */
.cards-grid-2 {
display: grid;
grid-template-columns: repeat(2, 1fr);
gap: 24px;
}
.card {
background: var(--bg-surface);
border: 1px solid var(--border);
border-radius: var(--radius-lg);
padding: 28px;
box-shadow: var(--shadow-sm);
transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
}
.card:hover {
transform: translateY(-2px);
box-shadow: var(--shadow-md);
border-color: var(--accent-border);
}
.card h3 {
font-size: 1.18rem;
margin-bottom: 10px;
color: var(--text-primary);
}
.card-lead {
font-size: 0.93rem;
color: var(--text-secondary);
margin-bottom: 16px;
}
.card-points {
list-style: none;
display: flex;
flex-direction: column;
gap: 10px;
}
.card-points li {
font-size: 0.89rem;
color: var(--text-secondary);
padding-left: 16px;
position: relative;
}
.card-points li::before {
content: "•";
position: absolute;
left: 0;
color: var(--accent);
font-weight: 700;
}
.card-points strong {
color: var(--text-primary);
}
.subsection-heading {
font-size: 1.3rem;
margin: 44px 0 20px;
color: var(--text-primary);
}
.case-study-card {
border-top: 4px solid var(--accent);
}
.case-meta {
margin-top: 16px;
padding-top: 16px;
border-top: 1px solid var(--border);
font-size: 0.88rem;
}
.case-outcome {
background: var(--bg-subtle);
padding: 12px 14px;
border-radius: 8px;
margin-top: 12px;
font-size: 0.9rem;
color: var(--text-primary);
}
/* 03 Projects / Products */
.product-card {
display: flex;
flex-direction: column;
gap: 14px;
}
.product-header {
display: flex;
flex-wrap: wrap;
align-items: center;
justify-content: space-between;
gap: 12px;
}
.status-pill {
font-size: 0.78rem;
font-weight: 700;
text-transform: uppercase;
letter-spacing: 0.05em;
background: var(--accent-soft);
color: var(--accent-dark);
padding: 4px 12px;
border-radius: 999px;
}
/* 04 Experience Timeline */
.timeline {
position: relative;
padding-left: 28px;
display: flex;
flex-direction: column;
gap: 28px;
}
.timeline::before {
content: "";
position: absolute;
left: 7px;
top: 8px;
bottom: 8px;
width: 2px;
background: var(--border);
}
.timeline-item {
position: relative;
background: var(--bg-surface);
border: 1px solid var(--border);
border-radius: var(--radius-lg);
padding: 24px 28px;
box-shadow: var(--shadow-sm);
}
.timeline-item::before {
content: "";
position: absolute;
left: -27px;
top: 28px;
width: 14px;
height: 14px;
border-radius: 50%;
background: var(--accent);
border: 3px solid var(--bg-page);
box-shadow: 0 0 0 1px var(--accent);
}
.exp-header {
display: flex;
flex-wrap: wrap;
justify-content: space-between;
align-items: baseline;
gap: 8px;
margin-bottom: 6px;
}
.exp-role {
font-size: 1.15rem;
font-weight: 700;
color: var(--text-primary);
}
.exp-date {
font-size: 0.85rem;
font-weight: 600;
color: var(--accent-dark);
background: var(--accent-soft);
padding: 3px 10px;
border-radius: 6px;
}
.exp-company {
font-size: 0.95rem;
font-weight: 600;
color: var(--text-secondary);
margin-bottom: 12px;
}
.exp-desc {
font-size: 0.93rem;
color: var(--text-secondary);
margin-bottom: 14px;
}
.exp-award {
display: inline-block;
font-size: 0.84rem;
font-weight: 600;
color: #92400e;
background: #fef3c7;
border: 1px solid #fde68a;
padding: 5px 12px;
border-radius: 8px;
margin-bottom: 14px;
}
.skill-tags-mini {
display: flex;
flex-wrap: wrap;
gap: 6px;
}
.skill-tag-mini {
font-size: 0.78rem;
font-weight: 500;
background: var(--bg-subtle);
color: var(--text-secondary);
padding: 4px 10px;
border-radius: 6px;
}
/* 05 Skills */
.skills-grid {
display: grid;
grid-template-columns: repeat(2, 1fr);
gap: 24px;
}
.skill-group h3 {
font-size: 1.05rem;
margin-bottom: 14px;
color: var(--text-primary);
}
.skill-cloud {
display: flex;
flex-wrap: wrap;
gap: 8px;
}
.skill-pill {
font-size: 0.84rem;
font-weight: 500;
background: var(--bg-page);
color: var(--text-primary);
border: 1px solid var(--border);
padding: 6px 12px;
border-radius: 8px;
}
/* 06 Credentials */
.credentials-grid {
display: grid;
grid-template-columns: repeat(2, 1fr);
gap: 24px;
}
.cred-list {
list-style: none;
display: flex;
flex-direction: column;
gap: 14px;
}
.cred-list li {
font-size: 0.92rem;
color: var(--text-secondary);
padding-bottom: 12px;
border-bottom: 1px solid var(--bg-subtle);
}
.cred-list li:last-child {
border-bottom: none;
padding-bottom: 0;
}
.cred-level {
display: inline-block;
font-size: 0.75rem;
font-weight: 700;
text-transform: uppercase;
letter-spacing: 0.04em;
color: var(--accent-dark);
margin-bottom: 2px;
}
.cred-title {
display: block;
font-weight: 600;
color: var(--text-primary);
}
/* 07 Contact */
.contact-box {
background: var(--text-primary);
color: #ffffff;
border-radius: var(--radius-lg);
padding: 44px 36px;
text-align: center;
}
.contact-box .section-kicker {
color: #38bdf8;
}
.contact-box h2 {
font-size: clamp(1.75rem, 3vw, 2.25rem);
color: #ffffff;
margin-bottom: 12px;
}
.contact-box p {
color: #cbd5e1;
max-width: 56ch;
margin: 0 auto 28px;
font-size: 0.98rem;
}
.contact-links {
display: flex;
flex-wrap: wrap;
justify-content: center;
gap: 14px;
}
.btn-light {
background: #ffffff;
color: var(--text-primary);
border: 1px solid #ffffff;
}
.btn-light:hover {
background: #e0f2fe;
border-color: #e0f2fe;
}
.btn-outline-light {
background: transparent;
color: #ffffff;
border: 1px solid rgba(255, 255, 255, 0.3);
}
.btn-outline-light:hover {
border-color: #38bdf8;
color: #38bdf8;
}
/* Footer */
footer {
padding: 32px 0 48px;
text-align: center;
font-size: 0.875rem;
color: var(--text-muted);
}
/* Scroll Reveal */
.reveal {
opacity: 0;
transform: translateY(16px);
transition: opacity 0.55s ease, transform 0.55s ease;
}
.reveal.is-visible {
opacity: 1;
transform: translateY(0);
}
/* Responsive Breakpoints */
@media (max-width: 900px) {
.hero-grid,
.profile-top,
.about-grid,
.cards-grid-2,
.skills-grid,
.credentials-grid {
grid-template-columns: 1fr;
}
.stats-grid {
grid-template-columns: repeat(2, 1fr);
}
.hero-visual {
order: -1;
justify-content: flex-start;
}
.photo-frame {
max-width: 180px;
border-radius: 18px;
}
.photo-initials {
font-size: 2.75rem;
}
}
@media (max-width: 768px) {
.hamburger {
display: inline-flex;
align-items: center;
justify-content: center;
}
.nav-links {
display: none;
position: absolute;
top: var(--nav-height);
left: 0;
right: 0;
background: var(--bg-surface);
flex-direction: column;
align-items: stretch;
gap: 0;
padding: 12px 24px 20px;
border-bottom: 1px solid var(--border);
box-shadow: var(--shadow-md);
}
.nav-links.open {
display: flex;
}
.nav-links a {
padding: 12px 0;
border-bottom: 1px solid var(--bg-subtle);
}
.nav-links li:last-child a {
border-bottom: none;
}
}
@media (max-width: 480px) {
.stats-grid {
grid-template-columns: 1fr;
}
.profile-card,
.card,
.timeline-item,
.contact-box {
padding: 22px 20px;
}
}


AT
01 About
02 Expertise
03 Projects
04 Experience
05 Skills
06 Credentials
07 Contact



Open to Senior Leadership roles

Abhishek Tiwari
SAP Technical Project Manager at MSD · Brno, Czech Republic

I am a Technical Project Manager and former SAP Basis Lead with 18+ years of experience delivering complex ERP transformations across pharmaceutical, manufacturing, publishing, and tech enterprises. For the past 8+ years, I have led global SAP S/4HANA implementations, RISE with SAP cloud migrations, and multi-country rollouts spanning Europe, North America, and Asia. Backed by hands-on expertise in SAP HANA, Linux/AIX, Oracle/DB2, Solution Manager, and Azure/AWS, I bridge the gap between deep technical engineering and executive governance—challenging architecture estimates, building bulletproof cutover runbooks, and keeping high-stakes deliveries on track. My core focus is regulated, high-availability environments requiring Computer System Validation (CSV), SOX compliance, and Zero Downtime Option (ZDO) upgrades.
SAP Technical Project Manager
SAP Transformation & Program Leadership
IICA Registered Independent Director
SAP S/4HANA, SAP Focused Run & SAP Focused Insights
Delivering Global SAP Programs
View My Work
LinkedIn
Get in Touch

AT
SAP Technical Project Manager
20+ Years in SAP Technical


Abhishek Tiwari
SAP Technical Project Manager at MSD · Brno, Czech Republic


Directing global SAP S/4HANA implementations, RISE with SAP cloud migrations (Azure/AWS), and multi-country rollouts across Europe, North America, and Asia.
Engineering 24/7 cutover runbooks and Zero Downtime Option (ZDO) upgrade strategies in regulated CSV and SOX environments.
Bridging hands-on SAP Basis, HANA, Linux/AIX, and database engineering with executive PMO steering committee governance.

20+
Years in SAP Technical & Managerial Roles


200+
SAP Instances & 26 Production Systems Directed


-20%
Project Risk Reduction via Toll-Gate Governance


+15%
Stakeholder Satisfaction Score Improvement


01 — About
Translating complex SAP landscapes into resilient cloud operations
I am a Technical Project Manager and former SAP Basis Lead with 18+ years of end-to-end enterprise delivery experience across pharmaceutical, manufacturing, publishing, and technology organisations. Over the past eight years, I have directed global SAP S/4HANA implementations, RISE with SAP cloud migrations, and multi-country rollouts spanning Europe, North America, and Asia.


Unlike purely non-technical project managers, I bring a deep hands-on foundation in SAP HANA, Linux/AIX, Oracle/DB2, Solution Manager, and Azure/AWS. This technical depth enables me to validate architectural estimates, engineer airtight cutover runbooks, and translate complex infrastructure risks into clear, actionable decisions for executive steering committees.


I specialise in mission-critical, highly regulated environments that demand strict Computer System Validation (CSV), SOX audit readiness, and Zero Downtime Option (ZDO) upgrade strategies—delivering high-stakes transformations on schedule, within budget, and with zero disruption to daily business operations.
Zero-Downtime Transformations
Cloud Migration Governance
Regulatory & CSV Compliance
Risk & TCO Optimization
Cross-Border Team Leadership

Working Style


Toll-Gate Governance
Running disciplined Preparation, Realisation, Testing, and Cutover gates with transparent Go/No-Go readiness criteria.


Technical Credibility
Challenging vendor estimates and validating architecture directly with Basis, database, and cloud engineering teams.


Executive Clarity
Translating complex landscape dependencies into concise PMO dashboards, RAID logs, and steering committee briefs.


Audit-Ready Documentation
Embedding CSV/SOX change controls, rollback playbooks, and Known Error Databases into everyday delivery to lower long-term TCO.




02 — Expertise
End-to-end SAP delivery, cloud migration, and governance
SAP S/4HANA & RISE with SAP Cloud Transformations

Leading full-lifecycle ERP implementations and cloud migrations onto hyperscaler infrastructures with a focus on scalability, disaster recovery, and security compliance.


Cloud Roadmap Alignment: Aligning RISE with SAP technical architectures with corporate business roadmaps and stakeholder expectations.
OS/DB & Hyperscaler Migrations: Executing homogeneous and heterogeneous migrations onto Microsoft Azure and AWS using Database Migration Option (DMO) approaches.
Performance & Hypercare Validation: Overseeing intensive load, stress, and volume testing alongside rapid-response post-go-live hypercare governance.

Zero-Disruption Cutover & Upgrade Engineering

Orchestrating high-stakes technical cutovers and complex upgrades across global multi-tier landscapes while safeguarding business continuity.


Cutover Playbook Execution: Designing hyper-detailed cutover runbooks and coordinating 24/7 technical shift schedules across international teams.
Zero Downtime Upgrades: Advocating for and executing Zero Downtime Option (ZDO) methodologies to minimize operational downtime during major releases.
Fallback & Data Integrity: Owning end-to-end technical fallback strategies and rehearsed rollback procedures to protect corporate data.

Enterprise PMO Governance & Risk Control

Steering complex multi-country programs on time and within budget by combining SAP Activate, PRINCE2®, Agile, and Waterfall frameworks.


Steering Committee Leadership: Chairing migration steering committees and delivering data-driven PMO dashboards and Go/No-Go recommendations.
Proactive Risk & Scope Management: Identifying early technical bottlenecks and scope deviations to cut project risks by 20% and protect budgets.
Cross-Platform & Vendor Alignment: Synchronizing dependencies across S/4HANA, Salesforce, and external technology partners under strict SLA/KPI governance.

Regulatory Compliance & SAP Basis Operations

Ensuring audit-ready change controls and high-availability infrastructure operations in strict pharmaceutical and enterprise environments.


CSV & SOX Compliance: Partnering with Computer System Validation (CSV) and audit teams to enforce structured, zero-disruption change controls.
Landscape Monitoring & Optimization: Establishing SAP Solution Manager OCC monitoring, LMDB governance, and Known Error Databases to reduce Total Cost of Ownership (TCO).
Global Service Transitions: Managing cross-border vendor transitions, technical knowledge transfer, and team upskilling across Europe, North America, and Asia.


Featured Case Studies


RISE with SAP Cloud Strategy & Zero-Downtime Upgrades (MSD)

High-availability pharmaceutical SAP landscapes required cloud modernisation and complex upgrades without disrupting regulated daily operations. I governed end-to-end SAP Basis infrastructure services across Azure and AWS, instituted formal toll-gate frameworks (Preparation, Realisation, Testing, Cutover), partnered with CSV teams on strict change controls, and engineered 24/7 cutover runbooks with Zero Downtime Option (ZDO) strategies.


Tools: RISE with SAP, Microsoft Azure, AWS, ZDO, CSV Governance, PMO Dashboards

Outcome: Delivered pre-S/4HANA projects under budget and ahead of schedule, reduced project risks by 20%, and increased stakeholder satisfaction scores by 15%.


Global Multi-Country SAP Rollout & Azure Cloud Migrations (IBM / Kyndryl)

Large-scale enterprise transformation programs required synchronized cutovers and cloud database migrations across complex, multi-platform landscapes. I directed full-lifecycle SAP delivery spanning 200+ SAP instances and 26 Production systems across the USA, Germany, UK, and India, leading a team of 10+ Delivery Leads and engineers across S/4HANA, RISE with SAP, and Salesforce workstreams.


Tools: Microsoft Azure, SAP S/4HANA, RISE with SAP, Agile/Waterfall, Salesforce Integration

Outcome: Consistently delivered global SAP rollouts under budget and ahead of schedule with seamless cross-platform go-lives.




03 — Projects & Frameworks
Delivery accelerators & governance frameworks
SAP S/4HANA Cutover Runbook & Toll-Gate Kit
Concept / Template


A standardised governance framework for enterprise SAP cloud migrations and upgrades designed to bring repeatability and audit readiness to high-stakes cutovers.


Key Features: Phase-by-phase toll-gate checklists (Preparation, Realisation, Testing, Cutover, Hypercare), 24/7 shift schedules, CSV/SOX sign-off gates, and technical rollback triggers.
Target Metrics: Zero unplanned business downtime and 20% reduction in cutover execution risks.


04 — Experience
Career timeline
SAP Technical Project Manager
Mar 2025 – Present

MSD · Czech Republic

Governing end-to-end SAP Basis infrastructure delivery, RISE with SAP cloud strategies on Azure/AWS, Zero Downtime Option (ZDO) upgrades, CSV-compliant change controls, 24/7 cutover runbooks, and executive steering committees.


RISE with SAP
Azure
AWS
ZDO
CSV Compliance
PMO Governance
Cutover Management

SAP Technical Project Manager
Sep 2017 – Oct 2024

IBM / Kyndryl · Czech Republic

Directed end-to-end SAP Basis projects, homogeneous/heterogeneous Azure cloud database migrations, and global transformation programs across RISE with SAP, S/4HANA, and Salesforce while leading a team of 10+ Delivery Leads and engineers.


Microsoft Azure
SAP S/4HANA
RISE with SAP
Agile & Waterfall
Global Rollouts
Team Leadership

Deputy Manager – SAP Basis
Feb 2016 – Jul 2017

Rieter India Pvt. Ltd. (Client: Rieter AG, Switzerland) · India & Switzerland
Certificate of Appreciation – RIETER Go INNOVATE (Jun 2016)

Led SAP Basis and database teams, executed AIX-to-Linux and SAP HANA migrations across 8 markets, rolled out 5 global SAP projects, established Solution Manager OCC monitoring, and led vendor transition from Itelligence AG in Germany.


SAP HANA
AIX to Linux
SAP Fiori
SLT Replication
Solution Manager 7.1
Vendor Transition

Team Lead – SAP Basis
Feb 2010 – Feb 2016

IBM India Pvt. Ltd. (Client: Johnson & Johnson) · India

Served as single point of contact for global SAP Basis delivery, vendor SLA governance, and SOX audit compliance across USA, UK, and Japan landscapes, executing SAP HANA installations on SUSE Linux, ECC on AIX/Oracle, and EHP upgrades.


SAP HANA
SUSE Linux
AIX
Oracle 11g
SOX Compliance
STMS
SLA Management



05 — Skills
Technical & program leadership stack
Project & Program Management

SAP Activate
PRINCE2®
Agile & Waterfall
PMO Governance
Steering Committee Reporting
Cutover & Release Management
Risk & Scope Control
RAID Logs
Vendor SLA/KPI Management

SAP Ecosystem

SAP S/4HANA
RISE with SAP
SAP ECC 6.0
SAP HANA
SAP BW
SAP NetWeaver
Solution Manager 7.1/7.2 (OCC, LMDB, SMSY)
SAP Fiori
SAP PI/PO
SAP BOBJ
SLT Replication
SUM
DMO
ZDO

Cloud, OS & Databases

Microsoft Azure
AWS
SUSE Linux (SLES)
Red Hat Enterprise Linux (RHEL)
IBM AIX
Oracle 11g
IBM DB2
Microsoft SQL Server

Compliance, Security & ITSM

Computer System Validation (CSV)
SOX Audit Readiness
ITIL® 4
Change & Incident Management
Root-Cause Analysis (RCA)
Disaster Recovery
Security Role Redesign
Known Error Database (KEDB)



06 — Credentials
Certifications, education & languages
Certifications


Expert / Practitioner
PRINCE2® Practitioner & Foundation


Specialist
SAP Certified Specialist – Project Manager - SAP Activate for Agile Implementation Management


Associate
SAP Certified Associate – Managing SAP S/4HANA Cloud Public Edition Projects


Foundation
ITIL® 4 Foundation (Badge verified on resume)


Education & Executive Training


2014
Executive MBA in Project Management


Undergraduate
Bachelor of Science (Electronics) – Nagpur University, Maharashtra, India


Executive Training
IT Project Management (Indian School of Business / Coursera) & Project Management Fundamentals MOOC (PMI)


Languages


English
Full Professional Proficiency


Hindi
Native / Bilingual


Czech
Elementary (A2)


Awards & Recognition


Jun 2016 · Rieter India Pvt. Ltd.
Certificate of Appreciation – RIETER Go INNOVATE




07 — Contact
Let's connect

Open to Senior Leadership roles in SAP Program Management, Cloud Transformation Governance, and Enterprise ERP Delivery across Europe and global markets.



Connect on LinkedIn

Back to Top



©  Abhishek Tiwari · SAP Technical Project Manager · Brno, Czech Republic

// Dynamic copyright year
document.getElementById('year').textContent = new Date().getFullYear();
// Mobile hamburger menu toggle
const menuToggle = document.getElementById('menuToggle');
const primaryNav = document.getElementById('primaryNav');
menuToggle.addEventListener('click', () => {
const isOpen = primaryNav.classList.toggle('open');
menuToggle.setAttribute('aria-expanded', isOpen);
});
// Close mobile menu when a nav link is clicked
primaryNav.querySelectorAll('a').forEach(link => {
link.addEventListener('click', () => {
primaryNav.classList.remove('open');
menuToggle.setAttribute('aria-expanded', 'false');
});
});
// Subtle fade-in-on-scroll observer
const prefersReducedMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
if (!prefersReducedMotion && 'IntersectionObserver' in window) {
const observer = new IntersectionObserver((entries, obs) => {
entries.forEach(entry => {
if (entry.isIntersecting) {
entry.target.classList.add('is-visible');
obs.unobserve(entry.target);
}
});
}, { threshold: 0.1 });
document.querySelectorAll('.reveal').forEach(el => observer.observe(el));
} else {
document.querySelectorAll('.reveal').forEach(el => el.classList.add('is-visible'));
}

