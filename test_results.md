# Test Results — Home Credit LAP Voice Agent

## 1. Testing Objective

To verify that the Retell AI voice agent follows the preliminary Loan Against Property (LAP) eligibility rules, handles customer responses naturally, and routes or closes calls appropriately.

## 2. Testing Environment

- **Platform:** Retell AI
- **Agent type:** Conversation Flow Agent
- **Testing method:** Retell browser-based test interface
- **Test scenarios:** 16
- **Evidence:** Audio recordings and conversation transcripts, where available

## 3. Test Cases and Results

| ID | Test Scenario | Expected Behavior | Actual Result | Status |
|---|---|---|---|---|
| TC-01 | Customer meets all seven criteria | Complete qualification and offer senior-expert handoff | All seven criteria were satisfied, and the qualification flow worked as expected. | Passed |
| TC-02 | Agricultural property | Explain the eligibility restriction and close politely | Agricultural property was handled according to the eligibility rule. | Passed |
| TC-03 | Original documents unavailable | Explain the requirement and close politely | The missing-document requirement was handled correctly. | Passed |
| TC-04 | Customer requests more than ₹75 lakh but accepts ₹75 lakh | Continue with the revised amount | The revised loan amount was handled correctly. | Passed |
| TC-05 | Customer refuses the ₹75 lakh cap | Explain the offer limit and close politely | The offer limit and customer's decision were handled correctly. | Passed |
| TC-06 | Income received only in cash | Explain the bank-income requirement and close politely | The income eligibility rule was applied correctly. | Passed |
| TC-07 | Tenure below 3 years or above 15 years | Apply the configured tenure rules correctly | The tenure eligibility rules were handled correctly. | Passed |
| TC-08 | Joint property ownership | Accept joint ownership and continue | Joint ownership was accepted under the preliminary criteria. | Passed |
| TC-09 | Self-employed customer with bank-received income | Continue qualification | The occupation and bank-received income criteria were handled correctly. | Passed |
| TC-10 | Customer provides property market value | Record the estimate without inventing a minimum threshold | The property value was handled without applying an unsupported minimum threshold. | Passed |
| TC-11 | Existing LAP or EMI-reduction request | Route to the specialist flow and close politely | The specialist-routing scenario was handled correctly. | Passed |
| TC-12 | Customer is busy | Ask for a preferred callback time and end the call | The callback-preference flow worked as expected. | Passed |
| TC-13 | Customer answers questions out of order | Retain previously provided information | Out-of-order answers were handled correctly. | Passed |
| TC-14 | Checklist is incomplete | Ask for missing information and avoid premature handoff | The incomplete-checklist scenario was handled correctly. | Passed |
| TC-15 | Customer is not the intended person | Protect customer privacy and end politely | The customer-verification scenario was handled correctly. | Passed |
| TC-16 | Disqualification occurs | Explain the reason without abruptly ending the call | The disqualification and call-closing behavior worked as expected. | Passed |

## 4. Test Summary

- **Total scenarios tested:** 16
- **Passed:** 16
- **Failed:** 0
- **Pending:** 0
- **Overall result:** All tested scenarios passed according to the observed test outcomes.

## 5. Issues and Improvements

During development and testing, attention was given to:
- Preventing abrupt call endings after disqualification.
- Explaining eligibility outcomes politely.
- Handling answers provided out of order.
- Avoiding premature handoff before completing the checklist.
- Routing existing LAP and EMI-reduction requests appropriately.

The agent was tested again after the call-ending behavior was improved.

## 6. Conclusion

The Retell AI voice agent successfully handled all 16 tested scenarios according to the observed outcomes. The testing covered the preliminary eligibility checklist, customer verification, callback handling, specialist routing, incomplete information, and polite call endings.

The agent performs preliminary qualification only. Final loan eligibility, applicable rates, documentation checks, and loan approval remain subject to the lender's assessment.
The test results should demonstrate whether the voice agent follows the specified qualification rules and conversation flow. The final conclusion must reflect the scenarios actually tested and their observed outcomes.
