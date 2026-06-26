---
title: Calm Focus Job Aid
layout: page
permalink: /courses/calm-focus/job-aid/
---

<style>
/* ── Screen styles ── */
.job-aid {
  max-width: 720px;
  margin: 0 auto;
  padding: 2rem 0 4rem;
}

.job-aid__header {
  border-bottom: 2px solid #7b68ee;
  padding-bottom: 1.5rem;
  margin-bottom: 2.5rem;
}

.job-aid__course {
  font-size: 0.78rem;
  font-weight: 600;
  letter-spacing: 0.09em;
  text-transform: uppercase;
  color: #a99ff5;
  margin-bottom: 0.5rem;
}

.job-aid__title {
  font-size: 1.75rem;
  font-weight: 700;
  letter-spacing: -0.03em;
  color: #eeeef5;
  margin-bottom: 0.25rem;
}

.job-aid__subtitle {
  font-size: 0.9rem;
  color: #9898b2;
}

.job-aid__print-btn {
  display: inline-block;
  margin-bottom: 2rem;
  padding: 0.5rem 1.25rem;
  background: rgba(123,104,238,0.12);
  border: 1px solid rgba(123,104,238,0.28);
  border-radius: 6px;
  font-size: 0.85rem;
  font-weight: 600;
  color: #a99ff5;
  cursor: pointer;
  letter-spacing: 0.02em;
}

.job-aid__print-btn:hover { background: rgba(123,104,238,0.2); color: #a99ff5; }

.ja-section {
  margin-bottom: 2.5rem;
  background: #14141f;
  border: 1px solid rgba(255,255,255,0.06);
  border-radius: 12px;
  overflow: hidden;
}

.ja-section__header {
  background: rgba(123,104,238,0.12);
  border-bottom: 1px solid rgba(123,104,238,0.2);
  padding: 0.875rem 1.5rem;
  display: flex;
  align-items: center;
  gap: 0.75rem;
}

.ja-section__number {
  width: 24px;
  height: 24px;
  background: #7b68ee;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 0.72rem;
  font-weight: 700;
  color: #fff;
  flex-shrink: 0;
}

.ja-section__title {
  font-size: 0.85rem;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #a99ff5;
  margin: 0;
}

.ja-section__body { padding: 1.5rem; }

.technique {
  margin-bottom: 1.5rem;
  padding-bottom: 1.5rem;
  border-bottom: 1px solid rgba(255,255,255,0.06);
}

.technique:last-child { margin-bottom: 0; padding-bottom: 0; border-bottom: none; }

.technique__name {
  font-size: 1rem;
  font-weight: 700;
  color: #eeeef5;
  margin-bottom: 0.75rem;
  letter-spacing: -0.01em;
}

.technique__steps {
  list-style: none;
  padding: 0;
  margin: 0 0 0.5rem;
}

.technique__steps li {
  display: flex;
  gap: 0.75rem;
  align-items: baseline;
  font-size: 0.9rem;
  color: #9898b2;
  margin-bottom: 0.375rem;
}

.technique__steps li::before {
  content: attr(data-step);
  width: 20px;
  height: 20px;
  background: rgba(123,104,238,0.15);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 0.68rem;
  font-weight: 700;
  color: #a99ff5;
  flex-shrink: 0;
}

.technique__tip {
  font-size: 0.825rem;
  color: #52526a;
  font-style: italic;
}

.boundary-question {
  font-size: 0.9rem;
  color: #9898b2;
  margin-bottom: 0.3rem;
  padding-left: 1rem;
  border-left: 2px solid rgba(123,104,238,0.3);
}

.boundary-responses { margin-top: 1.25rem; }

.boundary-response {
  background: rgba(255,255,255,0.03);
  border: 1px solid rgba(255,255,255,0.06);
  border-radius: 8px;
  padding: 0.75rem 1rem;
  font-size: 0.875rem;
  color: #9898b2;
  margin-bottom: 0.625rem;
  font-style: italic;
}

.checklist { list-style: none; padding: 0; margin: 0 0 1.25rem; }

.checklist li {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  font-size: 0.925rem;
  color: #9898b2;
  padding: 0.625rem 0;
  border-bottom: 1px solid rgba(255,255,255,0.04);
}

.checklist li:last-child { border-bottom: none; }

.checklist input[type="checkbox"] {
  width: 18px;
  height: 18px;
  accent-color: #7b68ee;
  flex-shrink: 0;
  cursor: pointer;
}

.ja-note {
  font-size: 0.825rem;
  color: #52526a;
  font-style: italic;
  border-left: 2px solid rgba(123,104,238,0.3);
  padding-left: 1rem;
  margin-top: 0.5rem;
}

.ja-back {
  display: inline-block;
  font-size: 0.85rem;
  color: #52526a;
  margin-top: 1rem;
}

.ja-back:hover { color: #9898b2; }

/* ── Print styles ── */
@media print {
  .site-header,
  .site-footer,
  .job-aid__print-btn,
  .ja-back { display: none !important; }

  body, .site-main { background: #fff !important; }

  .job-aid {
    max-width: 100%;
    padding: 0;
  }

  .job-aid__header { border-bottom: 2px solid #7b68ee; }
  .job-aid__course { color: #7b68ee; }
  .job-aid__title { color: #111; }
  .job-aid__subtitle { color: #555; }

  .ja-section {
    background: #fff;
    border: 1px solid #ddd;
    border-radius: 8px;
    break-inside: avoid;
    margin-bottom: 1.25rem;
  }

  .ja-section__header { background: #f3f1fe; border-bottom: 1px solid #d5cff9; }
  .ja-section__number { background: #7b68ee; }
  .ja-section__title { color: #4a38cc; }

  .technique__name { color: #111; }
  .technique__steps li { color: #333; }
  .technique__steps li::before { background: #f3f1fe; color: #4a38cc; }
  .technique__tip { color: #777; }
  .technique { border-bottom-color: #eee; }

  .boundary-question { color: #333; border-left-color: #a99ff5; }
  .boundary-response { background: #f9f9f9; border-color: #eee; color: #333; }

  .checklist li { color: #333; border-bottom-color: #eee; }
  .ja-note { color: #777; border-left-color: #a99ff5; }
}
</style>

<div class="job-aid">

  <div class="job-aid__header">
    <div class="job-aid__course">Calm Focus</div>
    <h1 class="job-aid__title">Stress Management Quick Reference</h1>
    <div class="job-aid__subtitle">Keep this handy for your next stressful moment.</div>
  </div>

  <button class="job-aid__print-btn" onclick="window.print()">⬇ Save as PDF / Print</button>

  <!-- Section 1 -->
  <div class="ja-section">
    <div class="ja-section__header">
      <div class="ja-section__number">1</div>
      <h2 class="ja-section__title">In-the-Moment Techniques</h2>
    </div>
    <div class="ja-section__body">

      <div class="technique">
        <div class="technique__name">Box Breathing</div>
        <ul class="technique__steps">
          <li data-step="1">Inhale slowly for 4 counts</li>
          <li data-step="2">Hold for 4 counts</li>
          <li data-step="3">Exhale slowly for 4 counts</li>
          <li data-step="4">Hold for 4 counts</li>
          <li data-step="5">Repeat 4 times</li>
        </ul>
        <div class="technique__tip">Tip: works anywhere — at your desk, before a meeting, between tasks.</div>
      </div>

      <div class="technique">
        <div class="technique__name">The 20-20-20 Rule</div>
        <ul class="technique__steps">
          <li data-step="1">Every 20 minutes of screen time</li>
          <li data-step="2">Look at something 20 feet away</li>
          <li data-step="3">Hold your gaze for 20 seconds</li>
        </ul>
        <div class="technique__tip">Tip: set a recurring timer or use a screen break app to build the habit.</div>
      </div>

      <div class="technique">
        <div class="technique__name">Movement Break</div>
        <ul class="technique__steps">
          <li data-step="1">Step away from your screen completely</li>
          <li data-step="2">Try shoulder rolls, neck stretches, or a short walk</li>
          <li data-step="3">Aim for at least 2–3 minutes</li>
        </ul>
        <div class="technique__tip">Tip: pair it with a natural pause — after a meeting or before switching tasks.</div>
      </div>

    </div>
  </div>

  <!-- Section 2 -->
  <div class="ja-section">
    <div class="ja-section__header">
      <div class="ja-section__number">2</div>
      <h2 class="ja-section__title">Boundary Response Guide</h2>
    </div>
    <div class="ja-section__body">

      <p style="font-size:0.875rem;color:#9898b2;margin-bottom:1rem;">When an after-hours request arrives, pause and ask yourself:</p>

      <div class="boundary-question">Is this a genuine emergency?</div>
      <div class="boundary-question">What is the actual consequence of waiting until tomorrow?</div>
      <div class="boundary-question">Am I responding from obligation or from choice?</div>

      <div class="boundary-responses">
        <p style="font-size:0.78rem;font-weight:700;letter-spacing:0.06em;text-transform:uppercase;color:#52526a;margin-bottom:0.75rem;">Ready responses</p>
        <div class="boundary-response">"I'm signing off for the day — I'll look at this first thing tomorrow."</div>
        <div class="boundary-response">"Happy to help. I'll have eyes on it by [time] tomorrow morning."</div>
        <div class="boundary-response">"This sounds important. Is there someone who can support tonight?"</div>
      </div>

    </div>
  </div>

  <!-- Section 3 -->
  <div class="ja-section">
    <div class="ja-section__header">
      <div class="ja-section__number">3</div>
      <h2 class="ja-section__title">Evening Ritual Checklist</h2>
    </div>
    <div class="ja-section__body">

      <p style="font-size:0.875rem;color:#9898b2;margin-bottom:1rem;">Choose at least 3 elements to build your end-of-day ritual. Do them in the same order each day.</p>

      <ul class="checklist">
        <li><input type="checkbox"> Close the laptop with intention</li>
        <li><input type="checkbox"> Write tomorrow's top three tasks</li>
        <li><input type="checkbox"> Change out of work clothes</li>
        <li><input type="checkbox"> Take a short walk</li>
        <li><input type="checkbox"> Turn off Slack notifications</li>
        <li><input type="checkbox"> Make a cup of tea</li>
      </ul>

      <div class="ja-note">Your ritual is a signal to your brain that work is done. The specific elements matter less than doing them consistently.</div>

    </div>
  </div>

  <a href="/courses/calm-focus/project-background/" class="ja-back">← Back to Project Background</a>

</div>
