
Make ir_mail_server silent and improve odoo server performance
========================================================================================================================
It's frustrating just how slow the sending email process in Odoo Server can be when you have many emails to send.
The whole interface freezes and the user can't do anything else just to wait, sometimes, for more than 30 seconds
for the interface to get back. So I made a lame hack for odoo mail server.

Module that adds customizations to the ir_mail_server module.
It sends the send_email job in background, making it independent from the web interface.
