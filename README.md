Satellite HTML report
=====================

INFORMATION
-----------

This is report template for satellite 6.5 host inventory...
It's base on https://www.redhat.com/en/blog/getting-started-satellite-65-reporting-engine

Requirements
------------

Redhat Satellite 6.5+ / Foreman 1.20+


How to use the template
------------------------

To use it:

1/ git clone git clone https://github.com/kamedodji/satellite-html-report.git

2/ hammer report-template  create --name "Satellite HTML Report Inventory" --file satellite-html-report/export.erb --default yes --organization-id 1

3/ You can check now that report template have been correctly imported:

    # hammer report-template list

4/ If previous is OK, generate your report:

    # hammer report-template generate --name "Satellite HTML Report Inventory" | tee /tmp/satellite-html-report.html

    # hammer report-template list

    # hammer report-template list

