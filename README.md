Drupal-Entity-Workflow
======================

Version : 7.x-1.0-dev

This currently provides a non-production development branch of an entity workflow module for Drupal 7

This is straight ahead of copy the excellent Workflow module by John VanDyk, with the idea of converting it over to work with Entities and not only just Nodes...

Insane possibly, but we have deadlines ;)

-------------------------------------------------------

Rework by @modernfidelity + @nano_monkey


@TODO :


- Node stuff - make sure we haven't broken any of the node functionality we get for free with workflow - i.e. form widgets for the workflow changes on node edit form, the workflow tab on the node page etc etc

- Comments and Transition History

- Scheduling

- Tokens - how are these used? Do we need them?

- GUI - Group Bundles by entity type. Add a checkbox to select individual bundles, and one to 'Map to all' bundles.

- Housekeeping: Crud/Helpers/DB Schema tidy up - replace nids with eids, $node with $entity etc etc

- entity_workflow_user_delete() needs amending

- entity_workflow_form_alter() needs amending

- The Node page workflow tab - need to make sure this is bulletproof for nodes and isn't broken for other entities

- TEST TEST TEST!

Gotchas - things to watch out for:

Anywhere we are calling variable_get/set() for the placement information for a node.

I've made amends to how these are initially saved and loaded in the entity_workflow_admin_ui_types_form
but this is not the only place these variables are used so just bear this in mind.

Could cause errors :S Has not been thoroughly tested yet to be able to say whether these changes will break anything.