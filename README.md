You will want to save the html and css files in the same folder separate from other demos to avoid conflicts

Required Edits
Line 5 - update the title of the page
Line 21 - update logo/pic URL.  Pay attention to inline notes/directions re: using a screen grab of a nav bar that needs to be full width
Line 23 - update header text.  This can be deleted if you don't want to use it

Other than that, you need to update your role names for any roles you want to pass over.  Look for any of the UserName or Email inputs.  You want to update Signer 1, Signer 2, etc to what ever your role names are in the "name" parameter of the input.
You don't need to touch the "id" or the "for" in the labels.

In the fields, you'll want to edit "tablabel" or "groupname" to whatever your tag label is in your template.

If you need more inputs, just copy and paste the entire "form-group" div that surrounds a control and make the edits you need to the new input.
Example, I copy the included text field input:
<div class="form-group">
  <!-- Edit Signer 1 below to something meaningful to your demo.  The change should be made in the label as well as the "name" value prior to the first underscrore. -->
  <label for="signer1_tabLabel">Signer 1 Text Field:</label>
  <input type="text" class="form-control" id="signer1_tabLabel" name="Signer 1_tabLabel" required="required">
</div>

I would edit this to read the following if my Role was "Customer" and the tag was "streetAddress":
<div class="form-group">
  <!-- Edit Signer 1 below to something meaningful to your demo.  The change should be made in the label as well as the "name" value prior to the first underscrore. -->
  <label for="signer1_streetAddress">Customer Street Address:</label>
  <input type="text" class="form-control" id="signer1_streetAddress" name="Customer_streetAddress" required="required">
</div>

IDs need to be updated so there aren't duplicates.

The demo.css file gives you a quick place to go change some easy formatting options.  Notes included inline.

Hit me up if you have questions.

Rob

