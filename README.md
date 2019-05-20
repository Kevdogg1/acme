I have written the framework for a generic communications service that could be implemented for
multiple companies. 

I instantiate a service which has a generic model (TAllInformation) that contains all information necessary for the
communications. Various functions act on this model, which is associated with the service. All data is stored in
class lists.

It is not a perfect solution and I have not abstracted fully in places, but it hopefully demonstrates
various fundamentals.

The flow is as follows:

1) Check the company to execute for and the medium to employ (email for ACME)

2) Retrieve all information needed to construct the communications such as
   people details, email addresses, people to exlude etc.. Load into TAllInformation 

3) Adust the generic model data (TAllInformation) to tweek any data such as leap year changes in the case of ACME.

4) Exclude items identified in step 2.

5) Send the communications.
