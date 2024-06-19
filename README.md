# A Peter Burkholder project


In late 2022 the Office of Personnel Management changed the password policies for the employee self-service site Employee Express (at https://employeeexpress.gov), so employees and former employees were regularly getting locked out of access to their accounts, often with dire consequences for their ability to buy a house, get a loan or change jobs. 

A few colleagues and I raised concerns that not only was the policy having negative human impacts, but was also likely to have negative security consequences since a) employees would be much more likely to believe a phishing email saying “change your password NOW before it expires at midnight” and b) since Employee Express already has a redirect from employeeexpress.com to employeeexpress.gov, it made typo-squating attacks more likely than if there were no redirect. 

To demonstrate the ease with which such an attack could take place (and to convince myself) I set up a copycat domain and site (at employeexpresss.com), and shared it discreetly with a few folks with more influence on policy than I have. It helped make the case that a) the password change policy should be changed for sanity & security and b) the current transparent redirect from employeeexpress.com to employeexpress.gov is bad practice as it trains people to use the .com domain and make typosquatting attacks more likely.

While the site did mimic the look and feel of the Employee Express site, any attempt to use the site raised a pop-up notifying users it was fake site, which you can see in the code at: 

https://github.com/pburkholder/eex/blob/main/index.html#L205-L206
https://github.com/pburkholder/eex/blob/main/index.html#L244-L245

And, since the code was open-source, and tied to my identity, I was not exercising any of the OpSec that an actual attacker would employ – although I should have taken the time then, instead of now, provide a link back to a full explanation.
