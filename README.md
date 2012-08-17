Drupal-Entity-Workflow
======================

Version : 7.x-1.0-dev

This currently provides a non-production development branch of an entity workflow module for Drupal 7

This is straight ahead of copy the excellent Workflow module by John VanDyk, with the idea of converting it over to work with Entities and not only just Nodes...

Insane possibly, but we have deadlines ;)

-------------------------------------------------------

Rework by @modernfidelity + @nano_monkey


@TODO :
-------

1. Transitions
Get this working today

2. Bundles - make mapping, transitions etc work with bundles not just parent entities
Start this today

3. Comments and Transition History

4. Scheduling

5. Tokens - how are these used? Do we need them?

6. GUI - is this ready?

7. Housekeeping:

- Constants - all upper case, currently: 'entity_workflow_CREATION'
- Crud/Helpers tidy up - order, replace nids with eids, $node with $entity etc etc
- DB schema tidy up - replace nids with eids etc etc

