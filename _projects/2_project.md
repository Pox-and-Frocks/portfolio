---
layout: page
title: The Lorenz Differential Equations
description: an example of a project component that uses a jupyter notebook
img: assets/img/jupyter.png
importance: 2
category: planning
giscus_comments: true
---

You can embed a jupyter notebook on a page like this. You can put any description here, and use the example below to include your notebook (just replace the file path).

{::nomarkdown}
{% assign jupyter_path = 'assets/jupyter/Lorenz.ipynb' | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/Lorenz.ipynb %}{% endcapture %}
{% if notebook_exists == 'true' %}
{% jupyter_notebook jupyter_path %}
{% else %}

  <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
