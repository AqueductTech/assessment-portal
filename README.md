# Aqueduct Cloud Assessment - Onboarding Portal

Public, client-facing pieces of Aqueduct's cloud assessment onboarding.

- `index.html`: the page a client administrator lands on after approving
  the read-only assessment application. Served via GitHub Pages at
  `https://aqueducttech.github.io/assessment-portal/`.
- `lighthouse.json`: an Azure Lighthouse template that grants Aqueduct
  three READ-ONLY roles (Reader, Security Reader, Cost Management Reader)
  on subscriptions a client chooses to include. Deployed through a
  "Deploy to Azure" button; visible and removable at any time under
  Service providers in the client's Azure portal.

Everything granted through this portal is read-only. Aqueduct cannot
create, change, or delete anything in a client tenant or subscription.
Clients can revoke all access themselves at any time: delete the
"Aqueduct Cloud Assessment - Read Only" enterprise application in Entra,
and remove the Aqueduct entry under Service providers in the Azure portal.

Questions: contact your Aqueduct engagement lead.
