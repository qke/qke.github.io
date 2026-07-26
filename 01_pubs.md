---
layout: page
title: Publications
permalink: /pubs/
---

<script type="text/javascript">
function toggle_visibility(id) {
    var e = document.getElementById(id);
    e.style.display = (e.style.display == 'block') ? 'none' : 'block';
}
</script>

<style>
.pub-content {
  display: flex;
  align-items: flex-start;
}

.pub-text {
  flex: 1;
  margin-right: 15px;
}

.pub-image img {
  width: 300px;
  border-radius: 6px;
}

.pub-item {
  margin-bottom: 20px;
}

.title {
  font-weight: bold;
}

@media (max-width: 700px) {
  .pub-content {
    flex-direction: column;
  }

  .pub-image img {
    width: 100%;
    max-width: 300px;
    margin-top: 10px;
  }
}
</style>


* [Google Scholar](https://scholar.google.com/citations?user=CSKDXt4AAAAJ&hl=en)
* [ORCID ID](https://orcid.org/0000-0002-2945-5274)
* [Scopus Author ID](https://www.scopus.com/authid/detail.uri?authorId=56366264000)

### Preprints

* [COMO: Closed-Loop Optical Molecule Recognition with Minimum Risk Training](https://arxiv.org/abs/2604.23546)<br>
Zhuoqi Lyu, **Q Ke**<br>
(2026)<br>
[arXiv](https://arxiv.org/abs/2604.23546)  |
[models & data](https://huggingface.co/Keylab/COMO) | 
[como-ocsr package](https://pypi.org/project/como-ocsr/) | 
[Github](https://github.com/netknowledge/COMO)

* [Not too long do read: Evaluating LLM-generated extreme scientific summaries](https://arxiv.org/abs/2512.23206)<br>
Zhuoqi Lyu, **Q Ke**<br>
[arXiv:2512.23206](https://arxiv.org/abs/2512.23206) (2025)

* [Periodical embeddings uncover hidden interdisciplinary patterns in the subject classification scheme of science](https://arxiv.org/abs/2512.22524)<br>
Zhuoqi Lyu, **Q Ke**<br>
[arXiv:2512.22524](https://arxiv.org/abs/2512.22524) (2025)

* [MorganBERT: Chemical substructure sequences meet language models for property prediction](https://doi.org/10.26434/chemrxiv-2025-67w3z)<br>
**Q Ke**, Junjie Dong<br>
ChemRxiv (2025)

* [Temporal search in the scientific space predicts breakthrough inventions](https://arxiv.org/abs/2107.09176)<br>
C Min, <b>Q Ke</b><br>
[arXiv:2107.09176](https://arxiv.org/abs/2107.09176) (2021)


### Published


{% for year_block in site.data.publications %}
  <h4>{{ year_block.year }}</h4>

  <ul class="pub-list">
    {% for paper in year_block.papers %}
      <li class="pub-item">
        <div class="pub-content">
          <div class="pub-text">
            <div class="title"><a href="{{ paper.doi }}">{{ paper.title }}</a></div>
            <div class="authors">{{ paper.authors }}</div>
            <div class="venue"><em>{{ paper.venue }}</em> <strong>{{ paper.volume }}</strong>, {{ paper.pages }}</div>
            {% if paper.links %}
              <div class="links">
                {% if paper.links.arxiv %}
                  <a href="{{ paper.links.arxiv }}">arXiv</a>
                {% endif %}
                {% if paper.links.data %}
                  <a href="{{ paper.links.data }}">Data</a>
                {% endif %}
                {% if paper.links.code %}
                  <a href="{{ paper.links.code }}">Code</a>
                {% endif %}
                {% if paper.links.project %}
                  <a href="{{ paper.links.project }}">Project</a>
                {% endif %}
                {% if paper.links.cover %}
                  <a href="{{ paper.links.cover }}">Cover</a>
                {% endif %}
                {% if paper.links.video %}
                  <a href="{{ paper.links.video }}">Video</a>
                {% endif %}
                {% if paper.links.interactive %}
                  <a href="{{ paper.links.interactive }}">Interactive</a>
                {% endif %}
                {% if paper.links.webby %}
                  <a href="{{ paper.links.webby }}"><font color="red">2020 Webby Awards for NetArt</font></a>
                {% endif %}
                {% if paper.links.honorable_mention %}
                  <a href="{{ paper.links.honorable_mention }}"><font color="red">Best Paper Honorable Mentions</font></a>
                {% endif %}
                {% if paper.links.nature_news %}
                  <a href="{{ paper.links.nature_news }}">Nature News</a>
                {% endif %}
                {% if paper.links.lse %}
                  <a href="{{ paper.links.lse }}">LSE Impact Blog</a>
                {% endif %}
              </div>
            {% endif %}
          </div>
          {% if paper.image %}
            <div class="pub-image">
              <img src="{{ paper.image }}">
            </div>
          {% endif %}
        </div>
      </li>
    {% endfor %}
  </ul>
{% endfor %}


### Others

* [Scientific birds of a feather flock together: science communication on social media rarely happens across or beyond disciplinary boundaries](https://blogs.lse.ac.uk/impactofsocialsciences/2017/07/12/scientific-birds-of-a-feather-flock-together-science-communication-on-social-media-rarely-happens-across-or-beyond-disciplinary-boundaries/)<br>
<b>Q Ke</b>, YY Ahn, CR Sugimoto<br>
<em>Impact of Social Sciences Blog</em> (2017)

* [Social media metrics as indicators of broader impact](https://web-archive.oecd.org/2016-10-20/418029-172%20-%20SugimotoOECDaltmetrics.pdf)<br>
CR Sugimoto, S Haustein, <b>Q Ke</b>, V Larivière<br>
<em>OECD Blue Sky III Forum on Science and Innovation Indicators</em> (2016)
