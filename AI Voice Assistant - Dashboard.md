# AI Voice and Chat Dashboard Document

This comprehensive handbook contains all essential information for Admin users of the platform, including dashboard operations, QA responsibilities, project workflows, and company policies. This document is designed for independent learning without requiring external explanation.

***

## 1. Dashboard Access \& User Management

### Dashboard Environments (Login URLs)

- **Staging Environment:** https://auth-staging.liaplus.com/auth/login
Used for testing features before they go live in production.
- **Production Environment:** https://auth.liaplus.com/auth/login
Used for all everyday work and live operations.


### User Roles \& Access Permissions

- **SuperAdmin:** Possesses global rights with unrestricted access to all organizations and assistants in the system. Can manage, modify, and oversee everything across the platform.
- **Admin:** Has limited access to only the organizations and assistants specifically assigned by the SuperAdmin. Cannot view or manage assistants or organizations without explicit permission.

**Important Note:** Before raising any access-related issues, verify with your SuperAdmin whether you have been granted the necessary permissions for that specific assistant or organization. This prevents time wastage for all team members.

***

## 2. Main Dashboard Overview \& Metrics

When you log into the platform, the main dashboard displays comprehensive performance metrics for all assistants under your management:

### Core Metrics

- **Total Call Duration:** Cumulative time spent on all calls across your assigned assistants.
- **Total Calls:** Complete count of calls made or received by your assistants.
- **Call Abandonment Rate:** Percentage of callers who disconnected before receiving assistance—higher rates may indicate excessive wait times or caller frustration.
- **Transfer Rate:** Percentage of calls that were transferred to another assistant or human agent.


### Detailed Call Analysis

The dashboard provides breakdown of key performance indicators:

- **Call Transferred:** Exact number of calls passed to other agents or departments.
- **Goal Achievement:** Whether the primary objective of each call was successfully completed.
- **User Satisfaction:** Measurement of caller satisfaction levels based on interactions.
- **SOP Adherence:** Compliance rate with Standard Operating Procedures during calls.
- **Call Adherence Risk:** Risk assessment of missing required procedural steps.
- **Average Handle Time per Assistant:** Mean duration each assistant spends handling individual calls.
- **First Call Resolution (FCR) per Assistant:** Number of issues resolved during the initial interaction without requiring follow-up calls.
- **Assistant Performance:** Comprehensive view showing call volume, handling time, and cost metrics for each assistant.

***

## 3. Assistant Management

### Sidebar Navigation - Assistants Section

The sidebar displays all assistants assigned to you or created within your account. From this section, you can create new assistants for clients or internal use, either using pre-built templates or building from scratch.

### Assistant Metrics Tab

This tab displays data only for existing assistants that have handled actual calls:

- **Total Calls:** Number of calls managed by the specific assistant.
- **Average Handle Time:** Mean duration of calls handled by the assistant.
- **Abandonment Rate:** Percentage of callers who disconnected before speaking.
- **Words Per Minute:** Conversation pace during calls.
- **Detailed Call Analysis:** Including transfer rates, goal achievement, satisfaction scores, SOP compliance, resolution rates, AI-to-human handover frequency, peak traffic hours, and handle time by issue category.


### Creating New Assistants

#### Information Tab Configuration

- **Assistant Name:** Clear, descriptive name for identification.
- **Category:** Type of issues handled (sales, IT support, customer service, etc.).
- **Call Type:** Specify inbound (incoming) or outbound (outgoing) call handling.
- **Description:** Detailed explanation of the assistant's purpose and functionality.
- **Image Upload:** Visual identifier for easy assistant recognition.


#### Prompt Section Setup

- **First Message:** Opening greeting from the assistant to callers.
- **Prompt Definition:** Comprehensive description of the assistant's use case and expected behavior.
- **Generate Prompt:** Auto-generation feature requiring complete, specific instructions (e.g., "Create a prompt for school admission inquiries that captures student contact details and program interests").
- **Assistant Goals:** Clear, measurable objectives (e.g., "Achieve 90% customer satisfaction rating").
- **End Message:** Professional call closure message.
- **Provider Selection:** Choose the Large Language Model (LLM) provider.
- **Model Selection:** Select specific version of the chosen LLM.
- **Knowledge Base Upload:** Add supporting documents in CSV, DOC, or PDF format (must be machine-readable text, not scanned images as OCR is not supported).
- **Max Tokens:** Controls response length and detail level based on model capabilities.
- **Temperature Setting:** Adjusts creativity and variation in assistant responses.


#### Helpful Resources

- **Prompt Structure Guide:** https://learnprompting.org/docs/basics/prompt_structure
- **ChatGPT Prompt Guide:** Provides comprehensive role and workflow structure information.
- **Sample Prompts Available:** UPES Call prompt, MetalBook Prompt, Template Prompts, ABC Bank Sample Scripts, LiaPlus Dashboard Sales and Capabilities Knowledge Base.


#### Live Client References

- **MetalBook:** E-commerce platform assistant.
- **Meity Startup Hub:** Digital India Corporation initiative.
For any modifications to these live clients, contact one of the Founder members for authorization and implementation.


### Speech Processing Configuration

#### Transcriber Section (Speech-to-Text)

- **Provider:** Select speech-to-text service provider.
- **Model:** Choose specific STT engine version.
- **Language:** Set primary language for audio processing.


#### Voice Section (Text-to-Speech)

- **Provider:** Select text-to-speech service provider.
- **Model:** Choose specific TTS engine version.
- **Voice Name:** Select voice characteristics (gender, accent, tone).
- **Background Sound:** Enable or disable ambient audio.
- **Speed Control:** Adjust speaking pace (slow, normal, fast).


### Configuration Settings

#### Left Side Controls

- **Interruption Level:** Sensitivity to caller interruptions during assistant speech.
- **Cutoff Flag:** Determines whether assistant stops mid-sentence when caller speaks.
- **Ideal Response Time:** Natural pause duration before assistant responds to maintain conversation flow.


#### Right Side Controls

- **End Conversation on Goodbye:** Automatically terminates calls when farewell phrases are detected.
- **Human Verification Checks:** Number of confirmations required before executing actions.
- **Cut Off Response:** Custom message delivered if assistant is interrupted mid-sentence.


### Actions \& Automation

#### Available Action Types

- **Send Email:** Automated email or SMS dispatch during calls.
- **Call Transfer:** Seamless handoff to human agents or specialized departments.
- **Data Extractor:** Intelligent extraction of key information (names, dates, contact details) from conversations.
- **Live Booking:** Real-time appointment or slot reservation capabilities.
- **Custom Actions:** API-integrated workflows tailored to specific business needs.


#### Action Configuration Details

- **Action Name:** Descriptive title for the workflow (e.g., "Schedule Appointment").
- **Description:** Clear explanation of action functionality.
- **Input Schema:** Required data fields and format specifications.
- **API URL:** Endpoint for data transmission and retrieval.
- **Data Schema:** Structure and format for information exchange.

**Critical Reminder:** Always click "Publish" after creating or modifying any assistant to save changes.

### Assistant Testing \& Sharing

#### Testing Methods

- **Direct Testing:** Use headphone icon for immediate testing.
- **Assistant View:** Access through "View Assistant" > "Try Assistant" for detailed testing interface.
- **Available Modes:** Web calls (browser-based), phone calls (when phone number is assigned).
- **Unavailable:** Live chat is not currently supported in the testing drawer.


#### Secure Sharing Options

- **Password Protection:** Require authentication for shared link access.
- **Expiration Settings:** Set specific date and time for link deactivation (maximum 7 days).
- **Usage Limits:** Restrict calling minutes available through shared link (maximum 100 minutes).
- **Link Management:** Generate, copy, and distribute secure access links.

***

## 4. Phone Number Management

Phone numbers must be assigned by SuperAdmin and can be provided through CZentric or Twilio services.

### Inbound Call Configuration

- **Phone Number Display:** Shows assigned number (e.g., +1 320-373-1508).
- **Automatic Handling:** Toggle for automated call answering.
- **Assistant Assignment:** Select which assistant handles incoming calls.
- **Fallback Number:** Backup number for calls when assistant fails to respond.


### Outbound Call Setup

- **Assistant Selection:** Choose assistant for making outbound calls.
- **Number Entry:** Manual input of recipient phone numbers (press Enter after each entry).
- **Call Initiation:** Start outbound calling process.


### Bulk Outbound (Feature in Development)

- **Contact Upload:** CSV, XLS, or XLSX file support for mass calling campaigns.
- **Automated Calling:** System-managed outbound calls to entire contact lists.
- **Scheduling:** Time-based campaign management (currently inactive pending full development).

***

## 5. Call Logs \& Analysis

The call logs section provides comprehensive records of all assistant interactions, including successful connections and failed attempts.

### Call Record Details

- **Assistant Name:** Identifies which assistant handled the call.
- **Call Type:** Source classification (Web for browser calls, Inbound for incoming, Outbound for outgoing).
- **End Reason:** Termination cause (currently shows "Not Available" when specific reason isn't captured).
- **Phone Number:** Associated number (shows "NA" for web-based calls).
- **Call Duration:** Exact time length (e.g., "22 secs," "1 min 53 secs").
- **Timestamp:** Precise start time and date of the call.


### Detailed Call Analysis Drawer

#### Info Tab

Displays basic call information including assistant name, unique call ID, call type and status, phone number involvement, total duration, and termination reason.

#### Transcript Tab

Complete conversation transcript in text format for thorough review of assistant-caller interactions and accuracy assessment.

#### Analysis Tab

Comprehensive call evaluation including:

- **Conversation Analysis:** Summary of discussion topics and outcomes.
- **Goal Achievement Status:** Whether assistant successfully fulfilled caller's primary request.
- **Follow-up Requirements:** Notes on any necessary post-call actions.
- **Transfer Information:** Details if call was escalated to human agents.
- **Resolution Timeline:** Speed of issue resolution.
- **User Satisfaction Measurement:** Caller happiness assessment.
- **SOP Compliance Rating:** Adherence to standard operating procedures.

***

## 6. Subscription Plans \& Billing

### Plan Status Overview

The sidebar displays current usage statistics, plan type, and available upgrade options. API documentation is accessible for developers requiring integration information.

### Available Plans

- **Free Plan:** Limited calling minutes with single concurrent call capability—ideal for initial testing and evaluation.
- **Standard Plan:** Basic monthly subscription with moderate minute allocation and cost-effective pricing.
- **Premium Plan:** Enhanced minute allowance with multiple simultaneous call support—optimized for team environments.
- **Business Plan:** Large-scale usage designed for companies with high call volumes and advanced feature requirements.
- **Enterprise Plan:** Fully customized solutions requiring direct sales consultation for pricing and feature specifications.


### Payment Processing

The checkout system allows plan confirmation, secure card and billing information entry, and subscription activation through Stripe's secure payment gateway.

***

## 7. User Account Management

### Feedback System

Located in the top-right corner, the feedback form enables users to submit:

- **Contact Information:** Full name, phone number, and email address.
- **Categorization:** Bug reports, feature requests, or general comments.
- **Detailed Messages:** Comprehensive description of feedback or issues.
- **Submission Options:** Submit completed feedback or cancel without sending.


### User Menu Options

- **Profile Access:** Personal account settings and information management.
- **Organization Settings:** Company-level configuration and team management.
- **Currency Selection:** Future feature for billing currency modification.
- **Secure Logout:** Safe account session termination.


### Profile Management

#### General Information

View and edit personal details including name, role, email address, profile picture, onboarding date, and organizational affiliations.

#### Security Settings

Password management allowing secure updates by entering current and new password combinations.

#### Account Deletion

Permanent account removal requiring email confirmation—this action is irreversible and removes all associated data.

### Organization Administration

- **Member Management:** View, edit, and remove team members with role and contact information.
- **API Key Management:** Generate, view, and revoke secure access tokens for system integration.
- **Subscription Upgrades:** Access and purchase organizational plan enhancements.
- **Security Verification:** Password confirmation required for API key generation to prevent unauthorized access.

***

## 8. Job Responsibilities \& Workflows

### Key Responsibilities

#### End-to-End Quality Assurance Ownership

As the designated QA professional, you maintain complete responsibility for quality assurance activities across all assigned projects and features. This encompasses bug detection, product reliability assurance, user satisfaction maintenance, and smooth release deployment oversight.

#### Proactive Bug Detection and Monitoring

- **Active Vigilance:** Maintain continuous surveillance for bugs, inconsistencies, and unwanted system behaviors across the entire product ecosystem.
- **Sprint Participation:** Actively engage in sprint rituals, daily scrums, and development progress meetings to stay current with emerging issues.
- **Initiative Testing:** Proactively test new features, integrations, and system changes immediately upon implementation.
- **Bug Tracking:** Maintain comprehensive records of bugs with regular status updates to ensure timely resolution.


#### Follow-up and Status Management

- **Regular Check-ins:** Conduct daily, weekly, and monthly reviews of reported bugs, ticket progress, and sprint objectives.
- **Cross-team Communication:** Actively communicate with developers, product managers, and fellow QA team members to ensure no issues are overlooked.
- **Backlog Management:** Review previous sprint issues and participate in backlog grooming with quality and triage considerations.


#### Project Management Tools

- **plane.so:** Primary tool for main product development tracking, QA ticket management, bug reporting, and sprint coordination.
- **Jira:** Additional tool used specifically for Food \& Beverage (FNB) projects, providing granular control and legacy ticket management.
- **Tool Proficiency:** Maintain current access credentials, utilize proper tagging and priority systems, ensure clear and reproducible documentation in all tickets.

***

## 9. Past Projects Handled

### Current Priority Project

**FNB –** This is the highest priority project requiring immediate and continuous QA attention. All testing efforts should prioritize FNB operational stability and feature correctness above other projects.

### Delivered Projects with Ongoing Maintenance

#### UPES EVENT – Completed

End-to-end QA has been completed including:

- Comprehensive event workflow testing
- Live testing during actual events
- Bug identification and resolution for attendee experience issues
- Feedback integration validation
- Periodic regression checks to prevent functionality deterioration


#### METALBOOK – Delivered with Active Monitoring Required

This e-commerce platform requires continuous monitoring and immediate response to emerging issues:

- **E-commerce Flow Testing:** Transaction processes, cart functionality, checkout procedures
- **Payment Integration Validation:** Gateway connections, security protocols, transaction completion
- **Catalog Accuracy:** Product information, pricing, availability status
- **Communication Systems:** Call handling workflows and chatbot conversation management
- **Customer Support Features:** Help desk functionality, query resolution, escalation procedures


#### MEITY STARTUP HUB – Delivered with Compliance Oversight

Government-supported startup platform requiring ongoing attention to:

- **Regulatory Compliance:** Adherence to government standards and requirements
- **Data Integrity:** User information security, platform data accuracy
- **Onboarding Robustness:** Registration processes, user verification, platform access workflows


### Demo Preparation Responsibilities

Regular preparation and verification of demonstration environments:

- **Feature Showcase:** Ensure all features display and function as intended
- **Edge Case Testing:** Comprehensive testing of unusual or boundary conditions
- **Call Simulation:** Realistic recreation of actual user environment conditions
- **Stakeholder Readiness:** Guarantee error-free, professional demonstrations for clients and management

***

## 10. Assistant Creation and Call Recording Workflow

### Use Case-Based Assistant Development

For every test scenario, client requirement, or workflow requiring QA validation:

- **Design Phase:** Create detailed assistant specifications matching real-world usage patterns
- **Configuration:** Ensure assistant settings precisely reflect intended use cases (e.g., Metalbook customer support simulation, UPES EVENT enrollment query handling)
- **Testing Alignment:** Verify assistant behavior matches expected client interactions and business requirements


### Call Recording Management

#### Standard Download Process

- **Dashboard Access:** Use auth.liaplus.com to access call recordings immediately after test sessions
- **Mandatory Documentation:** Download all relevant call recordings promptly for evidence preservation, detailed analysis, and defect demonstration
- **Quality Assurance:** Ensure recordings capture complete interactions for thorough review


#### Technical Issue Resolution

- **Primary Contacts:** Immediately notify **AI Engineers** when dashboard download issues occur (broken links, missing files, incomplete downloads)
- **Backup Recording Method:** Use mobile device built-in call recording as temporary solution while technical issues are resolved
- **Security Measures:** Store backup recordings securely and confidentially
- **Documentation:** Log backup method usage in QA tracking tools with appropriate transparency notes


### Post-Recording Workflow

- **Initial Sharing:** Distribute recordings to **Founders** for evaluation and feedback
- **Approval Process:** Await formal approval before proceeding to next workflow stage
- **Demo Preparation:** Forward approved recordings to **Founders** for demo design and presentation preparation
- **Reference Resource:** Access demo materials and additional resources at https://linktr.ee/liaplusai
- **Mandatory Documentation:** Ensure every QA test session includes proper recording proof for traceability and historical reference

***

## 11. QA Execution Process

### Daily Testing Protocol

- **Systematic Testing:** Daily evaluation of assigned assistants, core functionality, integrations, and critical user paths
- **Release Prioritization:** Follow latest release notes and deployment changes to identify testing priorities
- **Regression Testing:** Parallel execution of existing feature validation alongside new feature testing
- **Sanity Checks:** Never skip basic functionality verification even on updated builds


### Test Case Development

Create comprehensive test cases for every feature or system change:

- **Preconditions:** Required setup steps and initial system state
- **Detailed Steps:** Clear, sequential actions for test execution
- **Expected Results:** Specific outcomes anticipated from test execution
- **Actual Results:** Documented observations during test execution
- **Edge Cases:** Unusual conditions, error scenarios, and alternative user flows
- **Reproducibility:** Clear language enabling any team member to replicate tests independently


### Ticket Management System

#### Comprehensive Ticket Creation

For every identified bug or improvement opportunity, create detailed tickets including:

- **User Stories:** Clear scenario descriptions from user perspective (who, what, why)
- **Acceptance Criteria:** Complete list of conditions required for "done" status including edge cases
- **Test Case Integration:** Link relevant test cases to tickets for tracking and retesting
- **User Impact Analysis:** Detailed explanation of affected user segments, severity levels, potential business losses, reputation risks
- **Supporting Documentation:** Screenshots, logs, call recordings, reproduction steps, and relevant attachments


#### Priority and Severity Management

- **Regular Review Sessions:** Scheduled meetings with **Engineering Manager** and **Reporting Manager** to discuss:
    - Business blocker identification and prioritization
    - Critical regression assessment
    - High-severity defect evaluation
    - User impact and business risk analysis
    - Sprint and release priority adjustments
    - Critical ticket visibility in planning tools


### Continuous Improvement Process

- **Post-deployment Analysis:** Analyze recurring defects to identify process improvement and automation opportunities
- **Retrospective Participation:** Provide feedback on defect prevention and early detection strategies
- **Documentation Updates:** Maintain current test cases after major releases and preserve comprehensive edge-case documentation
- **Process Enhancement:** Suggest workflow improvements based on recurring issues and team efficiency observations

***

**End of Complete Handbook**

This comprehensive document serves as your complete reference guide for all platform operations, QA responsibilities, and company policies. Keep this document accessible for ongoing reference and share it with new team members for consistent onboarding and training.

