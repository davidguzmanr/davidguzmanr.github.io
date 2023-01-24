---
title: "EXIST-2021: sEXism Identification in Social neTworks"
excerpt: "Project for my *Text Mining* course. 
<br/><img src='/images/exist-2021.gif' style='width:500px;height:200px;' class='center'>"
collection: portfolio
---
Detecting online sexism may be difficult, as it may be expressed in very different forms. The aim of this competition and 
project is the detection of sexism in a broad sense, from explicit misogyny to other subtle expressions that involve implicit 
sexist behaviours. The automatic identification of sexisms in a broad sense may help to create, design and determine the evolution 
of new equality policies, as well as encourage better behaviors in society.

I applied fine-tuning to [bert-base-multilingual-uncased](https://huggingface.co/bert-base-multilingual-uncased) to make the classification.
I chose this model because the task contained text in English and Spanish. In the table below you can see the performance of my model, which is quite close to the winner of the shared task (see [EXIST-2021 results](http://nlp.uned.es/exist2021/#results)).

<style type="text/css">
.tg  {border:none;border-collapse:collapse;border-color:#ccc;border-spacing:0;margin:0px auto;}
.tg td{background-color:#fff;border-color:#ccc;border-style:solid;border-width:0px;color:#333;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#f0f0f0;border-color:#ccc;border-style:solid;border-width:0px;color:#333;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-mxj2{background-color:#f9f9f9;border-color:inherit;font-style:italic;text-align:center;vertical-align:top}
.tg .tg-yynm{background-color:#f0f0f0;border-color:#000000;color:#333333;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-abip{background-color:#f9f9f9;border-color:inherit;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-yynm" rowspan="2">Model</th>
    <th class="tg-7btt" colspan="2">Task 1: Sexism Identification</th>
    <th class="tg-7btt" colspan="2">Task 2: Sexism Categorization</th>
  </tr>
  <tr>
    <th class="tg-mxj2">Accuracy</th>
    <th class="tg-mxj2">F1</th>
    <th class="tg-mxj2">Accuracy</th>
    <th class="tg-mxj2">F1</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow">AI-UPV (winner)</td>
    <td class="tg-c3ow">0.7804</td>
    <td class="tg-c3ow">0.7802</td>
    <td class="tg-c3ow">0.6577</td>
    <td class="tg-c3ow">0.5787</td>
  </tr>
  <tr>
    <td class="tg-abip">My model</td>
    <td class="tg-abip">0.7537</td>
    <td class="tg-abip">0.7519</td>
    <td class="tg-abip">0.6165</td>
    <td class="tg-abip">0.5308</td>
  </tr>
</tbody>
</table>
<br><br>

The code with more explanations is in my GitHub [EXIST2021](https://github.com/davidguzmanr/EXIST2021).

<img src='/images/exist-2021.gif' class='center'>