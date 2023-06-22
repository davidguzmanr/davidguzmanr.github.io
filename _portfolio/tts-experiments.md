---
title: "Speech Generation for Indigenous Language Education & the EveryVoice TTS Toolkit"
excerpt: "TTS experiments with different settings"
collection: portfolio
---
<br>

# FastSpeech2 + HiFi-GAN base

<table>
  <tbody>
    <tr>
      <th style="text-align: center">5741.wav (Ground-Truth) </th>
      <th style="text-align: center">5741.wav (Synthesized) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/ground-truth/5741.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/HiFiGAN/base/5741.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  Pero la vergüenza no me impidió tomar una resolución.
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">6941.wav (Ground-Truth) </th>
      <th style="text-align: center">6941.wav (Synthesized) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/ground-truth/6941.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/HiFiGAN/base/6941.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  Se proponía presentarse a Don Carlos y retarle a desafío para decidir en juicio de Dios, peleando con toda lealtad, la grave cuestión que motivaba la guerra.
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">9603.wav (Ground-Truth) </th>
      <th style="text-align: center">9603.wav (Synthesized) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/ground-truth/9603.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/HiFiGAN/base/9603.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  Era un día de Marzo de esos que parecen días de Junio, privilegio de la corte de las Españas, que suele abrasarse en Febrero y helarse en Mayo.
  </em>
</div>
<br>

# FastSpeech2 + HiFi-GAN finetuned

<table>
  <tbody>
    <tr>
      <th style="text-align: center">5741.wav (Ground-Truth) </th>
      <th style="text-align: center">5741.wav (Synthesized) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/ground-truth/5741.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/HiFiGAN/finetuned/5741.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  Pero la vergüenza no me impidió tomar una resolución.
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">6941.wav (Ground-Truth) </th>
      <th style="text-align: center">6941.wav (Synthesized) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/ground-truth/6941.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/HiFiGAN/finetuned/6941.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  Se proponía presentarse a Don Carlos y retarle a desafío para decidir en juicio de Dios, peleando con toda lealtad, la grave cuestión que motivaba la guerra.
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">9603.wav (Ground-Truth) </th>
      <th style="text-align: center">9603.wav (Synthesized) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/ground-truth/9603.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/HiFiGAN/finetuned/9603.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  Era un día de Marzo de esos que parecen días de Junio, privilegio de la corte de las Españas, que suele abrasarse en Febrero y helarse en Mayo.
  </em>
</div>
<br>

# Acknowledgement
The synthetic speech samples were constructed using a [Spanish speaker dataset](https://discourse.mozilla.org/t/sharing-my-100h-of-single-speaker-spanish/45288) with the LJSpeech format collected and validated by [Carlos Fonseca](https://github.com/carlfm01).
