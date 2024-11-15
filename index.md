---
layout: page
title: Frugal AI Challenge
menu_title: Home
menu_icon: house-door
---

{:.secondary}
# {{ site.event_date }}, co-located with the 2025 AI Action Summit

<!-- REMOVE THIS SECTION when you use this template -->
<div class="lead" markdown="1">
Welcome to the homepage for the Frugal AI Challenge, co-located with the [2025 AI Action Summit](https://www.elysee.fr/en/sommet-pour-l-action-sur-l-ia), taking place on February 10 and 11th in Paris, France.
Sign up [here](https://docs.google.com/forms/d/e/1FAIpQLSdwrq9Rhe7fcFL2_UQrIP3bPb75-zKF7aHq2h--lF0iSoITIA/viewform?usp=sf_link) to receive updates and news about the Challenge.
</div>
<!-- END of section to remove -->

<div class="aside">
    <h2><i class="bi bi-calendar3"></i> Event timeline</h2>
    <dl>
        {% if site.registration_status == "soon" or site.registration_status == "open" or site.registration_status == "demo" %}
            <dt>{{ site.registration_opens_date }}</dt>
            <dd>
                Applications open for participants<br>
                {% if site.registration_status == 'open' %}
                    <a href="{{ site.baseurl }}{% link registration.md %}" class="btn">Register now</a>
                {% elsif site.registration_status == 'closed' %}
                    <a class="btn disabled">Registration has closed</a>
                {% elsif site.registration_status == 'soon' %}
                    <a class="btn disabled">Registration opens in January</a>
                {% endif %}
            </dd>
        {% endif %}

        <dt>{{ site.registration_closes_date }}</dt>
        <dd>Applications close</dd>

        <dt>{{ site.event_date }}</dt>
        <dd>Hackathon date</dd>
    </dl>
</div>

The goal of the **Frugal AI Challenge** is to encourage both academic and industry actors to keep **efficiency** in mind when deploying AI models. 

By tracking both energy consumption and performance for different AI for climate tasks, we can incentivize **frugality** in AI deployment, as well as addressing real-world challenges.

## Tasks 🥇

We have chosen three tasks across three modalities, all of which are useful in the global fight against the climate crisis:

1. **📝 Detecting climate disinformation 📝:** based on text from news articles.
2. **🔥 Classifying regions at risk of wildfires 🔥:** based on image data gathered via satellite.
3. **🌳🪓 Detecting illegal deforestation 🌳🪓 :** from bio-acoustic data recorded in the jungle

*We will announce more details about the tasks and release the datasets soon!*

##  Evaluation 🏆

---

We will track both **performance** and **efficiency** on each of the datasets:

- **Performance** will be measured based on metrics that reflect the real-world constraints of each task
- **Efficiency** will be measured using [Code Carbon](https://github.com/mlco2/codecarbon), a tool for measuring energy consumption and carbon emissions of code.
  
