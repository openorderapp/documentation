**Open Order Project Plan**

1. Write an overview of Open Order. Include as topics:
  1. Description
  2. User identities
  3. Other System elements
  4. User stories
  5. Wireframe/Sample Screens
  6. Software/Hardware/Services required.
  7. Testing Requirements
  8. Other requirements, questions, comments and concerns
    1. List in a &quot;brainstorming&quot; format

**Open Order User and Developer Guide**

**Description**

Open order is a software product that is used in a business to track value generated through interactions with customers. Of the 12 possible ways to generate income through a business (Josh Kaufman: [https://personalmba.com/12-standard-forms-of-value/](https://personalmba.com/12-standard-forms-of-value/)), Open Order will deal with all 12.

Method 2, Service, will be addressed first, in this proposed version.

The business in question has employees who perform a service on items owned by its customers. The business makes money by providing that service and charging the customers for the value they add.

Other methods to produce value will be addressed in future versions of this software.

**User Identities and Other System Elements**

An **administrator** is a user that can access, view and change anything in Open Order. They can update the input fields of the order, create new structures in it,and even change the configuration of the application. An administrator can &quot;open&quot; (add) one or many new businesses to the system.

An **employee** is a user in the business who interacts with customers. A business will have one or more employees. An employee collects the necessary information to do the work on the customer&#39;s goods. An employee also does the work on the customer&#39;s goods. An employee notifies the customer that the work is completed so that they can return to the business to pay for the service and pick up their improved or modified goods.

An employee collects payment due from customers against a statement.

A **customer** is someone who brings their goods to the business to be altered. One customer can have multiple items to be serviced. A customer can result in the generation of one or more invoices. It is considered that a customer will not be using the software directly, but will be sent reports, in the form of claim checks, notifications, invoices and statements.

A business **owner** is a special type of employee who has all the abilities of an employee, but can, in addition, access a business summary.

An **order** is a document that traces the movement of customer property, the work done on that property, the return of the customer&#39;s property, and payment for the service performed. The order details provide the basis of all generated reports.

A **claim check** is a (small) report provided to a customer when goods are dropped off at the business so that they can reclaim their goods after the service is performed. The claim check also provides proof that the customer&#39;s goods were received by the business, and facilitates retrieving them.

A **notification** is a report sent to a customer when the service work is completed.

An **invoice** is a report presented to a customer for payment due for one service performed. It summarizes that work and the payment expected from the customer for one instance of the service.

A **statement** is a report that summarizes a customer&#39;s invoices for a given time period. It presents an amount due to be paid at a given point in time (typically &quot;now&quot;). A statement can be generated automatically at the end of a given time period, and/or on demand.

A **business summary** report shows the total value of all the work performed and invoiced in a chosen time period for all customers. It includes the total amount of invoiceable work, and the value of funds generated and funds received for any work in that time period (a day, month, week, year or custom time interval). Only an owner or administrator can generate or view a business summary.

**User Stories**

As an **employee** , I want to:

- Validate myself as an authorized user of the system.
- Enter the details to create a new customer record.
- Enter the details of a customer order, with sufficient detail for processing.
- Generate a claim check for the customer&#39;s goods.
- Use the returning customer&#39;s claim check to find his processed goods.
- Generate a statement for a customer so that they can pay for the services provided.
- Collect funds from the customer.
- Provide proof of payment to the customer.

As an **administrator** , I want to:

- Do all tasks that an employee can do
- Generate a business summary for a period of time that interests me, to show how much business has been invoiced, and how much income is still outstanding.
- Update the input fields of the order
- Have full visibility of all aspects of the system.

**Wireframe/Sample Screens**

1. **Login: authentication and authorization.**
2. New Customer creation
3. **Order generation**
4. Claim check generation
5. Order tracking
6. Invoice generation
7. Statement generation
8. Business summary generation

**Software, Hardware, Services Requirements**

Front end: HTML5, CSS3, JavaScript, React(?)

Back end: SQL(?)

Testing Requirements

Test on Chrome, FireFox, Edge

Hosting: ?

**Other requirements and questions, comments, concerns (prioritized, somewhat):**

A database is needed to track customers&#39; property - of course. Noted in the Guide.

Need a super user that can see everything in the system - this is the Administrator.

Who are the users? - answered in the Guide (for now).

Is the user in a storefront or online? (does it matter?) - a storefront for now

Is the user the same person as the machine operator? - yes for now, but it needs to be thought of as a separable identity.

Name the inputs required to work on the customer&#39;s goods and the type of software elements they might suggest. (eg. radio buttons, textbox, etc.)

Now that we know the inputs needed for the work order (assuming the question above is answered fully and correctly), what inputs are needed to return goods and to invoice the customer. (do we need just the input fields plus some comments from the employee?)

What is Open Order? - that&#39;s what the Guide is for.

Who is using Open Order? - mainly the employee, but see the guide.

What does Open Order do? - see the Guide.

What software components will the system have?( Web server (API), database, front end)

What languages are the components written in?

Where are they stored?

What is the workflow?

What types of orders are there in business?

- Change state of customers&#39; goods
- Sell / buy something
- Personal service to customer
- Store customer goods
- Rental
- Manufacture goods for sale
- Distribution of goods
- Wholesale or retail?

Which type will we be concerned with?

- Change state of customers&#39; goods

What does the financial part of all this look like? (just orders, invoices and statements for now)

But what does the price piece look like? Just a simple price? Is any costing involved? (No, just a flat fee per task?)

What does payment look like? Debit? How? Need to interface with interac for example? (No)

Where are orders stored? (a db)

Where are customers&#39; goods stored? Are we tracking them? (our shelving for the time being)

What does it mean to have an order management system &quot;for everyone&quot;?

What tools will we use to build the project? Software? Hardware? Services?

What tools will we use to describe or present our work? (this document. Other progress reports. At what interval?)

If we send a customer an invoice by email, might he want a printed copy too, on the spot?

Are a work order and an invoice the same thing? (No, an order tracks all activities of the system. An invoice is a report generated from a work order once the product alteration is complete)

Who is &quot;everyone&quot;?

How do we prove that goods have been returned to a customer? (a zero dollar invoice?)

Is a work order number the same as an invoice number? (Do accountants need sequential invoice numbers?)

Should Open Order track the hours worked and payment made to the employee? (No.)

How will we charge for the service?

Will Open Order track anything related to the service other than the cost of performing it, and whether or not the work is complete?

If work orders and invoices are not the same thing, how are they related? (Orders are a parent form for an invoice report)

Will Open Order track customer financials (total amount owed, etc.)?

Who can access Open Order? (customer? employee? administrator?)

What else in the business should be tracked? (hours worked? Time taken to perform the service? Due dates of return goods to customers?)

What about customers who never come back to claim their goods? (not dealing with this at this time)

How will we network this?

NB: Mobile first.

How to notify customers for pick up (SMS at first; other methods later?).

How is the work priced? (fixed, hourly, custom?)

How are payments received? (credit card, terminal, cash?)

Do we need both an owner and an administrator? (No, I don&#39;t think so)

What about unpaid invoices and unclaimed goods? (for now, addressed by the generation of statements)
