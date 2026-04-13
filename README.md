

## ➡️ Available options

<!--options-->
<table>
  <tr>
    <td align="center" nowrap="nowrap">Option</i></td><td align="center" nowrap="nowrap">Description</td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_topics</code></h4></td>
    <td rowspan="2"><p>Enable topics plugin</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap">🌐 Web instances must configure <code>settings.json</code>:
<ul>
<li><i>metrics.run.puppeteer.scrapping</i></li>
</ul>
<b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_topics_mode</code></h4></td>
    <td rowspan="2"><p>Display mode</p>
<ul>
<li><code>labels</code>: display labels</li>
<li><code>icons</code>: display icons <em>(topics without icons will not be displayed)</em></li>
<li><code>starred</code>: alias for <code>labels</code></li>
<li><code>mastered</code>: alias for <code>icons</code></li>
</ul>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>string</code>
<br>
<b>default:</b> starred<br>
<b>allowed values:</b><ul><li>labels</li><li>icons</li><li>starred</li><li>mastered</li></ul></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_topics_sort</code></h4></td>
    <td rowspan="2"><p>Sorting method</p>
<ul>
<li><code>stars</code>: sort by most stars</li>
<li><code>activity</code>: sort by recent activity</li>
<li><code>starred</code>: sort by starred date</li>
<li><code>random</code>: sort randomly</li>
</ul>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>string</code>
<br>
<b>default:</b> stars<br>
<b>allowed values:</b><ul><li>stars</li><li>activity</li><li>starred</li><li>random</li></ul></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_topics_limit</code></h4></td>
    <td rowspan="2"><p>Display limit</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥
≤ 20)</i>
<br>
<b>zero behaviour:</b> disable</br>
<b>default:</b> 15<br></td>
  </tr>
</table>
<!--/options-->

## ℹ️ Examples workflows

<!--examples-->
```yaml
name: Labels
uses: lowlighter/metrics@latest
with:
  filename: metrics.plugin.topics.svg
  token: NOT_NEEDED
  base: ""
  plugin_topics: yes
  plugin_topics_limit: 12

```
```yaml
name: Icons
uses: lowlighter/metrics@latest
with:
  filename: metrics.plugin.topics.icons.svg
  token: NOT_NEEDED
  base: ""
  plugin_topics: yes
  plugin_topics_limit: 0
  plugin_topics_mode: icons

```
<!--/examples-->
