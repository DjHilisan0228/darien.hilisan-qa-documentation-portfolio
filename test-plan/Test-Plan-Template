# Test Plan Template

*Prepared by: Darien James Hilisan, QA Engineer*
*Based on the test plans I wrote and maintained for web applications, admin tools, scheduled jobs, and learning-content releases (2022 – present).*

> **How to use this template:** Replace everything in `[brackets]`. Delete sections that don't apply. Keep the scope section high-level at the start of a project and add detail as requirements are finalized. Each test case should be linked to the user story it tests.

---

## 0. Document Information

| Field | Details |
| --- | --- |
| Project / Feature Name | [Project name] |
| Related Epic / User Story | [Ticket link] |
| Test Plan Version | [v1.0] |
| Author | [QA Engineer name] |
| Reviewer(s) | [Test Lead / QA Reviewer] |
| Approver | [QA Supervisor / QA Manager] |
| Last Updated | [YYYY-MM-DD] |

---

## 1. Test Objectives

- Verify that [feature/system] meets the acceptance criteria defined in the user stories and system specifications.
- Confirm that existing features are not affected by the changes (regression).
- [If applicable] Check system stability, response time, and scalability under expected load.
- Provide the test results and a release recommendation to the project team.

---

## 2. Test Scope and Coverage

*The items below are high-level. More detailed requirements will be added as the project progresses, and this plan will be updated to match.*

### 2.1 Features to Be Tested

| Feature | Details | Component / Repository | Status |
| --- | --- | --- | --- |
| [e.g., Scheduled daily job] | [e.g., Applies restrictions automatically based on threshold rules] | [Service / repo name] | `NEW` |
| [e.g., Admin monitoring tool] | [e.g., Threshold configuration, list view, bulk ID upload] | [Back-office app] | `NEW` |
| [e.g., Email notifications] | [e.g., New templates for each rule tier] | [Web app / mail service] | `UPDATED` |
| [e.g., Audit / activity logs] | [e.g., Recording of record updates and DB trails] | [Web app] | `EXISTING` |
| [e.g., User scheduling page] | [e.g., Blocking / opening / closing of slots] | [Web app] | `REGRESSION` |

### 2.2 User Role / Account Type Coverage

✔ = In scope   ✖ = Out of scope

| Feature / Action | [Account Type A] | [Account Type B] | [Account Type C] | [Account Type D] |
| --- | --- | --- | --- | --- |
| [Action 1, e.g., Open slot] | ✔ | ✔ | ✖ | ✔ |
| [Action 2, e.g., Close slot] | ✔ | ✔ | ✖ | ✔ |
| Affected by project changes | ✔ | ✔ | ✖ | ✖ |

### 2.3 In Scope

**[Feature 1 — e.g., Business rules / thresholds]**
- [ ] Verify [rule] is applied when [condition] is met (minimum and maximum boundary values).
- [ ] Verify [rule] is NOT applied when [condition] is not met.
- [ ] Verify the scheduled job runs at the expected frequency and time window ([e.g., daily, 1:00–4:00 AM]).
- [ ] Verify records that were manually adjusted are skipped by the automation.
- [ ] Verify every action performed by the system is logged.

**[Feature 2 — e.g., User-facing pages]**
- [ ] Verify the user can view [updated data] for the current and following days.
- [ ] Verify the correct error / validation message is shown when [time limit or rule] is not met.
- [ ] Verify the confirmation pop-up shows the correct options, and buttons are enabled/disabled correctly.

**[Feature 3 — e.g., Email notifications]**
- [ ] Verify users receive the correct email for each rule tier (new vs. extension).
- [ ] Verify staff receive a summary report email with the required data fields.

**Edge Cases**
- [ ] [Two rules are triggered for the same record at the same time]
- [ ] [Concurrent actions by two users on the same record]
- [ ] [Boundary values: minimum, maximum, just below, just above]

**Regression Testing**
- [ ] Existing [feature] functions still work for all account types.
- [ ] Re-run existing automated test suites as smoke tests.

### 2.4 Out of Scope

1. [Account types / regions / user groups not affected by this change]
2. [Pages or modules owned by another team or partner]
3. [Features planned for a later phase]
4. [Third-party integrations (e.g., live chat, payment gateway)]

---

## 3. Estimates, Schedule, and QA Resources

### 3.1 QA Estimates

| Task | Estimated Man-days (1 resource) | Estimated Man-days (with 10% buffer) |
| --- | --- | --- |
| Planning (estimation, timeline, test plan) | [ ] | [ ] |
| Test Design (test cases / scenario matrix + review) | [ ] | [ ] |
| Test Script Creation (automation + review) | [ ] | [ ] |
| Test Execution (manual, automated, performance, regression) | [ ] | [ ] |
| UAT Support and Release Support | [ ] | [ ] |
| **Total** | [ ] | [ ] |

*The schedule may change based on the development timeline.*

### 3.2 QA Resources

| Resource Name | Role |
| --- | --- |
| [Name] | QA Engineer |
| [Name] | Test Lead / Assigned QA Reviewer (test cases, UAT checklist) |
| [Name] | QA Supervisor |

---

## 4. Test Strategy and Approach

### 4.1 Test Levels, Test Types, and Tools

*Listed in the order testing will be done:*

| Test Type | Environment | Tools | Remarks |
| --- | --- | --- | --- |
| Manual Testing | Staging | [Test management tool, e.g., BrowserStack Test Management / spreadsheet] | See Manual Testing Strategy |
| Automated Testing | Staging | Selenium via Robot Framework | See Automated Testing Strategy |
| Performance Testing | Staging | [Browser DevTools / Gatling / CloudWatch] | See Performance Testing Strategy |
| Regression / Sanity Testing | Staging | Existing test cases + automated scripts | Run after bug fixes to confirm other features are not affected |
| Ad hoc / Exploratory Testing | Staging | Record findings in the test deliverables file | After the main testing tasks |
| User Acceptance Testing (UAT) | Staging | UAT checklist | After each increment is delivered, or as agreed by the team |

**Test types NOT included in this plan:** [e.g., Compatibility testing, API testing, Security testing]

### 4.2 Test Types per Feature

| Feature | Manual | Automated | Performance | Regression | Exploratory | UAT |
| --- | --- | --- | --- | --- | --- | --- |
| [Feature 1] | ✔ | ✔ | ✖ | ✔ | As needed | ✔ |
| [Feature 2] | ✔ | ✖ | ✔ | As needed | As needed | ✔ |
| [Feature 3] | ✔ | ✖ | ✖ | ✔ | As needed | As needed |

### 4.3 Manual Testing Strategy

**Test Deliverables Preparation**
- Write test cases in [tool]. Store them in [shared project folder / test repository].
- Link each test case to the user story it tests.
- Create other deliverables as needed (scenario matrix, test progress tracker).

**Test Deliverables Review**
- Create a review task for each request (2–3 user stories/features per review).
- The reviewer approves by leaving an approval comment on the review task.

**Test Execution**
- Record results (Passed / Failed / Blocked / Not Run) in the test case file, with evidence.

### 4.4 Automated Testing Strategy

**Existing test scripts related to the project**
- [ ] There are no existing test scripts.
- [ ] There are existing test scripts: `[path/to/test_suite.robot]`

**Test script creation during the project**
- [ ] New test scripts will be created / existing suites will be updated.
- [ ] No new test scripts will be created.

**Repository:** [Link to automation repository]

**Script Preparation:** Re-check test accounts and test data before running. Update existing suites to cover new modules.

**Script Review:** Create a review task. The reviewer approves the merge request before merging.

**Execution and Reporting:** Run locally or through the CI pipeline. Upload the generated reports to the project folder.

### 4.5 Performance Testing Strategy

**Scope:** [e.g., Scheduled job, high-traffic pages, key API endpoints]

**Scenarios to Check:**
- [e.g., Total run time of the scheduled job]
- [e.g., Response time when processing a single record vs. multiple records]
- [e.g., Load levels by feature impact]

| Feature Impact | Load Levels | Acceptance Criteria |
| --- | --- | --- |
| High | [10 / 15 / 20 requests per second] | Response time under [1–3] seconds; no error responses; CPU usage under [20%] |
| Medium | [5 / 10 / 15 requests per second] | Same as above |
| Low | [3 / 5 / 10 requests per second] | Same as above |

**Execution:** Run the scenarios (manually with browser DevTools, or with a load-testing tool), and record the results in the test deliverables file.

**Initial Acceptance Criteria:**
- No error responses
- No timeout errors
- Processing time is similar to or faster than the current/manual process

### 4.6 Test Data Preparation

- **Staff / Admin Accounts:** Request access to [admin tools] with the required permissions.
- **End-User Accounts:** Create or search test accounts with the test-data tool for each account type in scope.
- **Customer Accounts:** Create test accounts with the debug tools.
- **Transactional Data:** Set up fresh test records manually (or with SQL scripts) rather than relying on copies of production data.

### 4.7 Test Environment

| Item | Details |
| --- | --- |
| Environment | [Staging cluster / environment name] |
| Applications | [User web app URL], [Admin tool URL], [Customer site URL] |
| Databases | [DB names, accessed through query tool] |
| Browsers | [e.g., Google Chrome (latest)] |
| Operating Systems | [e.g., macOS, Windows] |
| Monitoring / Logs | [e.g., Grafana, AWS CloudWatch] |

### 4.8 Entry and Exit Criteria

| Test Type | Entry Criteria | Exit Criteria |
| --- | --- | --- |
| Manual Testing | 1. User stories and system specs are available *(Product)*<br>2. Test cases are written and reviewed *(QA)*<br>3. Test environments are available *(DevOps)*<br>4. Code changes are reviewed and ready for testing *(Dev)* | • 100% of test cases passed; OR<br>• No open critical or major defects;<br>• Workarounds are provided for issues still to be fixed;<br>• Fixes are agreed for the next sprint;<br>• Test Summary Report is created |
| Automated Testing | 1. User stories and specs are available *(Product)*<br>2. Test scripts are written and reviewed *(QA)*<br>3. Environment is available *(DevOps)*<br>4. Code changes are ready for testing *(Dev)* | Same as above |
| Performance Testing | All changes are deployed (code and database updates) *(Dev)* | Acceptance criteria in 4.5 are met |
| Regression / Sanity Testing | All changes are deployed *(Dev)* | No regression defects found |
| UAT | 1. 100% of manual test cases passed *(QA)*; OR<br>2. No open critical or major defects *(Dev)*<br>3. UAT checklist is available *(Product)* | UAT checklist is signed off |

### 4.9 Suspension and Resumption Criteria

| 🔴 Suspension Criteria | 🟢 Resumption Criteria | Remarks |
| --- | --- | --- |
| Requirements or acceptance criteria change, or new requirements affect current criteria | Changes are discussed and agreed; impact is assessed; deliverables and timeline are updated | Pause testing for the affected story and continue with other items |
| Test environment becomes unavailable | Environment is available again | Check whether testing is possible in another environment |
| At least 60% of test cases fail or are blocked, OR a blocker defect stops critical/major test cases | The blocker is fixed, reviewed, and deployed to the test environment | Continue with items not affected by the blocker |

### 4.10 Defect Management

- Log defects in [issue tracker / project board].
- Follow the defect severity levels: **Critical / Major / Minor / Trivial**.
- **Summary format:** `[User Role] + [Action] + [Page/Module]`
  *Example: "Admin cannot save updated threshold values on the monitoring tool."*
- **Description template:**
  ```
  Scenario:
  Prerequisites:
  Steps to Reproduce:
  Expected Result:
  Actual Result:
  Evidence (screenshot / screen recording):
  Environment (Dev / Staging / Production):
  Severity Level:
  Impact:
  ```
- After logging: link the defect to the affected or blocked user story, and notify the developer in the team channel.

---

## 5. Release

### 5.1 QA Release Decision Checklist

We can release if:
1. The Sprint Review has passed; **and**
2. All test cases have passed:
   - 100% of staging test cases passed;
   - 100% of internal UAT test cases passed;
   - 100% of client/stakeholder UAT test cases passed; **or**
3. No critical test cases are still marked Failed or Blocked; **and**
4. Any remaining non-critical defects have an agreed fix plan and timeline.

### 5.2 QA Release Support Tasks

- Release Action Plan with a Test Summary Report
- Production Verification Checklist
- Test accounts prepared for production checks
- Rollback / hotfix support and monitoring if issues are found after release

---

## 6. Sign-off

| Role | Name | Date | Sign-off |
| --- | --- | --- | --- |
| QA Engineer | [ ] | [ ] | [ ] |
| Test Lead / QA Reviewer | [ ] | [ ] | [ ] |
| QA Supervisor | [ ] | [ ] | [ ] |
| Product Owner | [ ] | [ ] | [ ] |
