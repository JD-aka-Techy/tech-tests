
FWG quick onboarding form
=========================

FinancialWellnessGroup comprises of multiple sub companies each with their own branding and call centres. As such each business entity has its own brand and marketing websites each requiring development and maintenance. Obviously creating multiple unique websites generally offering similar solutions from scratch would increase costs uneccesarily.

We are looking to create a relatively simple contact form for new customers which collects some basic contact information along with some location and debt data. This form should be usable on any of our websites and therefore be brandable based on where it is hosted.

Complete the stories in order. Please note there is no expectation that you will complete all of these tasks, this exercise is meant to show how you approach the problem.

Stories:
-----------------------------------------

**As a** FWG Customer relations manager

**I want** A simple contact form that collects the following information:

- customer forename
- customer phone number
- customers country of residence: England, NI, Scotland, Wales
- the total amount of debt the customer has 

**So that** I can collect customer information for new leads

-----------------------------------------

**As a** FWG Customer relations manager

**I want** The contact form to add a source identifier to the submitted customer information body depending on the brand and the amount of debt the customer is in.

**So that** I can direct the customer to the appropriate call center

- If the customer is in England, NI or Wales and has a debt of less than £10K, sourceid should equal 'lowdebt-default'
- If the customer is in England, NI or Wales and has a debt of more than £10K, sourceid should equal 'highdebt-default'
- If the customer is in England, NI or Wales and has a debt of more than £100K, sourceid should equal 'extremedebt-default'
- If the customer is in England, NI or Wales and has a debt of more than £10K, sourceid should equal 'highdebt-default'
- If the customer is in Scotland and has a debt of less than £10K, sourceid should equal 'lowdebt-scotland'
- If the customer is in Scotland and has a debt of more than £10K, sourceid should equal 'highdebt-scotland'

----------------------------------------

**As a** FWG Customer relations manager

**I want** The contact form to be styled based on the brand

**So that** The customer knows who they are dealing with

Given a JSON object is provided containing the following, the form should adjust to represent these brand styles:
- brandname - a header title "{brandname} is ready to help!!"
- primary colour - brandname and the submit button should be this color