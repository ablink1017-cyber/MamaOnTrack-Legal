<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MamaOnTrack — Legal & Privacy</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,600;1,400;1,600&family=DM+Sans:wght@300;400;500&display=swap">
<style>
  :root {
    --terra:   #b5836a;
    --dark:    #1a1a1a;
    --linen:   #faf8f5;
    --white:   #ffffff;
    --border:  #e8e2db;
    --muted:   #8a8480;
    --green:   #7a9e87;
    --purple:  #8f8aa0;
    --blue:    #7a96a8;
    --yellow:  #c9a96e;
    --coral:   #c0614a;
    --teal:    #6a9e96;
  }

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--linen);
    color: var(--dark);
    line-height: 1.7;
    font-size: 15px;
  }

  /* ── HEADER ── */
  header {
    background: var(--dark);
    padding: 28px 40px 22px;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 100;
    border-bottom: 3px solid var(--terra);
  }

  .header-logo {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 36px;
    color: #f0ece4;
    letter-spacing: 0.01em;
    line-height: 1;
  }

  .header-sub {
    font-size: 10px;
    color: rgba(240,236,228,0.4);
    letter-spacing: 0.2em;
    text-transform: uppercase;
    margin-top: 6px;
  }

  /* ── NAV ── */
  nav {
    background: var(--linen);
    border-bottom: 1px solid var(--border);
    padding: 0;
    display: flex;
    justify-content: center;
    gap: 0;
    overflow-x: auto;
    position: sticky;
    top: 95px;
    z-index: 99;
    flex-wrap: wrap;
  }

  nav a {
    padding: 14px 20px;
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--muted);
    text-decoration: none;
    border-bottom: 2px solid transparent;
    white-space: nowrap;
    transition: all 0.2s;
  }

  nav a:hover, nav a.active {
    color: var(--terra);
    border-bottom-color: var(--terra);
  }

  /* ── LAYOUT ── */
  .page { display: none; }
  .page.active { display: block; }

  .page-hero {
    background: var(--dark);
    padding: 60px 40px 48px;
    text-align: center;
    border-bottom: 3px solid var(--terra);
  }

  .page-hero h1 {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-weight: 400;
    font-size: 52px;
    color: #f0ece4;
    margin-bottom: 10px;
  }

  .page-hero p {
    font-size: 13px;
    color: rgba(240,236,228,0.45);
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  .page-content {
    max-width: 780px;
    margin: 0 auto;
    padding: 52px 40px 80px;
  }

  /* ── SECTIONS ── */
  .section {
    margin-bottom: 48px;
    padding-bottom: 48px;
    border-bottom: 1px solid var(--border);
  }

  .section:last-child { border-bottom: none; }

  .section h2 {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-weight: 400;
    font-size: 30px;
    color: var(--dark);
    margin-bottom: 16px;
    padding-bottom: 10px;
    border-bottom: 1px solid var(--border);
  }

  .section h3 {
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--terra);
    margin: 24px 0 10px;
  }

  .section p {
    color: var(--dark);
    margin-bottom: 14px;
    line-height: 1.85;
    font-size: 14px;
  }

  .section ul {
    padding-left: 0;
    list-style: none;
    margin-bottom: 14px;
  }

  .section ul li {
    padding: 6px 0 6px 18px;
    position: relative;
    font-size: 14px;
    line-height: 1.7;
    color: var(--dark);
    border-bottom: 1px solid var(--border);
  }

  .section ul li:last-child { border-bottom: none; }

  .section ul li::before {
    content: '';
    position: absolute;
    left: 0;
    top: 14px;
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: var(--terra);
  }

  /* ── PROMISE BADGES ── */
  .badge-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 12px;
    margin: 20px 0;
  }

  .badge {
    background: var(--white);
    border: 1px solid var(--border);
    border-left: 3px solid var(--green);
    border-radius: 6px;
    padding: 14px 16px;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .badge-dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    background: var(--green);
    flex-shrink: 0;
  }

  .badge span {
    font-size: 13px;
    color: var(--dark);
    font-weight: 400;
  }

  /* ── HIGHLIGHT BOX ── */
  .highlight {
    background: var(--white);
    border: 1px solid var(--border);
    border-left: 3px solid var(--terra);
    border-radius: 6px;
    padding: 20px 24px;
    margin: 20px 0;
  }

  .highlight p { margin-bottom: 0; }

  /* ── TABLE ── */
  .data-table {
    width: 100%;
    border-collapse: collapse;
    margin: 16px 0;
    font-size: 13px;
  }

  .data-table th {
    background: var(--dark);
    color: #f0ece4;
    padding: 10px 14px;
    text-align: left;
    font-size: 10px;
    font-weight: 400;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    border-bottom: 2px solid var(--terra);
  }

  .data-table td {
    padding: 10px 14px;
    border-bottom: 1px solid var(--border);
    vertical-align: top;
    line-height: 1.6;
  }

  .data-table tr:nth-child(even) td { background: var(--linen); }

  /* ── CONTACT CARD ── */
  .contact-card {
    background: var(--white);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 28px 32px;
    text-align: center;
    margin-top: 24px;
  }

  .contact-card h3 {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-weight: 400;
    font-size: 26px;
    color: var(--terra);
    letter-spacing: 0;
    text-transform: none;
    margin-bottom: 8px;
  }

  .contact-card p { color: var(--muted); font-size: 13px; margin-bottom: 16px; }

  .contact-link {
    display: inline-block;
    padding: 10px 28px;
    background: var(--terra);
    color: var(--white);
    border-radius: 4px;
    text-decoration: none;
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    transition: opacity 0.2s;
  }

  .contact-link:hover { opacity: 0.85; }

  /* ── FOOTER ── */
  footer {
    background: var(--dark);
    padding: 40px;
    text-align: center;
  }

  .footer-logo {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 28px;
    color: #f0ece4;
    margin-bottom: 8px;
  }

  .footer-links {
    display: flex;
    gap: 24px;
    justify-content: center;
    flex-wrap: wrap;
    margin: 16px 0;
  }

  .footer-links a {
    font-size: 11px;
    color: rgba(240,236,228,0.45);
    text-decoration: none;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    cursor: pointer;
    transition: color 0.2s;
  }

  .footer-links a:hover { color: var(--terra); }

  .footer-copy {
    font-size: 11px;
    color: rgba(240,236,228,0.25);
    margin-top: 16px;
    letter-spacing: 0.04em;
  }

  /* ── EFFECTIVE DATE ── */
  .eff-date {
    display: inline-block;
    font-size: 10px;
    color: var(--terra);
    letter-spacing: 0.1em;
    text-transform: uppercase;
    border: 1px solid var(--terra);
    border-radius: 20px;
    padding: 4px 14px;
    margin-bottom: 32px;
  }

  /* ── MOBILE ── */
  @media (max-width: 600px) {
    header { padding: 20px 20px 16px; }
    .header-logo { font-size: 28px; }
    nav { padding: 0 16px; }
    nav a { padding: 12px 12px; font-size: 10px; }
    .page-hero { padding: 40px 20px 32px; }
    .page-hero h1 { font-size: 36px; }
    .page-content { padding: 32px 20px 60px; }
    .badge-grid { grid-template-columns: 1fr; }
  }
</style>
</head>
<body>

<header>
  <div class="header-logo">MamaOnTrack</div>
  <div class="header-sub">Built by a nurse mom, for every mom</div>
</header>

<nav>
  <a href="#" class="active" onclick="show('privacy')">Privacy Policy</a>
  <a href="#" onclick="show('terms')">Terms of Service</a>
  <a href="#" onclick="show('hipaa')">HIPAA Notice</a>
  <a href="#" onclick="show('cookie')">Cookie Policy</a>
  <a href="#" onclick="show('contact')">Contact Us</a>
</nav>

<!-- ══════════════════════════════════════════
     PRIVACY POLICY
══════════════════════════════════════════ -->
<div class="page active" id="privacy">
  <div class="page-hero">
    <h1>Privacy Policy</h1>
    <p>Effective Date: May 19, 2026 &nbsp;&middot;&nbsp; Last Updated: May 19, 2026</p>
  </div>
  <div class="page-content">
    <div class="eff-date">Effective: May 19, 2026</div>

    <div class="section">
      <h2>Our Privacy Promise</h2>
      <p>MamaOnTrack was built by a nurse and mother of three. We understand that the information you store here — your child's health history, your postpartum journey, your family's medical records — is among the most personal data that exists. We treat it that way.</p>
      <div class="badge-grid">
        <div class="badge"><div class="badge-dot"></div><span>Your data is never sold</span></div>
        <div class="badge"><div class="badge-dot"></div><span>No advertising — ever</span></div>
        <div class="badge"><div class="badge-dot"></div><span>No third-party trackers</span></div>
        <div class="badge"><div class="badge-dot"></div><span>Encrypted in transit and at rest</span></div>
        <div class="badge"><div class="badge-dot"></div><span>You own your data</span></div>
        <div class="badge"><div class="badge-dot"></div><span>Delete your account anytime</span></div>
      </div>
    </div>

    <div class="section">
      <h2>Information We Collect</h2>
      <h3>Information you provide</h3>
      <ul>
        <li>Account information — name, email address, and encrypted password</li>
        <li>Children's profiles — names, dates of birth, blood type</li>
        <li>Health records — symptoms, medications, vaccines, growth data, vitals, labs, allergies, milestones, visits, and all other entries you log</li>
        <li>Maternal health data — feeding sessions, pumping logs, hydration, nutrition, mood, sleep, cycle, and postpartum health entries</li>
        <li>Family calendar events — dates, times, titles, locations, and notes</li>
        <li>AI feature inputs — documents or images you upload to the Visit Scanner (processed in real time and never stored)</li>
      </ul>

      <h3>Information collected automatically</h3>
      <ul>
        <li>Device type and operating system (for compatibility)</li>
        <li>App version and crash reports (for bug fixing)</li>
        <li>Anonymous, aggregated usage patterns (to improve features — never tied to your identity)</li>
      </ul>

      <h3>Information we do NOT collect</h3>
      <ul>
        <li>Your location</li>
        <li>Your contacts or address book</li>
        <li>Your camera roll or photo library beyond images you explicitly upload</li>
        <li>Your microphone</li>
        <li>Any data from other apps on your device</li>
      </ul>
    </div>

    <div class="section">
      <h2>How We Use Your Information</h2>
      <table class="data-table">
        <thead><tr><th>Purpose</th><th>Data Used</th><th>Legal Basis</th></tr></thead>
        <tbody>
          <tr><td>Providing the app and its features</td><td>All data you enter</td><td>Contract performance</td></tr>
          <tr><td>Authentication and account security</td><td>Email, password hash</td><td>Legitimate interest</td></tr>
          <tr><td>AI feature processing (Sleep Planner, Visit Scanner)</td><td>Data you submit for AI processing</td><td>Consent (provided at time of use)</td></tr>
          <tr><td>Sending reminders and notifications</td><td>Health data, events, your preferences</td><td>Consent (opt-in)</td></tr>
          <tr><td>Improving the app</td><td>Anonymous, aggregated usage data only</td><td>Legitimate interest</td></tr>
          <tr><td>Customer support</td><td>Information relevant to your request</td><td>Contract performance</td></tr>
        </tbody>
      </table>
    </div>

    <div class="section">
      <h2>What We Will Never Do</h2>
      <ul>
        <li><strong>Sell your data</strong> — Your health data, your children's records, and your personal information will never be sold to any third party, not advertisers, not data brokers, not anyone.</li>
        <li><strong>Show you advertisements</strong> — MamaOnTrack is 100% ad-free on every plan. We do not use ad networks, ad SDKs, or behavioral targeting of any kind.</li>
        <li><strong>Share with insurers or employers</strong> — Your health information is never shared with insurance companies, employers, or government entities without your explicit written consent or a legal requirement.</li>
        <li><strong>Use your data to train AI models</strong> — Your personal entries and health records are never used to train artificial intelligence models.</li>
        <li><strong>Access your data without permission</strong> — Our team does not access individual user records except when explicitly required to resolve a support issue you have reported, with your consent.</li>
      </ul>
    </div>

    <div class="section">
      <h2>Data Sharing</h2>
      <p>We share your data only in the following limited circumstances:</p>
      <h3>Service providers</h3>
      <p>We use Supabase for secure database hosting and authentication. These providers process data only on our behalf and are contractually prohibited from using it for any other purpose.</p>
      <h3>AI processing</h3>
      <p>When you use the AI Sleep Planner or Visit Scanner, anonymized data is sent securely to Anthropic's Claude API. This data is not stored by Anthropic beyond the immediate request and is never used to train AI models.</p>
      <h3>Family access</h3>
      <p>If you invite caregivers through the Family Access feature, they can view data according to the role you assign them. You control this at all times and can revoke access instantly.</p>
      <h3>Legal requirements</h3>
      <p>We may disclose information if required by law, court order, or to protect the safety of any person. We will notify you of any such request to the extent permitted by law.</p>
    </div>

    <div class="section">
      <h2>Data Security</h2>
      <ul>
        <li><strong>Encryption in transit</strong> — All data sent between your device and our servers is encrypted using TLS 1.3</li>
        <li><strong>Encryption at rest</strong> — All data stored in our database is encrypted at rest using AES-256</li>
        <li><strong>Password security</strong> — Passwords are never stored in plain text. We use bcrypt hashing with salt</li>
        <li><strong>Row Level Security</strong> — Database access is enforced at the row level so users can only access their own family's data</li>
        <li><strong>Regular security audits</strong> — We conduct regular reviews of our security practices</li>
      </ul>
    </div>

    <div class="section">
      <h2>Your Rights</h2>
      <ul>
        <li><strong>Access</strong> — Request a copy of all data we hold about you and your family</li>
        <li><strong>Correction</strong> — Edit or correct any information at any time directly in the app</li>
        <li><strong>Deletion</strong> — Delete your account and all associated data permanently at any time. Deletion is immediate and irreversible</li>
        <li><strong>Portability</strong> — Export your health data in a portable format (Premium feature)</li>
        <li><strong>Withdraw consent</strong> — Revoke caregiver access at any time from the Family Access tab</li>
        <li><strong>Opt out of notifications</strong> — Disable any or all reminders from the Reminders tab at any time</li>
      </ul>
      <p>To exercise any of these rights, contact us at <strong>privacy@mamaontrack.com</strong>. We respond within 48 hours.</p>
    </div>

    <div class="section">
      <h2>Children's Privacy</h2>
      <p>MamaOnTrack is designed for use by parents and caregivers to track their children's health. The app is not directed at children and children do not create accounts. All children's health data is entered and controlled by a parent or guardian account holder.</p>
      <p>We comply with the Children's Online Privacy Protection Act (COPPA). If you believe we have inadvertently collected information from a child under 13 who has created their own account, please contact us immediately at privacy@mamaontrack.com.</p>
    </div>

    <div class="section">
      <h2>Changes to This Policy</h2>
      <p>We will notify you of any material changes to this Privacy Policy by email and through an in-app notification at least 30 days before changes take effect. Your continued use of the app after that date constitutes acceptance of the updated policy.</p>
      <p>For minor changes (such as clarifications), we will update the "Last Updated" date at the top of this page.</p>
    </div>

    <div class="section">
      <h2>Contact</h2>
      <div class="contact-card">
        <h3>Privacy Questions?</h3>
        <p>We respond to all privacy inquiries within 48 hours.</p>
        <a href="mailto:privacy@mamaontrack.com" class="contact-link">privacy@mamaontrack.com</a>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════
     TERMS OF SERVICE
══════════════════════════════════════════ -->
<div class="page" id="terms">
  <div class="page-hero">
    <h1>Terms of Service</h1>
    <p>Effective Date: May 19, 2026 &nbsp;&middot;&nbsp; Last Updated: May 19, 2026</p>
  </div>
  <div class="page-content">
    <div class="eff-date">Effective: May 19, 2026</div>

    <div class="section">
      <h2>Agreement to Terms</h2>
      <p>By downloading, installing, or using MamaOnTrack ("the App"), you agree to be bound by these Terms of Service ("Terms"). If you do not agree to these Terms, do not use the App.</p>
      <p>These Terms constitute a legally binding agreement between you and MamaOnTrack ("we," "us," or "our"). Please read them carefully.</p>
    </div>

    <div class="section">
      <h2>Description of Service</h2>
      <p>MamaOnTrack is a health tracking application designed for parents and caregivers to track their children's health information and their own maternal health. The App provides tools for logging health data, scheduling, and receiving AI-generated health insights.</p>
      <div class="highlight">
        <p><strong>Important:</strong> MamaOnTrack is a tracking and organizational tool only. It is NOT a medical device, does not provide medical advice, and is not a substitute for professional medical care. Always consult a qualified healthcare provider for medical decisions.</p>
      </div>
    </div>

    <div class="section">
      <h2>Eligibility</h2>
      <p>You must be at least 18 years old to create an account and use MamaOnTrack. By using the App, you represent and warrant that you are 18 years of age or older and have the legal capacity to enter into these Terms.</p>
    </div>

    <div class="section">
      <h2>Account Registration</h2>
      <ul>
        <li>You must provide accurate, current, and complete information when creating your account</li>
        <li>You are responsible for maintaining the confidentiality of your account credentials</li>
        <li>You are responsible for all activity that occurs under your account</li>
        <li>You must notify us immediately of any unauthorized use of your account</li>
        <li>You may not share your account with others or create accounts for third parties without their consent</li>
      </ul>
    </div>

    <div class="section">
      <h2>Subscription Plans and Billing</h2>
      <h3>Free Plan</h3>
      <p>The Free plan is available at no cost and provides access to core tracking features for one child. The Free plan is free forever with no automatic conversion to a paid plan.</p>
      <h3>Premium Monthly</h3>
      <p>Premium Monthly is billed at $6.99 per month. Your subscription will automatically renew each month until you cancel. You may cancel at any time from your account settings or through the App Store / Google Play.</p>
      <h3>Premium Lifetime</h3>
      <p>Lifetime access is available for a one-time payment of $49.99. This grants permanent access to all Premium features including all future updates, with no recurring charges.</p>
      <h3>Refund Policy</h3>
      <p>Monthly subscriptions canceled within 7 days of the initial purchase are eligible for a full refund. After 7 days, monthly subscriptions are non-refundable for the current billing period. Lifetime purchases are non-refundable after 14 days. Refund requests should be submitted to support@mamaontrack.com.</p>
      <h3>Price Changes</h3>
      <p>We reserve the right to change subscription prices with 30 days notice. Existing subscribers will be notified by email before any price change takes effect.</p>
    </div>

    <div class="section">
      <h2>Acceptable Use</h2>
      <p>You agree to use MamaOnTrack only for lawful purposes. You may not:</p>
      <ul>
        <li>Use the App to store or transmit information that is unlawful, harmful, or violates any third-party rights</li>
        <li>Attempt to gain unauthorized access to any part of the App or its systems</li>
        <li>Reverse engineer, decompile, or disassemble any part of the App</li>
        <li>Use the App for any commercial purpose without our prior written consent</li>
        <li>Impersonate any person or entity or falsely represent your affiliation with any person or entity</li>
        <li>Upload or transmit viruses or any other malicious code</li>
        <li>Interfere with or disrupt the integrity or performance of the App</li>
      </ul>
    </div>

    <div class="section">
      <h2>Health Information Disclaimer</h2>
      <p>The information provided in MamaOnTrack is for general tracking and organizational purposes only. Content informed by medical professionals and current evidence-based guidelines is provided for educational purposes only and does not constitute medical advice.</p>
      <p>MamaOnTrack is not a medical device and has not been evaluated by the U.S. Food and Drug Administration (FDA). Do not use the App as a substitute for professional medical advice, diagnosis, or treatment.</p>
      <p>Always seek the advice of your physician, pediatrician, or other qualified healthcare provider with any questions regarding a medical condition. If you believe you or your child are experiencing a medical emergency, call 911 immediately.</p>
    </div>

    <div class="section">
      <h2>AI Features</h2>
      <p>MamaOnTrack includes AI-powered features including the Sleep Planner and Visit Scanner. These features are powered by third-party AI services and are provided as organizational tools only.</p>
      <ul>
        <li>AI-generated sleep plans are based on published pediatric sleep guidelines and are not medical prescriptions</li>
        <li>AI-extracted visit information should always be reviewed and verified by you before saving</li>
        <li>AI features are provided on an "as available" basis and may not always produce accurate results</li>
        <li>We are not responsible for decisions made based on AI-generated content</li>
      </ul>
    </div>

    <div class="section">
      <h2>Intellectual Property</h2>
      <p>MamaOnTrack, including its name, logo, design, features, and content created by us, is owned by MamaOnTrack and protected by copyright, trademark, and other intellectual property laws.</p>
      <p>You retain ownership of all health data and content you enter into the App. By using the App, you grant us a limited license to store, process, and display your data solely for the purpose of providing the service to you.</p>
    </div>

    <div class="section">
      <h2>Family Access and Caregiver Accounts</h2>
      <p>The Family Access feature allows you to invite caregivers to view or contribute to your family's health records. You are responsible for:</p>
      <ul>
        <li>Ensuring that any caregiver you invite consents to having their information shared</li>
        <li>Assigning appropriate access roles to caregivers</li>
        <li>Revoking access from caregivers who should no longer have it</li>
        <li>Any actions taken by caregivers under your family account</li>
      </ul>
    </div>

    <div class="section">
      <h2>Termination</h2>
      <p>You may terminate your account at any time by deleting your account from within the App. Termination will result in the permanent deletion of all your data.</p>
      <p>We reserve the right to suspend or terminate your account if you violate these Terms. We will provide notice before termination except in cases of serious violations.</p>
    </div>

    <div class="section">
      <h2>Limitation of Liability</h2>
      <p>To the maximum extent permitted by law, MamaOnTrack shall not be liable for any indirect, incidental, special, consequential, or punitive damages arising from your use of the App.</p>
      <p>Our total liability to you for any claims arising from these Terms or your use of the App shall not exceed the amount you paid to us in the 12 months preceding the claim.</p>
    </div>

    <div class="section">
      <h2>Governing Law</h2>
      <p>These Terms are governed by the laws of the United States. Any disputes arising from these Terms shall be resolved through binding arbitration in accordance with the American Arbitration Association's rules, except that either party may seek injunctive relief in a court of competent jurisdiction.</p>
    </div>

    <div class="section">
      <h2>Changes to Terms</h2>
      <p>We may update these Terms from time to time. We will notify you of material changes by email and through an in-app notification at least 30 days before the changes take effect. Your continued use of the App after that date constitutes acceptance of the updated Terms.</p>
    </div>

    <div class="section">
      <h2>Contact</h2>
      <div class="contact-card">
        <h3>Questions about our Terms?</h3>
        <p>We are happy to clarify anything.</p>
        <a href="mailto:legal@mamaontrack.com" class="contact-link">legal@mamaontrack.com</a>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════
     HIPAA NOTICE
══════════════════════════════════════════ -->
<div class="page" id="hipaa">
  <div class="page-hero">
    <h1>HIPAA Notice</h1>
    <p>Notice of Privacy Practices &nbsp;&middot;&nbsp; Effective: May 19, 2026</p>
  </div>
  <div class="page-content">
    <div class="eff-date">Effective: May 19, 2026</div>

    <div class="section">
      <h2>Important Notice About HIPAA</h2>
      <div class="highlight">
        <p><strong>MamaOnTrack is a personal health record (PHR) application.</strong> As a PHR app used directly by consumers to manage their own health information, MamaOnTrack operates differently from covered healthcare entities under HIPAA.</p>
        <p style="margin-top:10px;">However, we take the privacy of your health information with the same seriousness as HIPAA-covered entities, and we voluntarily apply HIPAA-aligned practices to the handling of all health data in our App.</p>
      </div>
    </div>

    <div class="section">
      <h2>What Health Information We Handle</h2>
      <p>MamaOnTrack stores health-related information that you voluntarily enter, including:</p>
      <ul>
        <li>Children's medical history, symptoms, medications, vaccines, allergies, and vitals</li>
        <li>Maternal health information including postpartum recovery, feeding, nutrition, mood, and cycle data</li>
        <li>Doctor visit records and after-visit summaries you upload</li>
        <li>Growth measurements and developmental milestone records</li>
        <li>Laboratory results and vital signs</li>
      </ul>
    </div>

    <div class="section">
      <h2>How We Protect Your Health Information</h2>
      <ul>
        <li><strong>Technical safeguards</strong> — AES-256 encryption at rest, TLS 1.3 encryption in transit, row-level security in our database</li>
        <li><strong>Access controls</strong> — Only you and the caregivers you explicitly authorize can access your family's health data</li>
        <li><strong>Audit logs</strong> — We maintain records of who has accessed health data and when</li>
        <li><strong>Minimal access</strong> — Our staff does not access your health records except to resolve a support issue you have reported, with your consent</li>
        <li><strong>Secure deletion</strong> — When you delete your account or specific records, that data is permanently and irreversibly removed</li>
        <li><strong>Business associate agreements</strong> — We maintain appropriate agreements with all service providers who may process health data on our behalf</li>
      </ul>
    </div>

    <div class="section">
      <h2>Your Rights Regarding Health Information</h2>
      <ul>
        <li><strong>Right to access</strong> — You can view all health information stored in your account at any time within the App</li>
        <li><strong>Right to export</strong> — You can export your health records in a portable format (Premium feature)</li>
        <li><strong>Right to correct</strong> — You can edit or delete any health record at any time</li>
        <li><strong>Right to delete</strong> — You can permanently delete your account and all associated health data at any time</li>
        <li><strong>Right to restrict sharing</strong> — You control exactly who has access to your family's health information through the Family Access settings</li>
      </ul>
    </div>

    <div class="section">
      <h2>When We May Share Health Information</h2>
      <p>We will only share your health information in the following circumstances:</p>
      <ul>
        <li><strong>With your explicit consent</strong> — such as when you invite a caregiver through Family Access</li>
        <li><strong>For AI processing</strong> — when you use AI features, relevant data is sent securely to our AI provider. This is disclosed at the time of use and requires your consent.</li>
        <li><strong>As required by law</strong> — if compelled by a valid court order or applicable law</li>
        <li><strong>To protect safety</strong> — if we have a good-faith belief that disclosure is necessary to prevent serious harm</li>
      </ul>
      <p>We will <strong>never</strong> share your health information for marketing, advertising, or commercial purposes.</p>
    </div>

    <div class="section">
      <h2>Breach Notification</h2>
      <p>In the unlikely event of a data breach affecting your health information, we will notify you within 72 hours of discovering the breach. Notification will be provided by email and through an in-app alert, and will include:</p>
      <ul>
        <li>A description of what happened</li>
        <li>What information was involved</li>
        <li>Steps we are taking in response</li>
        <li>Steps you can take to protect yourself</li>
        <li>Contact information for questions</li>
      </ul>
    </div>

    <div class="section">
      <h2>Contact Our Privacy Officer</h2>
      <div class="contact-card">
        <h3>Privacy Officer</h3>
        <p>For questions about how we handle your health information or to exercise any of your rights, contact our Privacy Officer.</p>
        <a href="mailto:privacy@mamaontrack.com" class="contact-link">privacy@mamaontrack.com</a>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════
     COOKIE POLICY
══════════════════════════════════════════ -->
<div class="page" id="cookie">
  <div class="page-hero">
    <h1>Cookie Policy</h1>
    <p>Effective Date: May 19, 2026 &nbsp;&middot;&nbsp; Last Updated: May 19, 2026</p>
  </div>
  <div class="page-content">
    <div class="eff-date">Effective: May 19, 2026</div>

    <div class="section">
      <h2>Overview</h2>
      <p>This Cookie Policy explains how MamaOnTrack uses cookies and similar technologies when you visit our website (mamaontrack.com). This policy does not apply to the MamaOnTrack mobile app, which does not use cookies.</p>
    </div>

    <div class="section">
      <h2>What Are Cookies?</h2>
      <p>Cookies are small text files stored on your device when you visit a website. They help websites remember your preferences and understand how you use the site. Similar technologies include local storage, session storage, and pixel tags.</p>
    </div>

    <div class="section">
      <h2>Cookies We Use</h2>
      <table class="data-table">
        <thead><tr><th>Cookie Type</th><th>Purpose</th><th>Duration</th><th>Required?</th></tr></thead>
        <tbody>
          <tr><td>Session cookies</td><td>Keep you logged in during your session</td><td>Session only</td><td>Yes</td></tr>
          <tr><td>Authentication tokens</td><td>Remember your login state securely</td><td>30 days</td><td>Yes</td></tr>
          <tr><td>Preference cookies</td><td>Remember your display preferences</td><td>1 year</td><td>No</td></tr>
          <tr><td>Analytics (anonymous)</td><td>Understand how pages are used — no personal data</td><td>90 days</td><td>No</td></tr>
        </tbody>
      </table>
      <div class="highlight">
        <p><strong>What we do NOT use:</strong> We do not use advertising cookies, tracking pixels, social media pixels, third-party marketing cookies, or any cookies that track you across other websites.</p>
      </div>
    </div>

    <div class="section">
      <h2>Managing Cookies</h2>
      <p>You can control cookies through your browser settings. Most browsers allow you to view, delete, and block cookies. Please note that blocking essential cookies may affect your ability to log in and use our website.</p>
      <ul>
        <li><strong>Chrome</strong> — Settings &gt; Privacy and Security &gt; Cookies and other site data</li>
        <li><strong>Safari</strong> — Settings &gt; Safari &gt; Privacy & Security</li>
        <li><strong>Firefox</strong> — Settings &gt; Privacy & Security &gt; Cookies and Site Data</li>
        <li><strong>Edge</strong> — Settings &gt; Cookies and site permissions</li>
      </ul>
    </div>

    <div class="section">
      <h2>Contact</h2>
      <div class="contact-card">
        <h3>Cookie Questions?</h3>
        <p>We are happy to explain anything about how we use cookies.</p>
        <a href="mailto:privacy@mamaontrack.com" class="contact-link">privacy@mamaontrack.com</a>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════
     CONTACT US
══════════════════════════════════════════ -->
<div class="page" id="contact">
  <div class="page-hero">
    <h1>Contact Us</h1>
    <p>We respond to all inquiries within 48 hours</p>
  </div>
  <div class="page-content">

    <div class="section">
      <h2>Get in Touch</h2>
      <p>We are a small team built by a nurse mom and we genuinely want to hear from you — whether you have a question, feedback, a bug to report, or a privacy concern. Every message is read and responded to personally.</p>
    </div>

    <div class="section">
      <h2>Contact by Topic</h2>
      <table class="data-table">
        <thead><tr><th>Topic</th><th>Email</th><th>Response Time</th></tr></thead>
        <tbody>
          <tr><td>General questions and support</td><td>support@mamaontrack.com</td><td>Within 48 hours</td></tr>
          <tr><td>Privacy and data requests</td><td>privacy@mamaontrack.com</td><td>Within 48 hours</td></tr>
          <tr><td>Legal and compliance</td><td>legal@mamaontrack.com</td><td>Within 5 business days</td></tr>
          <tr><td>Press and media</td><td>press@mamaontrack.com</td><td>Within 3 business days</td></tr>
          <tr><td>Partnership inquiries</td><td>hello@mamaontrack.com</td><td>Within 5 business days</td></tr>
          <tr><td>Bug reports</td><td>support@mamaontrack.com</td><td>Within 24 hours</td></tr>
        </tbody>
      </table>
    </div>

    <div class="section">
      <h2>Data Requests</h2>
      <p>To request a copy of your data, correct your information, or delete your account and all associated data, you can:</p>
      <ul>
        <li>Delete your account directly from within the MamaOnTrack app (Settings &gt; Delete Account)</li>
        <li>Email us at privacy@mamaontrack.com with the subject line "Data Request — [type of request]"</li>
      </ul>
      <p>We will confirm receipt of your request within 24 hours and fulfill it within 30 days.</p>
    </div>

    <div class="section">
      <h2>Report a Security Issue</h2>
      <div class="highlight">
        <p>If you discover a security vulnerability in MamaOnTrack, please report it responsibly to <strong>security@mamaontrack.com</strong>. We take all security reports seriously and will respond within 24 hours. Please do not publicly disclose any security vulnerabilities before we have had a chance to address them.</p>
      </div>
    </div>

    <div class="section">
      <h2>Mailing Address</h2>
      <p>MamaOnTrack<br>
      United States<br>
      <em>Full mailing address will be listed at launch.</em></p>
    </div>

    <div class="section">
      <h2>Social Media</h2>
      <ul>
        <li>Instagram: @MAMA_ON_TRACK</li>
        <li>Facebook: @MamaOnTrack App</li>
      </ul>
    </div>

    <div class="contact-card">
      <h3>We are here for you</h3>
      <p>Built by a nurse mom, for every mom. Your feedback makes this app better for all of us.</p>
      <a href="mailto:support@mamaontrack.com" class="contact-link">support@mamaontrack.com</a>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════
     FOOTER
══════════════════════════════════════════ -->
<footer>
  <div class="footer-logo">MamaOnTrack</div>
  <div class="footer-links">
    <a onclick="show('privacy')">Privacy Policy</a>
    <a onclick="show('terms')">Terms of Service</a>
    <a onclick="show('hipaa')">HIPAA Notice</a>
    <a onclick="show('cookie')">Cookie Policy</a>
    <a onclick="show('contact')">Contact Us</a>
  </div>
  <div class="footer-copy">
    &copy; 2026 MamaOnTrack. All rights reserved.<br>
    Built by a nurse mom, for every mom. &nbsp;&middot;&nbsp; Always ad-free.
  </div>
</footer>

<script>
  var navLinks = document.querySelectorAll('nav a');
  var footerLinks = document.querySelectorAll('.footer-links a');

  function show(page) {
    // Hide all pages
    document.querySelectorAll('.page').forEach(function(p) {
      p.classList.remove('active');
    });
    // Show selected
    document.getElementById(page).classList.add('active');
    // Update nav
    navLinks.forEach(function(a, i) {
      var pages = ['privacy','terms','hipaa','cookie','contact'];
      a.classList.toggle('active', pages[i] === page);
    });
    // Scroll to top
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
</script>

</body>
</html>
