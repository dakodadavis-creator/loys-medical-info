<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Loys D. Baites — Medical Info & Medications</title>
  <style>
    :root{
      --bg:#0b0f14;
      --card:#111827;
      --text:#e5e7eb;
      --muted:#94a3b8;
      --border:rgba(148,163,184,.25);
      --accent:#38bdf8;
      --warn:#fb7185;
      --chip:rgba(56,189,248,.12);
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
      background: linear-gradient(180deg, #05070a, var(--bg));
      color:var(--text);
      padding:16px;
    }
    .wrap{max-width:960px;margin:0 auto;}
    header{
      display:flex;gap:12px;align-items:flex-start;justify-content:space-between;
      padding:16px;border:1px solid var(--border);border-radius:16px;
      background: rgba(17,24,39,.75); backdrop-filter: blur(6px);
    }
    h1{margin:0;font-size:18px;line-height:1.2}
    .sub{margin:6px 0 0 0;font-size:13px;color:var(--muted)}
    .chips{display:flex;flex-wrap:wrap;gap:8px;justify-content:flex-end}
    .chip{
      font-size:12px; padding:8px 10px;border-radius:999px;
      border:1px solid var(--border); background:var(--chip); color:var(--text);
      white-space:nowrap;
    }
    .grid{display:grid;grid-template-columns:1fr;gap:14px;margin-top:14px;}
    @media (min-width: 860px){
      .grid{grid-template-columns:1fr 1fr;}
      .full{grid-column:1 / -1;}
    }
    .card{
      padding:16px;border-radius:16px;border:1px solid var(--border);
      background: rgba(17,24,39,.75);
    }
    .card h2{margin:0 0 10px 0;font-size:14px;color:#f1f5f9}
    .kv{
      display:grid;grid-template-columns:140px 1fr;gap:8px 12px;
      font-size:13px;line-height:1.35;
    }
    .k{color:var(--muted)}
    .v{color:var(--text)}
    .alert{
      border-left:4px solid var(--warn);
      background: rgba(251,113,133,.10);
    }
    .note{
      margin-top:10px;padding:10px 12px;border-radius:12px;
      border:1px dashed rgba(148,163,184,.45);
      color:var(--muted);font-size:12px;
    }
    table{
      width:100%;
      border-collapse:collapse;
      border:1px solid var(--border);
      border-radius:12px;
      overflow:hidden;
      font-size:13px;
    }
    th,td{
      padding:10px;
      border-bottom:1px solid var(--border);
      vertical-align:top;
    }
    th{
      text-align:left;
      background: rgba(148,163,184,.08);
      font-weight:600;
      font-size:12.5px;
      color:#f1f5f9;
    }
    tr:last-child td{border-bottom:none}
    a{color:var(--accent);text-decoration:none}
    a:hover{text-decoration:underline}
    .footer{
      margin-top:14px;
      text-align:center;
      color:var(--muted);
      font-size:12px;
    }
    .printBtn{
      display:inline-block;margin-top:10px;
      padding:8px 12px;border-radius:999px;
      border:1px solid var(--border);
      background: rgba(148,163,184,.08);
      color:var(--text);
      font-size:12px;
    }
    @media print{
      body{background:#fff;color:#000;padding:0}
      header,.card,table{background:#fff;border-color:#ddd}
      .chip,.note,.printBtn{display:none !important}
      .k,.footer{color:#444}
      a{color:#000;text-decoration:none}
      .wrap{max-width:none}
    }
  </style>
</head>

<body>
  <div class="wrap">
    <header>
      <div>
        <h1>Medical Info & Medication List — Loys D. Baites</h1>
        <p class="sub">
          Last updated:
          <span id="lastUpdated"></span>
          • Intended for appointment check-in, ER, and medication reconciliation.
        </p>
        <a class="printBtn" href="#" onclick="window.print(); return false;">Print this page</a>
      </div>
      <div class="chips">
        <div class="chip"><strong>Active Cancer Patient</strong></div>
        <div class="chip">West Cancer Clinic</div>
      </div>
    </header>

    <div class="grid">
      <section class="card alert full">
        <h2>Important</h2>
        <div class="kv">
          <div class="k">Status</div>
          <div class="v"><strong>Active cancer patient — treated at West Cancer Clinic</strong></div>

          <div class="k">SSN (Last 4)</div>
          <div class="v"><em>Not on file</em></div>

          <div class="k">Photo</div>
          <div class="v"><em>Not on file</em></div>
        </div>
        <div class="note">
          To add SSN last-4, replace “Not on file”. To add a photo, upload an image to the repo and update the “Photo” section.
        </div>
      </section>

      <section class="card">
        <h2>Patient</h2>
        <div class="kv">
          <div class="k">Name</div><div class="v">Loys D. Baites</div>
          <div class="k">DOB</div><div class="v">03/04/1958</div>
          <div class="k">Patient ID</div><div class="v">562410</div>
          <div class="k">Phone</div><div class="v"><a href="tel:+19014890764">901-489-0764</a></div>
          <div class="k">Address</div>
          <div class="v">
            1584 Eastmoreland Ave Apt 3<br/>
            Memphis, TN 38104
          </div>
        </div>
      </section>

      <section class="card">
        <h2>Treating Facility</h2>
        <div class="kv">
          <div class="k">Clinic</div><div class="v">West Cancer Clinic</div>
          <div class="k">Address</div>
          <div class="v">
            1588 Union Avenue<br/>
            Memphis, TN 38104
          </div>
          <div class="k">Phone</div><div class="v"><a href="tel:+19013001562">(901) 300-1562</a></div>
          <div class="k">Fax</div><div class="v">(901) 685-9718</div>
          <div class="k">Oncologist</div><div class="v">Dr. Leonard Jeff Harris (Oncologist)</div>
          <div class="k">Direct</div><div class="v"><a href="tel:+19016830055">901-683-0055</a></div>
          <div class="k">Email</div><div class="v"><a href="mailto:HarrisPod@westclinic.com">HarrisPod@westclinic.com</a></div>
        </div>
      </section>

      <section class="card full">
        <h2>Emergency Contact / Medical POA</h2>
        <div class="kv">
          <div class="k">Name</div><div class="v">DaKoda Davis</div>
          <div class="k">Role</div><div class="v">Friend and Medical POA</div>
          <div class="k">Phone</div><div class="v"><a href="tel:+12134530609">213-453-0609</a></div>
        </div>
      </section>

      <section class="card full">
        <h2>Prescription Medications</h2>
        <table>
          <thead>
            <tr>
              <th style="width:26%;">Medication</th>
              <th style="width:16%;">Strength</th>
              <th style="width:34%;">How Taken</th>
              <th style="width:24%;">Purpose</th>
            </tr>
          </thead>
          <tbody>
            <tr><td><strong>Acalabrutinib maleate</strong></td><td>100 mg tablet</td><td>1 tablet by mouth every 12 hours</td><td>Leukemia</td></tr>
            <tr><td><strong>Allopurinol</strong></td><td>300 mg tablet</td><td>1 tablet by mouth twice daily</td><td>Uric acid reduction</td></tr>
            <tr><td><strong>Alprazolam</strong></td><td>1 mg tablet</td><td>1 tablet by mouth every 12 hours as needed</td><td>Anxiety</td></tr>
            <tr><td><strong>Atorvastatin</strong></td><td>20 mg tablet</td><td>1 tablet by mouth once daily</td><td>Cholesterol</td></tr>
            <tr><td><strong>Benazepril–HCTZ</strong></td><td>10 mg / 12.5 mg tablet</td><td>1 tablet by mouth once daily</td><td>Blood pressure</td></tr>
            <tr><td><strong>Bupropion SR</strong></td><td>150 mg tablet</td><td>1 tablet by mouth twice daily</td><td>Depression</td></tr>
            <tr><td><strong>Fluticasone nasal spray</strong></td><td>50 mcg</td><td>2 sprays in each nostril once daily</td><td>Allergic rhinitis</td></tr>
            <tr><td><strong>Gabapentin</strong></td><td>300 mg capsule</td><td>1 capsule by mouth three times daily</td><td>Nerve pain</td></tr>
            <tr><td><strong>Lansoprazole (delayed-release)</strong></td><td>30 mg capsule</td><td>1 capsule by mouth every morning</td><td>Acid reflux</td></tr>
            <tr><td><strong>Meloxicam</strong></td><td>15 mg tablet</td><td>1 tablet by mouth once daily</td><td>Pain / inflammation</td></tr>
            <tr><td><strong>Triamcinolone cream</strong></td><td>0.1% topical</td><td>Apply as directed</td><td>Skin inflammation</td></tr>
            <tr><td><strong>Valacyclovir</strong></td><td>500 mg tablet</td><td>1 tablet by mouth once daily</td><td>Shingles prevention</td></tr>
            <tr><td><strong>Wixela Inhub</strong></td><td>250 / 50 mcg inhaler</td><td>Use as directed</td><td>COPD / Asthma</td></tr>
            <tr><td><strong>Zolpidem</strong></td><td>10 mg tablet</td><td>1 tablet by mouth at bedtime</td><td>Sleep</td></tr>
          </tbody>
        </table>
      </section>

      <section class="card full">
        <h2>Over-the-Counter / Supplements</h2>
        <table>
          <thead>
            <tr>
              <th>Name</th>
              <th>Dose</th>
              <th>Frequency</th>
            </tr>
          </thead>
          <tbody>
            <tr><td><strong>Centrum Silver</strong></td><td>Multivitamin</td><td>Once daily</td></tr>
            <tr><td><strong>Ester-C Immune Support</strong></td><td>Vitamin C</td><td>Once daily</td></tr>
          </tbody>
        </table>

        <div class="note">
          If any medication is stopped/started or doses change, update this page and the QR code will still work.
        </div>
      </section>
    </div>

    <div class="footer">
      Tip: Add this page to your phone home screen for quick access.
    </div>
  </div>

  <script>
    const d = new Date();
    document.getElementById("lastUpdated").textContent = d.toLocaleDateString();
  </script>
</body>
</html>
