===========================
eCommerce Attribute values 
===========================

.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/github-dhongu%2Fdeltatech-lightgray.png?logo=github
    :target: https://github.com/dhongu/deltatech/tree/15.0/deltatech_website_sale_attributes
    :alt: dhongu/deltatech

|badge1| |badge2| 

Features:
 - Afisare valori atribute in functie de produsele determinate

in website_sale.products_attributes
after:
<t t-foreach="attributes" t-as="a">
add
<t t-set="a_value_ids" t-value="a.value_ids.filtered(lambda v: v.id in value_ids.ids)"/>

replace t-foreach="a.value_ids. with t-foreach="a_value_ids.

**Table of contents**

.. contents::
   :local:

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/dhongu/deltatech/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed
`feedback <https://github.com/dhongu/deltatech/issues/new?body=module:%20deltatech_website_sale_attributes%0Aversion:%2015.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Terrabit
* Dorin Hongu

Maintainers
~~~~~~~~~~~

.. |maintainer-dhongu| image:: https://github.com/dhongu.png?size=40px
    :target: https://github.com/dhongu
    :alt: dhongu

Current maintainer:

|maintainer-dhongu| 

This module is part of the `dhongu/deltatech <https://github.com/dhongu/deltatech/tree/15.0/deltatech_website_sale_attributes>`_ project on GitHub.

You are welcome to contribute.
