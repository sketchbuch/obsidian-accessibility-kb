# Accessibility Tree

The accessibility tree contains accessibility-related information for most HTML elements and is derived from the [DOM Tree](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model).

---

The tree is a series of nodes that represent parts of a web page that are exposed to accessibility APIs. Each node has the following parts:

1. **Name**
   A label that is communicated to [[Assistive Technologies]]
2. **Role**
   The [[ARIA]] [role](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles) that the node represents.
3. **Description**
   This is optional, but could give more information about the node to users.
4. **State**
   The state is built using [[ARIA]] attributes to help communicate information to users. An example of state could be the min, max, and current values of an amount picker.

An example node for a button might be:

| Attribute   | Value                                                 |
| ----------- | ----------------------------------------------------- |
| Name        | Go to Basket                                          |
| Role        | button                                                |
| Description | View your shopping basket and complete your purchase. |
| State       | -                                                     |

The tree's information is communicated to [[Assistive Technologies]] via platform specific accessibility APIs.