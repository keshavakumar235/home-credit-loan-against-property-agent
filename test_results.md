# Test Results — Home Credit LAP Voice Agent

## 1. Testing Objective

The objective is to verify that the voice agent follows the preliminary Loan Against Property (LAP) qualification rules, handles customer responses naturally, and routes or ends calls correctly.

## 2. Test Cases

**Important:** Update the Observed Result and Status columns based on what actually happened during your Retell tests. Do not mark a scenario as passed unless you verified it.

| Test ID | Scenario | Expected Result | Observed Result | Status |
|---|---|---|---|---|
| TC-01 | Customer satisfies all seven criteria | Complete the checklist and offer a senior-expert handoff | Record actual outcome | Pending verification |
| TC-02 | Customer offers agricultural property | Explain the property eligibility rule and end qualification | Record actual outcome | Pending verification |
| TC-03 | Customer does not have original property documents | Explain that original documents are required and end qualification | Record actual outcome | Pending verification |
| TC-04 | Customer requests ₹80 lakh and agrees to ₹75 lakh | Confirm the revised amount and continue qualification | Record actual outcome | Pending verification |
| TC-05 | Customer requests more than ₹75 lakh and declines the cap | Explain the maximum offer and end qualification | Record actual outcome | Pending verification |
| TC-06 | Customer receives income only in cash | Explain the income requirement and end qualification | Record actual outcome | Pending verification |
| TC-07 | Customer requests a tenure below 3 years | Explain the permitted tenure range and end qualification | Record actual outcome | Pending verification |
| TC-08 | Customer requests a tenure above 15 years | Explain the permitted tenure range and end qualification | Record actual outcome | Pending verification |
| TC-09 | Customer has joint property ownership | Accept joint ownership and continue the checklist | Record actual outcome | Pending verification |
| TC-10 | Self-employed customer receives income through a bank | Accept the occupation/income response and continue qualification | Record actual outcome | Pending verification |
| TC-11 | Customer provides an estimated property value | Record the answer without inventing a minimum-value threshold | Record actual outcome | Pending verification |
| TC-12 | Customer already has a LAP or wants EMI reduction | Route to a specialist and end the current qualification flow | Record actual outcome | Pending verification |
| TC-13 | Customer is busy | Ask for a preferred callback time and end the call | Record actual outcome | Pending verification |
| TC-14 | Customer gives answers out of order | Retain relevant answers and avoid unnecessary repetition | Record actual outcome | Pending verification |
| TC-15 | Customer has not answered every checklist item | Ask for missing information; do not hand off prematurely | Record actual outcome | Pending verification |
| TC-16 | Customer is not the intended person | Avoid disclosing offer details and end politely | Record actual outcome | Pending verification |

## 3. Testing Environment

- **Platform:** Retell AI
- **Agent type:** Conversation Flow Agent
- **Testing method:** Retell browser-based test interface
- **Voice and model:** As configured in the Retell dashboard
- **Evidence:** Save the corresponding audio recording and transcript for each important test.

## 4. Test Summary

- Total scenarios listed: 16
- Scenarios passed: Update after testing
- Scenarios failed: Update after testing
- Scenarios pending: Update after testing

## 5. Defects and Improvements

Document any issues discovered during testing, such as abrupt call endings, repeated questions, incorrect eligibility decisions, or premature handoffs.

For each issue, record:
1. The scenario that triggered it.
2. The actual behavior.
3. The correction made to the agent.
4. The retest result.

## 6. Conclusion

The test results should demonstrate whether the voice agent follows the specified qualification rules and conversation flow. The final conclusion must reflect the scenarios actually tested and their observed outcomes.
