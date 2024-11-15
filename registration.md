---
title: Challenge registration
menu_title: Registration
menu_icon: clipboard-check
event_status:
 - soon
---

{:.lead}
Participation is open to researchers or practitioners from any institution,
and we encourage contributions from early career
researchers. {% if site.registration_status
== "soon" or site.registration_status == "demo" %}Registration opens on
{{ site.registration_opens_date }}.{% endif %} The closing date for applications
is {{ site.registration_closes_date }}.

<div class="aside" markdown="1">

{% if site.registration_status == "soon" or site.registration_status == "demo" %}
  <a class="btn disabled">Registration opens soon</a>
{% endif %}
{% if site.registration_status == "open" or site.registration_status == "demo" %}
  [Complete the application form](https://forms.office.com/...){:.btn target="_blank"}
{% endif %}
{% if site.registration_status == "closed" or site.registration_status == "demo" %}
  <a class="btn disabled">Registration has closed</a>
{% endif %}

The closing date for applications is {{ site.registration_closes_date }} and 
winners will be announced at the in-person event in {{ site.event_date }}.
</div>

The datasets for each task will be shared in early December, and we will provide 
example evaluation Jupyter notebooks, as well as technical support and guidance.

The closing date for the applications is {{ site.registration_closes_date }}. If
you have any queries, or have any difficulties completing the registration form,
please email our dedicated mailbox: <{{ site.mailbox_address }}>.

[faq]: {{ site.baseurl }}{% link faq.md %}
