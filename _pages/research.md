---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
display_categories: [Current Projects, Past Projects]
horizontal: false
header:
  og_image: 
---

I earned my PhD in physiological signal processing and machine learning from the [Université Grenoble Alpes](https://www.univ-grenoble-alpes.fr/){: target="_blank"} in France, where I conducted my research at the [Gipsa-Lab](https://www.gipsa-lab.grenoble-inp.fr/){: target="_blank"}. My doctoral work focused on total laryngectomy surgery, which involves the removal of the larynx following advanced throat cancer, with the goal of enabling the feasibility of an implantable active artificial larynx prosthesis. This led to the development of a laboratory prototype that demonstrated the feasibility of a real-time detection of swallowing using specific neck measurements, followed by the activation of an airway protective mechanism.

Currently, I am working as a postdoctoral researcher at the [University of Tokyo](https://www.u-tokyo.ac.jp/en/){: target="_blank"}, within in the [Saito Laboratory](https://www.ytksailab.org){: target="_blank"}, on biological experiment automation and protein engineering. Specifically, I use artificial intelligence methods to automate a robot designed to conduct experiments on protein engineering. Additionally, my work on protein engineering methods aimed at developing new and improved proteins for medical applications.

<nbsp>

{% include base_path %}

{% for category in page.display_categories %}
	<h2 class="category">{{ category }}</h2>
	{% assign categorized_projects = site.research | where: "category", category %}
	{% assign sorted_projects = categorized_projects | sort:"order_number" %}
	<!--<div style="padding-top: 20px; padding-right: 20px; padding-bottom: 20px; padding-left: 20px">-->
	<div style="padding-bottom: 205px">
	{% for post in sorted_projects %}
		{% include archive-single.html type="grid" %}
	{% endfor %}
	</div>
{% endfor %}

<!--{% include base_path %}-->
<!--{% assign ordered_pages = site.research | sort:"order_number" %}-->
<!--{% for post in ordered_pages %}-->
<!--  {% include archive-single.html type="grid" %}-->
<!--{% endfor %}-->

