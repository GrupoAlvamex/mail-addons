# mail-addons
Odoo (OpenERP) mail addons

List of repositories:
---------------------

* https://github.com/it-projects-llc/misc-addons
* https://github.com/it-projects-llc/pos-addons
* https://github.com/it-projects-llc/mail-addons
* https://github.com/it-projects-llc/rental-addons
* https://github.com/it-projects-llc/access-addons
* https://github.com/it-projects-llc/website-addons
* https://github.com/it-projects-llc/l10n-addons
* https://github.com/it-projects-llc/odoo-telegram
* https://github.com/it-projects-llc/odoo-saas-tools

Donation
========
Feel free to support our efforts by purchasing [our mail modules at app store](https://apps.odoo.com/apps/modules/category/Discuss/browse?price=Paid&order=Newest&author=IT-Projects+LLC)





Debrand Email Template
========

-- note that you should find and replace the 'new color' (#505fb5) prior to running.

Colors
=======
UPDATE mail_template set body_html = replace(replace(body_html, '#875A7B', '#505fb5'), 'rgb(135,90,123)', '#505fb5');

Footers
======
UPDATE mail_template set body_html = replace(body_html, '<tr><td align="center">Powered by <a href="https://www.odoo.com">Odoo</a>.</td></tr>', '');
                      
                      
UPDATE mail_template set body_html =
  replace(body_html, ' using <a href="www.odoo.com" style=" color: #505fb5;"><strong>Odoo</strong></a>', '');
UPDATE mail_template set body_html =
  replace(body_html, ' using <a href="www.odoo.com" style="text-decoration:none; color: #505fb5;"><strong>Odoo</strong></a>', '');
UPDATE mail_template set body_html =
  replace(body_html, '    using
    <a href="https://www.odoo.com" style="text-decoration:none; color: #505fb5;">Odoo</a>', '');
UPDATE mail_template set body_html =
  replace(body_html, '                <p>---<br />
                    Odoo - Open Source Business Applications<br />
                    http://www.odoo.com<br />
                </p>', '');
UPDATE mail_template set body_html =
  replace(body_html, '    <p style="font-size: 11px; margin-top: 10px;">
        <strong>Sent by ${user.company_id.name} using <a href="www.odoo.com" style="text-decoration:none; color: #505fb5;">Odoo</a></strong>
    </p>', '');
