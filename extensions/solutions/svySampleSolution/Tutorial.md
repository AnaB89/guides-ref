# Tutorial Part 1

Welcome to the Servoy Tutorial !

This tutorial introduces you to the essentials of Servoy by walking you through building a simple Web Application with a product catalog.

## Create your first grid

In this step of the tutorial, you will become familiar with some of the Servoy basics. You will build a product catalog and learn how to build a form having a feature rich grid, inheriting an existing form.

![Product Catalog](images/2020-01-17\_1415.png)

### Introduction

The Servoy sample solution, cloudSampleSolution is the starting point for this tutorial. You will be walked through how the solution has been built creating new user interfaces, new features, learning the basic Servoy techniques. Make sure your environment is properly setup to start this journey. You need the Servoy sample database and the Servoy Sample solution to be your active solution.

![Initial Setup](images/2020-01-17\_1412\_1.png)

### Create Form

You will now create the product catalog as your first grid Form. To create a new Form, in the **Solution Explorer** pane (left side), right-click the active Solution named _cloudSampleSolution_ and select **Create new form**.

:information\_source: _A Servoy **Form** is the object end-users can interact with in your application. You can compose your user interface using 1 or more Forms; you can nest Forms into each other and interchange them dynamically as the user operates with your application._

**Form Name**\


When creating a Form you need to enter an unique Form name. You can choose any form name that makes sense to you; however is suggested to use same naming proposed by this tutorial for convenience. Type "productsTableView" into the Form name.

**NOTE**: Despite the fact that you can choose any name, it is recommended to use the same naming of this tutorial since objects name will be referenced in future steps.

**DataSource**\
Secondly pick a Datasource for the form. The Datasource is an optional property of the form; as the name suggests a Datasource is a source of data. It can be an SQL table, a view or any other source of data (e.g. the result-set of a Web Service).

:information\_source: _When a Datasource is set for your form, it allows your form and the elements in it to bind to the Datasource data. By doing this, you can select its columns, calculations and aggregations as a "data provider" on form elements, so that record (a data entry item) values are automatically displayed and synchronized between the application and the source of data._

Let’s select the Datasource of your form, expand the _example\_data_ server and select the _products_ Datasource. You will be able to create the product’s catalog via data binding against the product’s table.

**Extends**\
Thirdly, let the Form inherit UI & business logic from the existing base Form _baseTableAdvanced_. Click Extends and select the super Form _baseTableAdvanced_.

:information\_source: _Servoy highly encourages reusability and extendability. The baseTableAdvanced Base Form has been created in the sample solution with the intent to be used as an extendable “template” for the grid interfaces created in the sample solution. It will offer base interface and base functionalities providing consistent look & feel and features across all grid interfaces. Note, any form can be extended; you can create anytime your own set of base For._

_Any Servoy Form can be extended and used at your best convenience; moreover, in the extended Form instance you will be able to modify and augment the base interface and base functionalities; as much as reusability is highly valuable, a high level of flexibility is also important in order to accomplish what a complex application may require._

![Create Form](images/2020-01-09\_1721.png)

Finally click on Finish, you will be prompted to the Servoy Form Editor. The Form Editor is a graphical user interface that allows users to quickly and easily create and modify Servoy Forms without the need for manual coding. In the following steps you will edit the productsTableView Form so you can build your product catalog.

#### Set title text

In your productsTableView, editable in the Form Editor, you will see with red dotted borders the Form’s Elements inherited from the baseTableAdvanced Form.

:information\_source: _A Form Element is an instance of a UI Component ( a reusable and encapsulated UI component with an unique behavior and appearance ). Every Element is configurable in the Form Editor Properties pane. Let’s now change the title of your new Form to something better suitable. The Label Component is a simple component which can display any text value._

Click onto the “Title” Element and in the **Property pane** (at the right side), change the value of the property text from 'Title' to 'Products Catalog' typing in it.

![Title Text](images/2020-01-09\_1740.png)

#### Grid's Column

Is now time to start modeling the UI for your product catalog; the base Form already has a Table Element which you can use to display the list of products. The Form created is bound to the product Datasource; you can add Columns in the Table element and set the data binding for each single Column.

In the Form’s **Editor Palette**, where all components are listed (left corner of the Form Editor), type “Data Grid” into the search box; drag the **column** item from the Palette onto the Table Element in Form to add a column into the grid.

Set the Column bindings in the **Properties pane** (right side). The first Column in Table will display the Product Name:

* Choose the dataprovider value of the Column; select productname.
* Set the headerTitle value; type 'Product'.
* Specify an unique id; type 'productname'.

![Add Column](images/2020-01-09\_1728.png)

#### Related Column

Add another Column onto the Table. The second Column will display the product’s Category type. Note, each product record has a categoryid which points to the id of the related Datasource categories. You can use the Relation object products\_to\_categories and bind the second Column to the related category’s name.

* Choose the dataprovider of the 2nd Column; select products\_to\_categories.categoryname.
* Set the headerTitle value; type 'Category'.
* Give the Column an unique id; type 'categoryname'.

#### Column with Valuelist

Add a third Column onto the Table to display the product’s supplier name. As like the categoryid, each product record has a supplierid pointing to the id of the related Datasource supplier. In the 2nd Column you have already used the relation object to display related values in grid. Let’s now learn something new and let’s use the suppliers Valuelist pattern to resolve the supplierid into the supplier’s name.

* Pick the dataprovider of the 3rd Column; select supplierid.
* Pick the Column’s valuelist, select the valuelist suppliers.
* Set the headerTitle value; type “Supplier”.
* Give the Column an unique id; type 'suppliername'..

The suppliers Valuelist will resolve the dataprovider value, supplierid, to the translated display value.

#### Edit Main Menu

The Form is now ready to be accessed to visualize the product catalog. Let’s add a new entry into the main menu. The main menu is a Sidenav Element of the Servoy Form _mainNavMenu_. Most of the application developed requires a menu that can be populated and manipulated dynamically; the menu can be indeed populated dynamically with a simple script.

In the SolutionExplorer right click the mainNavMenu Form and select **Open in Script Editor** to edit the Form’s script.

![Open Form Scripting](images/2020-01-17\_1417.png)

The base function _loadMenuItems_ of the _mainNavMenu_ Form returns a list of menu items; edit the function loadMenuItems to include the new Product menu item. You can place the new Product menu item at any position; in this sample is placed as 2nd menu item right after the Home menu entry.

```
function loadMenuItems() {
	...

	// HOME
	menuItem = new Object();
	menuItem.id = "homeDashboard";
	menuItem.text = "DASHBOARD"
	menuItem.iconStyleClass = "fa fa-th-large";
	menuItems.push(menuItem);
	
	// PRODUCTS
	menuItem = new Object();
	menuItem.id = "productsTableView";
	menuItem.text = "PRODUCTS"
	menuItem.iconStyleClass = "fas fa-shopping-basket";
	menuItems.push(menuItem);

	// CUSTOMERS
	....

}
```

#### Launch the Client

You can click **Launch NG Client** to see the result of your work. Click the newly created PRODUCTS menu option to see in action your new product catalog.

You have performed few simple steps to get that far. Let's make few more simple and enhance your catalog.

### Other Column Properties

Is very simple to enhance your product catalog with nice extra features. In the following steps you will learn how to format columns and advanced filtering. Add more Columns onto the Table with relevant information: Unit Price, Quantity per Unit and Units in Stock. Format the the value of the unit price and the units in stock using the Column’s Format Property.

#### Format Data

Add more Columns onto the Table with relevant information: Unit Price, Quantity per Unit and Units in Stock. Format the the value of the unit price and the units in stock using the Column’s Format Property.

Add new Column for Unit Price:

* Pick unitprice as the dataprovider of the Column.
* Set the headerTitle value; type 'Unit Price'.
* Set the Column format value to ¤#.00.
* Change the Column width value; type 100.
* Give the Column an unique id; type 'price'.

Add new Column for Quantity per Unit:

* Pick quantityperunit as the dataprovider of the Column.
* Set the headerTitle value; type 'Quantity p/u'.
* Give the Column an unique id; type 'quantityperunit'.

Add new Column for Units in Stock:

* Pick unitsinstock as the dataprovider of the Column.
* Set the headerTitle value; type 'Units in Stock'.
* Set the Column format value to #,###.
* Set the Column width value; type 80.
* Give the Column an unique id; type 'unitsinstock'.

#### Column Filters

In Servoy there are multiple ways to filter data. To start with let’s use the default configuration of the Toolbar Filter Component.

:information\_source: _The Toolbar Filter Component provides out-of-the-box modern UX patterns to filter data in a grid; is also extensible allowing customizations and other UX patterns and filter types._

In the base Form, which your productsTableView is extending, the Table Element is already connected with the Toolbar Filter Component. Column filter is enabled via the FilterType property; set the FilterType for the column and will be available in the filter toolbar.

:information\_source: _Note the advanced filters applied by the end-user will be persisted and restored at the next login for the same user._

Select the following Columns in Table and set the Column Property filterType as suggested below:

* Productname: set filterType to TEXT
* Category: set filterType to TEXT
* Supplier: set filterType to TEXT
* Price: set filterType to NUMBER
* Unitsinstock: set filterType to NUMBER

#### Multiselect Filter

Note the category filter behaves differently compared to the supplier filter; the supplier filter makes use the of valuelist Column property, which you have already set before, to populate the list of available options. The end user can pick from the list which values to filter on.

What about the product’s category ? Let’s change the category Column so that you can provide the same user experience given with the supplier filter.

Edit the category column as follow:

* Change the selected dataprovider from products\_to\_categories.categoryid to categoryid.
* Pick the Column’s valuelist: select the valuelist categories.

#### Launch the Client

You can click **Launch NG Client** to see the result of your work. Click the newly created PRODUCTS menu option to see in action your new product catalog.
