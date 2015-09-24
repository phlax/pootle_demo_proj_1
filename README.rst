Pootle VCS config examples
==========================



GNU Style
---------

.. code-block:: ini

   [default]
   translation_path = gnu_style/po/<lang>.po
```

Directory layout
^^^^^^^^^^^^^^^^

::
   -- gnu_style
      |
      +-- po
          |
	  +-- en.po
	  |
	  +-- zu.po


Pootle layout
^^^^^^^^^^^^^


-- $project
   |
   +-- en
   |   |
   |   +- en.po
   |   
   +-- zu
       |
       +- zu.po



GNU Style - named folders
-------------------------

Config
^^^^^^

.. code-block:: ini
   [default]
   translation_path = gnu_style_named/po-<filename>/<lang>.po


Directory layout
^^^^^^^^^^^^^^^^

-- gnu_style_named
   |
   +-- po-example1
   |   |
   |   +-- en.po
   |   |
   |   +-- zu.po
   |
   +-- po-example2
       |
       +-- en.po
       |
       +-- zu.po


Pootle layout
^^^^^^^^^^^^^

-- $project
   |
   +-- en
   |   |
   |   +- example1.po
   |   |
   |   +- example2.po   
   |   
   +-- zu
       |
       +- example1.po
       |
       +- example2.po   

