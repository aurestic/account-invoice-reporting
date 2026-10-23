This module prints the bank account details (bank, BIC/SWIFT and IBAN) of the
invoice's recipient bank account on the invoice report.

Up to Odoo 17 it also selected the company bank account matching the invoice
currency; since Odoo 18 the core already prefers the bank account in the
invoice currency (see `account.move._compute_partner_bank_id`), so that part
was dropped in the 19.0 migration.
