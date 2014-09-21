.. _Enabling and Configuring Cohorts:

##########################################
Enabling and Configuring Cohorts
##########################################

To support private discussions for cohorts, you select a strategy for assigning
your students to cohort groups: automated assignment, manual assignment, or a
hybrid approach. See :ref:`Options for Assigning Students to Cohorts`. You also
decide whether to open any of the course-wide discussion topics to
participation by all students. See :ref:`TBD`.

After you select a strategy, you complete these steps (as applicable):

#. :ref:`Enable the cohort feature<Enable Cohorts>`.

#. :ref:`Enable automated cohort assignment<Enable Automated Cohort Assignment>`` and :ref:`define auto cohort groups<Define Auto Cohort Groups>`, or 
   Define manual cohort groups and assign students to them, or
   Do both. 

#. Identify the course-wide discussion topics that you want to support private,
   cohort-only participation. Optional.

#. Assign students to manual cohort groups. Applies to manual and hybrid
   assignement strategies only.

To complete these steps you use Studio and the Instructor Dashboard for your
live course.

.. _Enable Cohorts:

********************************
Enabling the Cohort Feature
********************************

#. Open the course in Studio. 

#. Select **Settings**, then **Advanced Settings**.

#. In the **Cohort Configuration** field, place your cursor between the
   supplied pair of braces.

#. Press Enter, type ``"cohorted":true``, and then press Enter again. 

 .. image:: ../Images/Enable_cohorts.png
  :alt: Cohort Configuration dictionary field with the cohorted key defined 
        as true

#. Click **Save Changes**.

***************************************************
Implementing the Automated Assignment Strategy
***************************************************

.. _Enable Automated Cohort Assignment:

============================================
Enable Automated Cohort Assignment
============================================

You complete this step if you selected either the automated or hybrid
assignment strategy for your course.

#. Open the course in Studio. 

#. Select **Settings**, then **Advanced Settings**.

#. In the **Cohort Configuration** field, place your cursor after
   ``"cohorted":true``.

#. Type a comma ``,`` character and then press Enter.

#. Type ``"auto_cohort":true`` and then press Enter again. 

 .. image:: ../Images/Enable_auto_cohorts.png
  :alt: Cohort Configuration dictionary field with the auto_cohort key defined 
        as true

#. Click **Save Changes**.

You continue by defining the auto cohort groups. 

.. _Define Auto Cohort Groups:

============================================
Define Auto Cohort Groups
============================================

You complete this step if you selected either the automated or hybrid
assignment strategy for your course.

.. note:: Students can see the name of the cohort group they are assigned to. 
 The message "This post is visible only to Group *cohort name*" appears with
 each post in discussion topics that support private, cohort-only
 participation.

#. Open the course in Studio. 

#. Select **Settings**, then **Advanced Settings**.

#. In the **Cohort Configuration** field, place your cursor after
   ``"auto_cohort":true``.

#. Type a comma ``,`` character and then press Enter.

#. For the automated assignment strategy, you define a set of groups. Place
   each group name within quotation marks, separate the names with commas, and
   place each one on a new line:
   
   ``"auto_cohort_groups":[
       "example_1st_group_name",
       "example_2nd_group_name",
       "example_3rd_group_name"
     ]`` 
   
   Then, press the Enter key again.

  .. image:: ../Images/Multi_auto_cohort_group.png
   :alt: Cohort Configuration dictionary field with the auto_cohort_groups key 
        with three values

#. For the hybrid strategy, you enter a single group name. Type
   ``"auto_cohort_groups":["example_group_name"]`` and then press Enter again.
   
 .. image:: ../Images/Single_auto_cohort_group.png
  :alt: Cohort Configuration dictionary field with the auto_cohort_groups key 
        with one value

#. Click **Save Changes**.


.. _:

***************************************************
Implementing the Manual Assignment Strategy
***************************************************

==========================================
Define Manual Cohort Groups
==========================================




==========================================
Assign Students to Cohort Groups Manually
==========================================





All cohort configs:

=====================================
Define Open Course-Wide Discussion Topics
=====================================

All courses include a page named **Discussion**. When you create a course, a
discussion topic named "General" is available for you to include by default.
You can add more course-wide discussion topics to guide how students share and
find information during your course. Such course-wide topics might include
Feedback, Troubleshooting, or Technical Help. Discussions in these topics can
begin as soon as your course is available.

All content-specific discussion topics, which you add to your course outline in discussion components, are cohorted.

:ref:`Create CourseWide Discussion Topics`



1. Studio Turn it on (cohorted)
2. Studio (optional) define some general discussion topics (cohorted_discussions): Announcements, FAQ, Errata, Troubleshooting. So that you only have to post once to them to reach all students.

To set up auto: 

3. Studio turn it on (auto_cohort)
4. Studio define the cohort groups (auto_cohort_groups)
   
To set up manual-only cohorting:

3. LMS define cohort groups
4. LMS assign students to cohort groups

assignment occurs when each student visits the discussion page

To set up hybrid:

