
## Task 1: Quality Assurance Testing

### Objective
Perform comprehensive exploratory testing of the RealWorld demo application (https://demo.realworld.show) and document findings with evidence.

### Key Findings

#### Validation Vulnerabilities
- **Whitespace-Only Sign Up Bypass**: Account creation accepts whitespace-only credentials
- **Whitespace-Only Article Creation**: Article form bypasses empty content validation
- **Whitespace-Only Comments**: Comments field accepts whitespace without validation

#### Security & Authentication Issues
- **JWT Token Persistence**: Authentication token remains valid after user logout
- **Session Management**: No proper token revocation on logout

#### Functionality & UX Concerns
- **Pagination Issues**: Article comments lack proper pagination controls for large datasets
- **API Error Handling**: Invalid routes return poor error messages instead of proper HTTP responses
- **Profile Image UX**: Image URL field only accepts URLs; no file upload fallback
- **Focus State Bug**: Logo and sign-in elements lack visible focus indicators for keyboard navigation

#### Production Readiness
- Documented edge cases and unexpected behaviors that could impact production stability

### Testing Methodology
- Manual exploratory testing across all application features
- Cross-browser compatibility assessment
- Security and validation testing
- User experience and accessibility evaluation
- Screenshot documentation and evidence collection

### Deliverables
- Detailed QA Report (PDF) with categorized findings, severity levels, and reproduction steps
- Supporting screenshots demonstrating each issue
- Clear recommendations for remediation

---

## Task 2: n8n Workflow Automation

### Objective
Design and implement a multi-step automation workflow using n8n Cloud that demonstrates workflow orchestration, API integration, data transformation, and conditional logic.

### Workflow Architecture

**Trigger & Data Retrieval**
- Event-driven trigger (schedule or webhook)
- Calls public API to fetch data

**Data Processing**
- Transforms and filters API results
- Applies business logic rules
- Prepares data for enrichment

**API Enrichment**
- Second API call to enrich processed data
- Combines results from multiple sources

**Conditional Branching**
- Routes workflow based on data conditions
- Handles success and error scenarios

**Error Handling**
- Comprehensive error catching
- Fallback logic for API failures
- Graceful degradation

**Notification Delivery**
- Sends digest to configured notification channel
- Formatted for readability and action

### Key Features
- Robust error handling and retry logic
- Data transformation and validation
- Multi-source API integration
- Conditional routing and branching
- Clean notification formatting

### Deliverables
- `workflow.json`: Complete n8n workflow export
- Workflow screenshot showing visual structure
- Successful execution screenshot with sample output
- Detailed workflow documentation explaining each step

---

## Technologies & Tools

| Category | Technologies |
|----------|---------------|
| **Testing & QA** | Manual exploratory testing, cross-browser testing, security assessment |
| **Workflow Automation** | n8n Cloud, REST APIs, JSON transformation |
| **Documentation** | Markdown, PDF reports, screenshots |
| **Platforms** | RealWorld demo application, n8n Cloud |

---

## Submission Checklist

- ✅ Task 1: Comprehensive QA testing completed with documented findings
- ✅ Task 1: Bug report with reproduction steps, screenshots, and severity levels
- ✅ Task 1: Evidence-based findings with clear categorization
- ✅ Task 2: n8n workflow implemented with multi-step automation
- ✅ Task 2: Workflow includes API integration, transformation, and conditional logic
- ✅ Task 2: Error handling implemented throughout workflow
- ✅ Task 2: Workflow exported and documented
- ✅ Task 2: Successful execution screenshots provided
- ✅ Bonus: Additional automation examples included (if applicable)
- ✅ README: Comprehensive documentation of approach and findings

---

## Screenshots & Evidence

### Task 1: Testing Evidence
- Sign-up validation bypass demonstration
- Article creation whitespace vulnerability
- Comment submission issues
- JWT token persistence proof
- API error handling examples
- UI focus state problems
- Profile image URL limitations

### Task 2: Workflow Execution
- n8n workflow visual diagram
- Successful workflow execution with output
- Data transformation examples
- Error handling in action

---

## Approach & Methodology

### Quality Assurance Testing
1. **Scope Definition**: Identified critical user journeys across the application
2. **Exploratory Testing**: Performed unscripted testing to discover edge cases
3. **Systematic Documentation**: Captured each issue with evidence and reproduction steps
4. **Risk Assessment**: Categorized findings by severity and business impact
5. **Clear Recommendations**: Provided actionable remediation guidance

### Workflow Design
1. **Requirements Analysis**: Understood the multi-API integration requirements
2. **Architecture Planning**: Designed workflow flow with decision points
3. **Error Resilience**: Built comprehensive error handling throughout
4. **Testing & Validation**: Executed and verified successful operation
5. **Documentation**: Documented each workflow component for maintainability

---

## Key Competencies Demonstrated

- **QA Expertise**: Manual testing, exploratory testing, bug identification and documentation
- **Security Mindedness**: Input validation, authentication, and API security assessment
- **Attention to Detail**: Comprehensive documentation with evidence and reproduction steps
- **Technical Problem-Solving**: Workflow design and complex automation scenarios
- **API Integration**: Multi-API orchestration with data transformation
- **Communication**: Clear documentation suitable for technical and non-technical stakeholders
- **Professional Delivery**: High-quality outputs demonstrating production-ready thinking

---

## Conclusion

This submission demonstrates a comprehensive understanding of QA principles, testing methodologies, and modern automation workflows. The work reflects the ability to identify production-impacting issues, communicate findings clearly, and design robust automation solutions that handle real-world complexity.

---

**Submission Date:** 2026

**Candidate:** Deep Saha

**Contact:** hiremeasadeveloper@gmail.com
