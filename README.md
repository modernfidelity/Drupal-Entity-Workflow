Drupal-Entity-Workflow
======================

Version : 7.x-1.0-dev

This currently provides a non-production development branch of an entity workflow module for Drupal 7

This is straight ahead of copy the excellent Workflow module by John VanDyk, with the idea of converting it over to work with Entities and not only just Nodes...

Insane possibly, but we have deadlines ;)

-------------------------------------------------------

Rework by @modernfidelity + @nano_monkey


@TODO :


1. Transitions

2. Bundles - make mapping, transitions etc work with bundles not just parent entities

3. Comments and Transition History

4. Scheduling

5. Tokens - how are these used? Do we need them?

6. GUI:
- Group Bundles by entity type. Add a checkbox to select individual bundles,
and one to 'Map to all' bundles.

7. Housekeeping:

- Crud/Helpers tidy up - order, replace nids with eids, $node with $entity etc etc
- DB schema tidy up - replace nids with eids etc etc
- Clean up entity API load, insert, save and delete hooks. All working but with warnings and notices.

8. Gotchas - things to watch out for.
Anywhere we are calling variable_get/set() for the placement information for a node.
I've made amends to how these are initially saved and loaded in the entity_workflow_admin_ui_types_form
but this is not the only place these variables are used so just bear this in mind. Could cause errors :S
Has not been thoroughly tested yet to be able to say whether these changes will break anything.

9. entity_workflow_form_alter() needs amending

10. The workflow tab - need to make sure this is bulletproof for nodes and isn't broken for other entities