---
layout: page
title: Frugal AI Challenge
menu_title: Home
menu_icon: house-door
---

{:.secondary}
# {{ site.event_date }}, virtual and in-person

<!-- REMOVE THIS SECTION when you use this template -->
<div class="lead" markdown="1">
Welcome to the homepage for the Frugal AI Challenge, co-located with the [2025 AI Action Summit](https://www.elysee.fr/en/sommet-pour-l-action-sur-l-ia), taking place on February 10-11 in Paris, France.

Sign up [here](https://framaforms.org/2025-frugal-ai-summit-1732038008) to receive updates and news about the Challenge.
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

By tracking both energy consumption and performance for different AI for climate tasks, we can incentivize **frugality** in AI deployment while also addressing real-world challenges.

We have chosen three tasks across three modalities, all of which are useful in the global fight against the climate crisis: detecting climate disinformation, classifying regions at risk of wildfires, and detecting illegal deforestation. We will evaluate both **performance** and **efficiency** on each of the datasets, based on the real-world constraints of each task and the energy used.

The datasets for each task are hosted on our [Hugging Face organization page](https://huggingface.co/collections/frugal-ai-challenge/frugal-ai-challenge-tasks-673dd5ee724c6659a5b42443) - you can download them and start training models! 
