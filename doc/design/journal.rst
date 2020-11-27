.. _model-account.journal:

Journal
=======

A *Journal* represents a book of original entry from traditional manual
accounting.
In Tryton it allows `Account Moves <model-account.move>` of the same class
to be grouped together.
Every account move gets associated with a journal, and the journal defines
what sequence is then used to number the account move.

Among the journal's properties is a type.
This limits where the journal can be used.

.. seealso::

   The journals can be found by opening the main menu item:

      |Financial --> Configuration --> Journals --> Journals|__

      .. |Financial --> Configuration --> Journals --> Journals| replace:: :menuselection:`Financial --> Configuration --> Journals --> Journals`
      __ https://demo.tryton.org/model/account.journal

Reports
-------

.. _report-account.move.general_journal:

General Journal
^^^^^^^^^^^^^^^

In Tryton the general journal lists all of the
`Account Moves <model-account.move>` that happened between the selected start
and end dates.
It also includes details such as the accounts, debits and credits involved.

.. seealso::

   The general journal can be printed by using the main menu item:

      :menuselection:`Financial --> Reporting --> Print General Journal`

Wizards
-------

.. _wizard-account.move.open_journal:

Open Journal
^^^^^^^^^^^^

The *Open Journal* wizard allows you to get a list of the journal entries for
a specific `Period <model-account.period>`.

.. seealso::

   The wizard can be started by using the main menu item:

      :menuselection:`Financial --> Entries --> Open Journal`

.. _model-account.journal.period:

Journal Period
==============

For each `Company <company:model-company.company>`, a *Journal Period* links
together the concepts of a `Journal <model-account.journal>`, and an accounting
`Period <model-account.period>`.
It provides a way of partially closing a period one journal at a time.

.. seealso::

   The company's journal periods can be listed by opening the main menu item:

      |Financial --> Reporting --> Journals - Periods|__

      .. |Financial --> Reporting --> Journals - Periods| replace:: :menuselection:`Financial --> Reporting --> Journals - Periods`
      __ https://demo.tryton.org/model/account.journal.period

   The company's open journal periods can be found using the main menu item:

      :menuselection:`Financial --> Entries --> Journals - Periods`
