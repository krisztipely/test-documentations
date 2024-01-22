# Functional Test Scenarios for Event Management System

## Event Creation

**Scenario: Successfully Create Event**

Steps:
- Log in to the "Event Organizer Interface."
- Provide all mandatory information (Event Name, Date and Time, Location, Organizer's Name, Organizer's Email, Event Description, Event Type, Ticket Types, and Pricing).
- Click on the "Create Event" button.
  
Expected Result: Event is successfully created, and a confirmation popup appears.

**Scenario: Incomplete Event Creation**

Steps:
- Log in to the "Event Organizer Interface."
- Provide incomplete information (e.g., miss Event Name).
- Click on the "Create Event" button.
  
Expected Result: Alert message appears, highlighting the mandatory fields that need to be filled.

**Scenario: Email Validation**

Steps:
- Log in to the "Event Organizer Interface."
- Enter an incorrect email format in the Organizer's Email field.
- Click on the "Create Event" button.
  
Expected Result: Alert message prompts, stating: "Please ensure the correctness of your email: yourname@example.com."

## Email Notifications

**Scenario: Successful Event Creation Notification (Organizer)**

Steps:
- Successfully create an event.
  
Expected Result: Popup notification confirms successful creation, and an email is received by the organizer with event details and a confirmation link.

**Scenario: New Event Creation Notification (Admin)**

Steps:
- Successfully create a new event.
  
Expected Result: Administrator receives an email notification with details and a link to approve/disapprove the event.

**Scenario: Approval Notification (Organizer)**

Steps:
- Administrator approves the event.
  
Expected Result: Organizer receives an email notifying them that the event registration has been approved, along with a link to manage the event.

## Error Handling:

**Scenario: Password Mismatch**

Steps:
- Log in to the "Event Organizer Interface."
- Enter a password and its confirmation with a mismatch.
- Click on the "Create Event" button.

Expected Result: Alert message appears, stating: "Passwords do not match."

**Scenario: Empty Mandatory Field**

Steps:
- Log in to the "Event Organizer Interface."
- Leave a mandatory field empty (e.g., Event Name).
- Click on the "Create Event" button.
  
Expected Result: Alert message appears, indicating: "This is a mandatory field; please fill it for registration."

## Clarifying Questions:

Question: What is the maximum length for the Organizer's Name and Ticket Types?

Question: Can multiple ticket types be added with the same pricing?

Question: Is there a specific format for the Event Date and Time?

Question: What steps should I take to approve or disapprove an event?

Question: Are there any limitations for creating events?

## Additional Notes:

The event should not be publicly accessible before approval.

Automatic message sent to the user upon approval.
