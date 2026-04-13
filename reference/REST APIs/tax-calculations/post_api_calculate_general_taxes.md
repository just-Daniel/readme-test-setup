---
title: Tax Calculator API
excerpt: >
  InsCipher’s Tax Calculator API simplifies compliance by automatically
  calculating complex, state-specific insurance taxes and fees for single or
  multi-line transactions. By providing basic details like location, dates, and
  coverage types, you instantly receive a complete line-by-line tax breakdown,
  the exact state stamp wording, transparent calculation rules, and a list of
  necessary filing documents to ensure accurate quoting and compliance.


  <h2>🚀 Watch This First</h2>

  <p>Before getting started, please watch this short walkthrough:</p>

  <p><a
  href="https://support.inscipher.com/hubfs/Dev%20Hub/Tax%20Calculator%20API.mp4"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:8px 12px; border-radius:6px; text-decoration:none;
  display:inline-block;"><strong>Watch the Tax Calculator API
  video</strong></a></p>


  <hr/>


  <details>

  <summary><strong>Getting Started</strong></summary>




  ### Obtaining Access
   InsCipher requires that you first obtain contracted permission to utilize our Tax Calculator API. If you are not already contract, please reach out to <a href="mailto:info@inscipher.com" style="color:#d9f2ff;">Sales</a> to start that process. If you are a client, please work with your InsCipher implementation specialist to get setup and obtain your API key.


  ### Important Variables to Consider

  To ensure accurate request construction, reference the following data tables
  for mapping codes and interpreting compliance deliverables:

  <br><br>

  - <a
  href="https://lookerstudio.google.com/u/0/reporting/f3c07407-ee34-4ec9-8a4a-f90b1d585e6b/page/p_4q66kh8crc"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Generic Lines of Business List</a> (Map the
  lines of business you write to our generic coverage list)

  - <a
  href="https://lookerstudio.google.com/u/0/reporting/41dce747-d045-4e1f-884d-07d23581a90a/page/p_83noca0k9c"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Transaction Types List</a> (Map your
  transaction types to our list)

  - <a
  href="https://lookerstudio.google.com/u/0/reporting/f3c07407-ee34-4ec9-8a4a-f90b1d585e6b/page/p_otc1uchjqc"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Document Requirements</a> (State-specific
  policy document required to bind coverage)

  - <a href="https://lookerstudio.google.com/s/pruKt8r4i3Q" target="_blank"
  rel="noopener noreferrer" style="background-color:#d9f2ff; padding:0 3px;
  border-radius:3px;">State Stamp Wording</a>

  - <a
  href="https://lookerstudio.google.com/u/0/reporting/f3c07407-ee34-4ec9-8a4a-f90b1d585e6b/page/p_xv4ud8gjqc"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Unique State Tax Titles</a>





  ### Tax Calculation Category

  - Non-Admitted (Default): <code>"non-admitted": 0</code>

  - Admitted (Kentucky Only): <code>"admitted": 1</code>

  </details>




  <details>



  <summary><strong>FAQs</strong></summary>


  ### Can I calculate taxes for future policy effective dates?


  State taxes and fees can change at any time. However, most states update taxes
  in the fall (if they update taxes at all). InsCipher maintains at least one
  full calendar year tax rates at a time. Tax rules are updated for the
  following year by the InsCipher Compliance Team (typically finalized
  Sept/Oct). Because future rates are unpredictable, best practice is to submit
  transactions within the current calendar year.


  ### How do I calculate taxes on endorsements?


  For endorsements, submit the **difference** in premium (not the new total).

  - **APE (Additional Premium):** Submit the positive difference (e.g., original
  $500, new $650, submit **$150**).

  - **RPE (Return Premium):** Submit the positive difference. The system
  recognizes the RPE transaction type and applies it as a credit automatically.


  ### How are Documents returned via this endpoint?


  1. **Templates:** Links to download blank state forms.

  2. **Requirements:** Informational flags indicating if a specific document is
  required for submission.


  ### How do Generic Lines of Business Import Codes work?


  Use our <a
  href="https://lookerstudio.google.com/u/0/reporting/f3c07407-ee34-4ec9-8a4a-f90b1d585e6b/page/p_4q66kh8crc"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Generic Import Codes</a> (GEN-XXXX) to
  simplify line of business mapping to state specific codes. Some states have
  line of business specific tax rates (not all). Custom mapping adjustments can
  be requested during implementation.


  ### How should I understand tax titles?


  In some states, rather than having a unique field name, we have chose to
  repurpose field names for specific fees. Refer to the <a
  href="https://lookerstudio.google.com/u/0/reporting/f3c07407-ee34-4ec9-8a4a-f90b1d585e6b/page/p_xv4ud8gjqc"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Unique State Tax Titles</a> datasheet for
  definitions.


  ### Do states restrict broker or carrier fees?


  Also uncommon, certain states restrict fees. In the JSON response, we will
  automatically adjust the fee amounts (should there be fee restrictions). For a
  summary, refer to the <a
  href="https://lookerstudio.google.com/u/0/reporting/f3c07407-ee34-4ec9-8a4a-f90b1d585e6b/page/p_tz4ybpmhzc"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Fee Restrictions Guide</a>.


  ### What classifies as 'Taxable Fees'?


  InsCipher will determine whether or not a specific broker or carrier fee is
  taxable and return the calculated amount in the JSON response. It is important
  that you map the fees you charge to the insured (in excess of premium) to
  either 'Broker Fees' [agency_fee], 'Carrier Fees' [inspection_fees]. For a
  summary of taxable fees, please refer to the <a
  href="https://lookerstudio.google.com/u/0/reporting/f3c07407-ee34-4ec9-8a4a-f90b1d585e6b/page/p_f7qdebf6sd"
  target="_blank" rel="noopener noreferrer" style="background-color:#d9f2ff;
  padding:0 3px; border-radius:3px;">Taxable Fees Guide</a>.


  </details>
api:
  file: oas_tax_calculations.json
  operationId: post_api_calculate_general_taxes
hidden: false
---