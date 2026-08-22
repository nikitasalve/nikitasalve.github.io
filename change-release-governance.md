---
layout: default
title: ITIL Change & Release Governance
---

<style>
.change-page {
  max-width: 1080px;
  margin: 0 auto;
  color: #172033;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
}

.change-hero {
  text-align: center;
  padding: 38px 20px 32px;
  border-bottom: 1px solid #e5e7eb;
}

.change-hero h1 {
  margin: 0 0 12px;
  font-size: 36px;
  letter-spacing: -0.5px;
}

.change-hero p {
  max-width: 720px;
  margin: auto;
  color: #64748b;
  font-size: 16px;
  line-height: 1.7;
}

.section {
  margin: 44px 0;
}

.section h2 {
  margin-bottom: 8px;
  font-size: 25px;
}

.section-intro {
  color: #64748b;
  line-height: 1.65;
  max-width: 800px;
}

/* Change lifecycle */

.change-flow {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 12px;
  margin-top: 30px;
}

.change-step {
  position: relative;
  text-align: center;
  padding: 22px 10px;
  background: #f8fafc;
  border: 1px solid #e2e8f0;
  border-radius: 12px;
}

.change-step:not(:last-child)::after {
  content: "→";
  position: absolute;
  right: -17px;
  top: 40px;
  color: #94a3b8;
  font-size: 20px;
  z-index: 2;
}

.step-number {
  display: inline-flex;
  width: 34px;
  height: 34px;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  background: #0f3b82;
  color: white;
  font-size: 13px;
  font-weight: 700;
}

.change-step h3 {
  margin: 11px 0 6px;
  font-size: 15px;
}

.change-step p {
  margin: 0;
  color: #64748b;
  font-size: 12px;
  line-height: 1.5;
}

/* Governance cards */

.governance-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 18px;
  margin-top: 25px;
}

.governance-card {
  padding: 25px;
  border: 1px solid #e2e8f0;
  border-radius: 14px;
  background: #ffffff;
}

.governance-card h3 {
  margin-top: 0;
  color: #0f3b82;
  font-size: 18px;
}

.governance-card ul {
  margin-bottom: 0;
  padding-left: 20px;
}

.governance-card li {
  margin: 7px 0;
  color: #64748b;
  font-size: 14px;
  line-height: 1.5;
}

/* Decision model */

.decision-model {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
  margin-top: 25px;
}

.decision-card {
  padding: 24px;
  border-radius: 14px;
  background: #f8fafc;
  border: 1px solid #e2e8f0;
}

.decision-card h3 {
  margin-top: 0;
  font-size: 18px;
}

.decision-card p {
  color: #64748b;
  font-size: 14px;
  line-height: 1.6;
}

/* Change table */

.change-table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 24px;
  font-size: 14px;
}

.change-table th,
.change-table td {
  padding: 14px 16px;
  border-bottom: 1px solid #e2e8f0;
  text-align: left;
}

.change-table th {
  background: #f8fafc;
  color: #172033;
}

.change-table td {
  color: #64748b;
}

/* Tool tags */

.tools {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 20px;
}

.tool {
  padding: 9px 15px;
  border: 1px solid #dbe4f0;
  border-radius: 20px;
  background: #f8fafc;
  color: #334155;
  font-size: 13px;
}

/* Closing statement */

.closing {
  margin-top: 45px;
  padding: 28px;
  border-left: 4px solid #0f3b82;
  background: #f8fafc;
}

.closing p {
  margin: 0;
  color: #475569;
  line-height: 1.7;
}

/* Responsive */

@media (max-width: 850px) {
  .change-flow {
    grid-template-columns: repeat(3, 1fr);
  }

  .change-step:not(:last-child)::after {
    display: none;
  }

  .governance-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 600px) {
  .change-flow,
  .decision-model {
    grid-template-columns: 1fr;
  }

  .change-hero h1 {
    font-size: 29px;
  }

  .change-table {
    display: block;
    overflow-x: auto;
  }
}
</style>

<div class="change-page">

<section class="change-hero">

<h1>ITIL Change &amp; Release Governance</h1>

<p>
  Governing production changes through structured assessment, risk management,
  approval, implementation and post-change review.
</p>

</section>


<section class="section">

<h2>Change Governance Lifecycle</h2>

<p class="section-intro">
  A controlled change lifecycle that supports safe and compliant production
  implementation within the broader release process.
</p>

<div class="change-flow">

<div class="change-step">
  <span class="step-number">01</span>
  <h3>Request</h3>
  <p>Scope &amp; impact</p>
</div>

<div class="change-step">
  <span class="step-number">02</span>
  <h3>Assess</h3>
  <p>Risk &amp; dependencies</p>
</div>

<div class="change-step">
  <span class="step-number">03</span>
  <h3>Plan</h3>
  <p>Implementation &amp; rollback</p>
</div>

<div class="change-step">
  <span class="step-number">04</span>
  <h3>Approve</h3>
  <p>CAB &amp; authorization</p>
</div>

<div class="change-step">
  <span class="step-number">05</span>
  <h3>Implement</h3>
  <p>Controlled execution</p>
</div>

<div class="change-step">
  <span class="step-number">06</span>
  <h3>Review</h3>
  <p>Validation &amp; closure</p>
</div>

</div>

</section>


<section class="section">

<h2>Release Manager Governance Areas</h2>

<p class="section-intro">
  Key areas of change governance involved in coordinating controlled
  production releases.
</p>

<div class="governance-grid">

<div class="governance-card">
<h3>01 · Risk &amp; Impact Assessment</h3>
<ul>
  <li>Review the scope and affected services</li>
  <li>Assess business and technical impact</li>
  <li>Identify dependencies and implementation risks</li>
  <li>Confirm appropriate mitigation actions</li>
</ul>
</div>

<div class="governance-card">
<h3>02 · Implementation Planning</h3>
<ul>
  <li>Review implementation approach</li>
  <li>Confirm deployment window and ownership</li>
  <li>Review validation activities</li>
  <li>Review rollback or backout strategy</li>
</ul>
</div>

<div class="governance-card">
<h3>03 · CAB &amp; Change Approval</h3>
<ul>
  <li>Coordinate required change approvals</li>
  <li>Prepare change information for governance review</li>
  <li>Track approval decisions</li>
  <li>Confirm approved implementation windows</li>
</ul>
</div>

<div class="governance-card">
<h3>04 · Implementation &amp; Closure</h3>
<ul>
  <li>Coordinate approved production implementation</li>
  <li>Track implementation progress</li>
  <li>Confirm post-implementation validation</li>
  <li>Support change closure and review</li>
</ul>
</div>

</div>

</section>


<section class="section">

<h2>Change Types</h2>

<div class="decision-model">

<div class="decision-card">
<h3>Normal Change</h3>
<p>
Planned production changes that undergo assessment, approval and scheduled
implementation.
</p>
</div>

<div class="decision-card">
<h3>Emergency Change</h3>
<p>
Urgent production changes requiring expedited assessment, authorization and
implementation coordination.
</p>
</div>

<div class="decision-card">
<h3>Release-Related Change</h3>
<p>
Production changes associated with an approved release and coordinated with
the overall release plan and deployment window.
</p>
</div>

</div>

</section>


<section class="section">

<h2>Change Risk Assessment</h2>

<p class="section-intro">
  Change risk is considered before implementation to support appropriate
  governance and deployment decisions.
</p>

<table class="change-table">

<thead>
<tr>
  <th>Assessment Area</th>
  <th>Key Considerations</th>
</tr>
</thead>

<tbody>

<tr>
  <td><strong>Business Impact</strong></td>
  <td>Customer, business process and service impact</td>
</tr>

<tr>
  <td><strong>Technical Impact</strong></td>
  <td>Applications, integrations, infrastructure and environments</td>
</tr>

<tr>
  <td><strong>Dependencies</strong></td>
  <td>Cross-team, application and deployment dependencies</td>
</tr>

<tr>
  <td><strong>Implementation</strong></td>
  <td>Deployment sequence, timing and execution requirements</td>
</tr>

<tr>
  <td><strong>Rollback</strong></td>
  <td>Backout approach and recovery considerations</td>
</tr>

<tr>
  <td><strong>Validation</strong></td>
  <td>Post-change technical and business validation</td>
</tr>

</tbody>

</table>

</section>


<section class="section">

<h2>Change &amp; Release Alignment</h2>

<div class="closing">

<p>
<strong>Release Management</strong> coordinates the overall release lifecycle,
while <strong>Change Management</strong> provides governance and control over
the production changes required to implement that release.
</p>

<br>

<p>
<strong>Release Plan → Change Assessment → Approval → Implementation →
Production Validation → Change Closure</strong>
</p>

</div>

</section>


<section class="section">

<h2>Tools &amp; Practices</h2>

<div class="tools">

<span class="tool">ServiceNow ITSM</span>
<span class="tool">ITIL V4</span>
<span class="tool">Change Management</span>
<span class="tool">CAB Governance</span>
<span class="tool">Risk Assessment</span>
<span class="tool">Azure DevOps</span>
<span class="tool">CI/CD</span>

</div>

</section>


<section class="section">

<h2>Release Manager Perspective</h2>

<p class="section-intro">
  Effective change governance ensures that production changes are assessed,
  approved, coordinated and implemented with appropriate risk and operational
  controls.
</p>

</section>

</div>
