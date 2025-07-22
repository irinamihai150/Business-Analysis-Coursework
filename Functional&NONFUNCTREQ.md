**Project Description**

Modernising the Loyalty Program within Brightstar

**Points of Contact**

Irina Mihai

**Document references**

 ( [https://tracks.codeyourfuture.io/business-analysis/sprints/2/prep/](https://tracks.codeyourfuture.io/business-analysis/sprints/2/prep/),https://tracks.codeyourfuture.io/business-analysis/prep/)

**Purpose**

This document details the functional and non-functional requirements for a digital application designed to improve the loyalty program among Bright Star Stakeholders. This application focuses on improving the existing loyalty program by providing digital features such as account creation, login, point tracking and redemption.

**Functional Requirements**

| ID | Functional Requirements | Testing Phase | Status |
| :---- | :---- | :---- | :---- |
| **FR1** | The system shall allow users to register for a loyalty account via a mobile-friendly interface | Test Case 1  | To be done |
| **FR2** | The system shall generate a digital loyalty card with a barcode  on a mobile or desktop | Test Case 2 | To be done |
| **FR3** | The system shall allow users to view their current loyalty points and rewards in real-time |  |  |
| **FR4** | The system  shall allow users to link an existing physical card to the digital account |  |  |
| **FR5** | The system shall support purchase functionality by linking to the existing online store |  |  |
| **FR6** | The system shall display the points the customer earned after the transaction |  |  |
| **FR7** | The system shall allow the user to log in with existing credentials |  |  |
| **FR8**  | The system shall receive customer transaction data from the existing POS or CRM systems in order to calculate and update loyalty points in real-time or near real-time. |  |  |
| **FR9** | The system shall allow users to reset their password. |  |  |
| **FR10** | The System shall calculate the point based on the purchase amount |  |  |

**Non-functional Requirements**

| ID | Non-functional requirements |
| :---- | :---- |
| **NFR1** | The system shall be mobile-responsive on all modern devices. |
| **NFR2** | The system shall be designed for integration into the existing website |
| **NFR3** | The system shall allow point updates in 10 seconds after the transaction |
| **NFR4** | The system shall use AWS for scalability |
| **NFR5** | The system shall send an email within 10 minutes confirming the successful creation of a new account |

**Project Scope: BrightStars Loyalty Program**  
**Project Objective**   
Will design a mobile-friendly interface for BrightStar that improves user engagement, enables digital sign-up, and real-time points tracking. The solution will be accessible via mobile devices and integrated into BrightStar’s existing web system.  
**Timeline:** 6 months from the start date, final application no later than 12 months from project approval.

**Deliverables:** Completed app.  
**Reports:** Project manager to provide weekly updates  
**Budget:** to be determined  
**Constraints:** 

- A major upgrade to the main accounts is planned next year.

**In scope**:

* Mobile-friendly interface for customer registration and login  
* Digital loyalty card generation  
* Real-time points tracking: earn, view and redeem.  
* Physical card linking to the digital account  
* Hosting the app on AWS or Azure

**Exclusions:** (Out of Scope)  
 Expand to the full e-commerce app  
 Improving the refund process.

**Application Features**

* The application should allow users to sign up & login via a mobile-friendly interface.   
* It will allow real-time loyalty point updates and tracking.  
* Digital loyalty card: Barcode  
* Points are redeemable at the checkout.  
* Personalised offers and notifications.  
* Card linking: option to connect an existing physical card

**System Overview**

* Secure and scalable system hosted on AWS  
* Built with a responsive design for mobiles  
* Focused on digitalising BrightStar’s loyalty experience for end users.  
* Secure account management and real-time points updates.

**Future Consideration**  
The stakeholders' feedback has identified pain points in the return items process, and this could be included in the next phase of the project. it is recommended as a second phase after the loyalty system is deployed.

Describe in your own words the differences between a use case, a scenario and a user story.

A user story is a statement used to document a feature or functionality that a user would like in a software application.  
 A use case is what the system does from the user’s point of view, and the functional requirements the system will support


**As a** buyer **I want** to be able to sign up **So that** I can access my loyalty account

### **Acceptance Criteria 1: Form Validation for Empty Fields**

Given that the user is on the sign-up page  
And the sign-up form includes the following compulsory fields: Title, First Name, Last Name, Email Address, Date of Birth, Password, and Confirm Password  
When the user leaves any compulsory field empty  
And clicks the "Submit" or "Sign Up" button  
Then the form should not be submitted  
And the user should see an error message indicating which field(s) need to be filled in

**Acceptance Criteria 2: Wrong Passwords**  
Scenario: User enters different passwords  
Given that the user fills all compulsory fields   
When the password and the confirm password do not match  
Then the form should not be submitted  
And the user should see an error message saying that the passwords are not the same.

**Acceptance Criteria 3: Invalid email format**  
Scenario: Users enter an incorrectly formatted email  
Given that the user fills all compulsory fields  
And the email address is not valid(missing  “@”)  
When the user clicks submit  
Then the form should not be submitted  
And the user should see an error message saying “Please enter a valid email address in the format [firstname.lastname@example.com](mailto:firstname.lastname@example.com)”

**Acceptance Criteria 4 Succesful Sign-up**  
Scenario : successful sign-up  
Given that the user fills all compulsory fields  
When the submit clicks the submit button for the form  
And clicks the sign-up button  
Then the user should be redirected to their account  
And the user should see a welcome message saying that sign up was succesfully.

**Acceptance Criteria 5 Form Loading Time**  
Scenario: Sign up form loads within 4 seconds  
Given the user is on the sign-up page   
When the page is loaded  
Then the sign-up form should load within 4 seconds.

| Id | User\_story |
| :---- | :---- |
| US1 | **As a** buyer, **I want** to be able to sign up **so that** I can access my loyalty account |

| Story\_ Id | Ac\_Id | Acceptance Criteria | Status |
| :---- | :---- | :---- | :---- |
| US1 | AC1 | Given that the user is on the sign-up pageAnd the sign-up form includes the following compulsory fields: Title, First Name, Last Name, Email Address, Date of Birth, Password, and Confirm PasswordWhen the user leaves any compulsory field emptyAnd clicks the "Submit" or "Sign Up" buttonThen the form should not be submittedAnd the user should see an error message indicating which field(s) need to be filled in  |  |
| US1 | AC2 | Scenario: User enters different passwords Given that the user fills all compulsory fields  When the password and the confirm password do not match Then the form should not be submitted And the user should see an error message saying that the passwords are not the same.  |  |
| US1 | AC3 | Scenario: Users enter an incorrectly formatted email Given that the user fills all compulsory fields And the email address is not valid(missing  “@”) When the user clicks submit Then the form should not be submitted And the user should see an error message saying “Please enter a valid email address in the format [firstname.lastname@example.com](mailto:firstname.lastname@example.com)”  |  |
| US1 | AC4 | Scenario : successful sign-up Given that the user fills all compulsory fields When the submit clicks the submit button for the form And clicks the sign-up button Then the user should be redirected to their account And the user should see a welcome message saying that sign up was succesfully. |  |

1. Suggest a list of epics for an improved solution within BrightStar

**Epics:**

* **Modernising the Loyalty Program**:  
   The goal is to make the loyalty program easier to use, so customers can sign up quickly, earn points, and use them whenever they want. I’d choose this first because it helps improve **customer engagement** and **feedback**. It’s also important because the competition already has modern loyalty systems, so we need to catch up.

* **Building a Full E-commerce App**:  
   This is about developing an app where users can buy products directly. The stakeholders said this is a key goal for the business. However, without a solid **loyalty program** and **customer engagement**, the success of the e-commerce app might not be as high.

### **Why Modernizing the Loyalty Program First?**

I think we should start with the loyalty program because it’s something that will bring value right away. It helps build a connection with customers, so they’ll be more likely to use the app and buy things later on.

| ID | Functional requirements(low-level) | High-Level Requirements | User Stories |
| :---- | :---- | :---- | :---- |
| **FR1** | The system shall allow users to register for a loyalty account via a mobile-friendly interface | The system shall enable seamless customer onboarding via mobile and desktop platforms to increase sign-up rates.  | **As a**  new customer, **I want to** register for a loyalty account using my mobile device, **so that** I can easily join the rewards program anytime and anywhere. |
| **FR2** | The system shall generate a digital loyalty card with a barcode  on a mobile or desktop device | Competitive edge |  |
| **FR3** | The system shall allow users to view their current loyalty points and rewards in real-time | Customer engagement |  |
| **FR4** | The system  shall allow users to link an existing physical card to the digital account | The platform shall allow linking of legacy (physical) loyalty cards to the new digital accounts to preserve existing point balances. | As an existing customer, I want to be able to link my card So that I can keep my existing points |
| **FR5** | The system shall support purchase functionality by linking to the existing online store | The loyalty system shall integrate with existing BrightStar system to ensure customer purchases |  |
| **FR6** | The system shall display the points the customer earned after the transaction | Real-Time Feedback |  |
| **FR7** | The system shall allow the user to log in with existing credentials | Improve Customer Experience |  |
| **FR8**  | The system shall receive customer transaction data from the existing POS or CRM systems in order to calculate and update loyalty points in real-time or near real-time. | Seamless Pos Integration |  |
| **FR9** | The system shall allow users to reset their passwords. | Improve Customer Experience |  |
| **FR10** | The System shall calculate the point based on the purchase amount | Automated Rewards System |  |

