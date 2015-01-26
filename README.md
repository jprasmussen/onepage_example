# One Page Site Example

This is an example theme of a one page site for Drupal 7. This is only intended
to be an example and I do not intend to support this as a production ready 
project. 

---
### Basic Drupal 7 Configuration

**Requirements:**
* Entity
* Entity Reference
* Inline Entity Form

You will need two content types. I used Basic Page as my first and created a second named Section.

**Section Fields and Display**
* Create a new content type and call it “Section” or what ever makes sense to you.
* Add an image field and call it “Background image”. No need to do extra configuration here. _However if you decide to call this field something else you need to update the node.tpl to use this field._ 
* Go to the Manage Display tab and move your background image to the disabled section and save. 

**Baisc Page Fields**
* Now on basic page create an entity reference field. 
* When creating this field choose the Inline Entity Reference Form as the widget.
* Configure this field to use the Section content type and allow it to create new nodes.
* Also set this to allow unlimited values (at the bottom in the global fieldset) and save.

**Baisc Page Display**
* Goto the manage display on the Basic Page.
* Hide the title of the entity reference field you just created.
* Change the field formatter to Rendered Entity
* Click the gear to the right of the field to manage it’s settings.
* Set this field’s view mode to default or full and uncheck show links. Save the settings.
* Now save the display settings. 

From here you should be able to create a new Basic Page and add Sections at the same time. The theme should correctly insert the background image on the respective sections. 

---

### Better Documentation
Please let me know if I need to clarify any of the above. Just threw this together so I am sure there is missing information.
