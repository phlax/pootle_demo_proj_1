Pootle VCS config examples
==========================



GNU Style
---------

Configuration:

.. code-block:: ini

   [default]
   translation_path = gnu_style/po/<lang>.po


Directory layout::

   -- gnu_style
      |
      +-- po
          |
	  +-- en.po
	  |
	  +-- zu.po

Pootle layout::

  -- $project
     |
     +-- en
     |   |
     |   +- en.po
     |   
     +-- zu
         |
	 +- zu.po


++++


GNU Style - named folders
-------------------------

Examples:

- GTK - https://git.gnome.org/browse/gtk+/tree/


Configuration:

.. code-block:: ini

   [subdir1]
   translation_path = gnu_style_named_folders/po-<filename>/<lang>.po


Directory layout::

  -- gnu_style_named_folders
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


Pootle layout::

  -- $project
     |
     +-- en
     |   |
     |   +-- subdir1
     |       |
     |       +- example1.po
     |       |
     |       +- example2.po   
     |   
     +-- zu
         |
         +-- subdir1
             |
             +- example1.po
             |
             +- example2.po   

++++



GNU Style - named files
-----------------------

Examples:

- Tuxpaint


Configuration:

.. code-block:: ini

   [subdir2]
   translation_path = gnu_style_named_files/po/<filename>-<lang>.po


Directory layout::

  -- gnu_style_named_files
     |
     +-- po
         |
         +-- example1-en.po
         |
         +-- example1-zu.po
         |
         +-- example2-en.po
         |
         +-- example2-zu.po


Pootle layout::

  -- $project
     |
     +-- en
     |   |
     |   +-- subdir2
     |       |
     |       +- example1.po
     |       |
     |       +- example2.po   
     |   
     +-- zu
         |
         +-- subdir2
             |
             +- example1.po
             |
             +- example2.po   

++++


Non-GNU style
-------------


Configuration:

.. code-block:: ini

   [subdir3]
   translation_path = non_gnu_style/<lang><directory_path>/<filename>.po


Directory layout::

  -- non_gnu_style
     |
     +-- locales
         |
         +-- en
	 |   |
	 |   +-- example1.po
	 |   |
	 |   +-- example2.po
	 |   |
	 |   +-- subsubdir
	 |       |
	 |       +-- example3.po
	 |       |
	 |       +-- example4.po
	 |
         +-- zu
	     |
	     +-- example1.po
	     |
	     +-- example2.po
	     |   
	     +-- subsubdir
	         |
	         +-- example3.po
	         |
	         +-- example4.po


Pootle layout::

  -- $project
     |
     +-- en
     |   |
     |   +-- subdir3
     |       |
     |       +- example1.po
     |       |
     |       +- example2.po   
     |       |
     |       +-- subsubdir
     |           |
     |           +-- example3.po
     |           |
     |           +-- example4.po
     |   
     +-- zu
         |
         +-- subdir3
             |
             +- example1.po
             |
             +- example2.po   
             |
             +-- subsubdir
                 |
                 +-- example3.po
                 |
                 +-- example4.po

++++
