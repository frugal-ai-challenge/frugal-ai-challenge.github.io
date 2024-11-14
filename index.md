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

{% if site.event_status != "over" %}

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
  
## Organizing Committee 💪

**Sasha Luccioni *(Hugging Face)*** Sasha is the Climate Lead at Hugging Face, a global startup in responsible open-source AI, where she spearheads research, consulting and capacity-building to elevate the sustainability of AI systems. She is a founding member of Climate Change AI (CCAI) and a board member of Women in Machine Learning (WiML).

**Theo Alves da Costa *(Data For Good)***  Théo specializes in Data Analytics and Artificial Intelligence (AI) applied to the social and ecological transition. He is the Head of "AI for Sustainability and Climate" unit at the French data-focused firm Ekimetrics and also serves as the co-president of the non-profit Data For Good.

**Juliette Fropier *(French Ministry of Ecological Transition)*** Juliette is part of Ecolab, the innovation lab of the French Ministry of Ecological Transition. Ecolab works for the valorization of public data and innovative answers to the double emergency of ecological transition and digital transformation. As such, Ecolab is responsible for the AI & ecological transition roadmap of the French government, in conjunction with all the ministries involved in the AI national strategy
 
**Yacine Jernite (*Hugging Face*)**  Yacine is the Machine Learning and Society Lead at Hugging Face, where he works on ML systems governance at the intersection of regulatory and technical tools. Most recently, he served as the co-organizer and data area chair for the [BigScience workshop](https://bigscience.huggingface.co/) on large language models.

## **Advisory Board** 🪄

Rumman Chowdhury (*Humane Intelligence*), Boris Gamazaychikov (Salesforce), Claire Monteleoni *(INRIA & University of Colorado Boulder),* David Rolnick (*McGill & Mila & Climate Change AI*), Gael Varoquaux (*INRIA*), Karteek Alahari (*INRIA*)
