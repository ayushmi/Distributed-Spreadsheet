CS632A Distributed Systems
===========================
Project: Distributed Spreadsheet
=================================

1. Problem Statement:

Google Spreadsheets allows multiple users to edit a spreadsheet in collaborative manner. However, the sharing is either in granularity of column or row. Basically when a column or row is selected, a lock on the rewsource is acquired by a peer. Only after peer releases the column other peers can acquire lock. The idea of this project is to let peers draw and select multiple number of arbitrary boxes on a table and edit it. Note that the selection will automatically acquire locks also on certain other cells which contain functions on the locked cells. However, these auto locks do not allow the original peer to modify functions. While editing is on every body can see modified values. Furthermore, if cells having formula being modified then there could be multiple dependencies which should be properly handled to make the full collaborative editing possible. 


