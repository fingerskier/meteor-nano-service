# meteor-nano-service
Nano service architecture for MeteorJS apps.

A simple element patterned after micro-services but on a smaller scale.  Basically, one template, it's control logic (client & server), routes, and model in 2 small files (plus css if needed).  This is a pattern that I'm coming to love as it helps to avoid crosstalk between application pieces that should be controlled separately.

If a particular nServ doesn't need routes or a model just remove that code.  By nature you can duplicate startup functions, pub/sub declarations (i.e. different filters on the same dataset), and route-targets without issue.  This focuses each nServ on doing one thing - it makes architecture and maintenance much easier.
