---
title: "Speech Generation for Indigenous Language Education & the EveryVoice TTS Toolkit"
excerpt: "TTS experiments with different settings"
collection: portfolio
permalink: /portfolio/tts-experiments/
---

<br>

- [Vocoders](#vocoders)
  - [FastSpeech2 + HiFi-GAN base](#hifi-gan-base)
  - [FastSpeech2 + HiFi-GAN finetuned](#hifi-gan-finetuned)
  - [FastSpeech2 + BigVGAN base](#bigvgan-base)
  - [FastSpeech2 + BigVGAN finetuned](#bigvgan-finetuned)
- [Ensemble](#ensemble)
- [SeamlessM4T](#seamlessm4t)
  - [SeamlessM4T-large](#seamlessm4t-large)
  - [SeamlessM4T-large finetuned (eng-spa)](#seamlessm4t-large-finetuned-eng-spa)
  - [SeamlessM4T-large finetuned (moh)](#seamlessm4t-large-finetuned-moh)
- [Denoiser](#denoiser)
- [EveryVoice vocoder](#everyvoice-vocoder)

# Vocoders

## FastSpeech2 + HiFi-GAN base {#hifi-gan-base}

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

## FastSpeech2 + HiFi-GAN finetuned {#hifi-gan-finetuned}

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

## FastSpeech2 + BigVGAN base {#bigvgan-base}

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
          <source src="/files/audios/BigVGAN/base/5741.wav" autoplay="">
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
          <source src="/files/audios/BigVGAN/base/6941.wav" autoplay="">
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
          <source src="/files/audios/BigVGAN/base/9603.wav" autoplay="">
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

## FastSpeech2 + BigVGAN finetuned {#bigvgan-finetuned}

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
          <source src="/files/audios/BigVGAN/finetuned/5741.wav" autoplay="">
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
          <source src="/files/audios/BigVGAN/finetuned/6941.wav" autoplay="">
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
          <source src="/files/audios/BigVGAN/finetuned/9603.wav" autoplay="">
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

# Ensemble {#ensemble}

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;margin:0px auto;}
.tg td{border-bottom-width:1px;border-color:black;border-style:solid;border-top-width:1px;border-width:0px;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-bottom-width:1px;border-color:black;border-style:solid;border-top-width:1px;border-width:0px;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg" style="width:70%">
<thead>
  <tr>
    <th class="tg-amwm">Speaker ID</th>
    <th class="tg-amwm">ES</th>
    <th class="tg-amwm">EN</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-baqh">Training (unique utterances):</td>
    <td class="tg-baqh"></td>
    <td class="tg-baqh"></td>
  </tr>
  <tr>
    <td class="tg-baqh">Speaker-Dependent</td>
    <td class="tg-baqh">541</td>
    <td class="tg-baqh">13100</td>
  </tr>
  <tr>
    <td class="tg-baqh">Sampling 1st</td>
    <td class="tg-baqh">541</td>
    <td class="tg-baqh">4112</td>
  </tr>
  <tr>
    <td class="tg-baqh">Sampling 2nd</td>
    <td class="tg-baqh">541</td>
    <td class="tg-baqh">4174</td>
  </tr>
  <tr>
    <td class="tg-baqh">Sampling 3rd</td>
    <td class="tg-baqh">541</td>
    <td class="tg-baqh">4142</td>
  </tr>
  <tr>
    <td class="tg-baqh">Ensemble (Sampling 1+2+3)</td>
    <td class="tg-baqh">541</td>
    <td class="tg-baqh">8921</td>
  </tr>
  <tr>
    <td class="tg-baqh">Testing</td>
    <td class="tg-baqh">100</td>
    <td class="tg-baqh">100</td>
  </tr>
</tbody>
</table>
<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;margin:0px auto;}
.tg td{border-bottom-width:1px;border-color:black;border-style:solid;border-top-width:1px;border-width:0px;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-bottom-width:1px;border-color:black;border-style:solid;border-top-width:1px;border-width:0px;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-fpwh{background-color:#81FF81;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow"></th>
    <th class="tg-7btt" colspan="3">HiFi-GAN (universal)</th>
    <th class="tg-7btt" colspan="3">HiFi-GAN (finetuned)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow"></td>
    <td class="tg-7btt">English</td>
    <td class="tg-7btt">Spanish</td>
    <td class="tg-amwm">Sample</td>
    <td class="tg-7btt">English</td>
    <td class="tg-7btt">Spanish</td>
    <td class="tg-amwm">Sample</td>
  </tr>
  <tr>
    <td class="tg-7btt">SD-30-minutes<br>(speaker dependant)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.476</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-30-minutes.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.791</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-30-minutes.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">SD-5-hours<br>(speaker dependant)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.286</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-5-hours.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.631</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-5-hours.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">MU<br>(multi-speaker/language)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">8.467</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-test-en-es-low.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">8.625</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-test-en-es-low.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">OV<br>(oversampling)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.677</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-test-en-es-low-augmentation.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.946</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-test-en-es-low-augmentation.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">E1 (multi-speaker/language <br>with resampled corpora)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.698</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-test-ensemble-1.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">8.063</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-test-ensemble-1.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">E2 (multi-speaker/language <br>with resampled corpora)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.834</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-test-ensemble-2.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">8.093</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-test-ensemble-2.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">E3 (multi-speaker/language <br>with resampled corpora)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.745</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-test-ensemble-3.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">8.081</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-test-ensemble-3.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">EN<br>(ensemble model)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-fpwh">7.289</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-test-ensemble.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-fpwh">7.592</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-test-ensemble.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">EN<br>(ensemble model weighted)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.372</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9900-test-ensemble-weighted.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">7.695</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9900-test-ensemble-weighted.wav" autoplay=""></audio></td>
  </tr>
</tbody>
</table>
<div>
  <center>
  <em>
  Mel-ceptral distortion (smaller is better).
  </em>
  </center>
</div>
<br>

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;margin:0px auto;}
.tg td{border-bottom-width:1px;border-color:black;border-style:solid;border-top-width:1px;border-width:0px;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-bottom-width:1px;border-color:black;border-style:solid;border-top-width:1px;border-width:0px;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-fpwh{background-color:#81FF81;border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow"></th>
    <th class="tg-7btt" colspan="3">HiFi-GAN (universal)</th>
    <th class="tg-7btt" colspan="3">HiFi-GAN (finetuned)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow"></td>
    <td class="tg-7btt">English</td>
    <td class="tg-7btt">Spanish</td>
    <td class="tg-amwm">Sample</td>
    <td class="tg-7btt">English</td>
    <td class="tg-7btt">Spanish</td>
    <td class="tg-amwm">Sample</td>
  </tr>
  <tr>
    <td class="tg-7btt">SD-30-minutes<br>(speaker dependant)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.287</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-30-minutes.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.286</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-30-minutes.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">SD-5-hours<br>(speaker dependant)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.328</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-5-hours.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.336</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-5-hours.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">MU<br>(multi-speaker/language)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.316</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-test-en-es-low.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.308</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-test-en-es-low.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">OV<br>(oversampling)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.312</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-test-en-es-low-augmentation.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.320</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-test-en-es-low-augmentation.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">E1 (multi-speaker/language <br>with resampled corpora)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.306</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-test-ensemble-1.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.289</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-test-ensemble-1.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">E2 (multi-speaker/language <br>with resampled corpora)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.324</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-test-ensemble-2.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.312</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-test-ensemble-2.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">E3 (multi-speaker/language <br>with resampled corpora)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.308</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-test-ensemble-3.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.299</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-test-ensemble-3.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">EN<br>(ensemble model)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-fpwh">0.344</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-test-ensemble.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.303</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-test-ensemble.wav" autoplay=""></audio></td>
  </tr>
  <tr>
    <td class="tg-7btt">EN<br>(ensemble model weighted)</td>
    <td class="tg-c3ow">-</td>
    <td class="tg-c3ow">0.335</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan/9436-test-ensemble-weighted.wav" autoplay=""></audio></td>
    <td class="tg-c3ow">-</td>
    <td class="tg-fpwh">0.312</td>
    <td class="tg-baqh"><audio controls="controls"><source src="/files/audios/ensemble/hifigan-finetuned/9436-test-ensemble-weighted.wav" autoplay=""></audio></td>
  </tr>
</tbody>
</table>
<div>
  <center>
  <em>
  F0 correlation (bigger is better).
  </em>
  </center>
</div>
<br>

# SeamlessM4T

## SeamlessM4T-large {#seamlessm4t-large}

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/eng/0.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/spa/0.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/fra/0.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The quick brown fox jumps over the lazy dog.
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  El zorro marrón rápido salta sobre el perro perezoso.
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le renard brun rapide saute sur le chien paresseux.
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/eng/1.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/spa/1.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/fra/1.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The earliest book printed with movable types, the Gutenberg, or forty-two line Bible of about 1455
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  El primer libro impreso con tipos móviles, la Gutenberg, o Biblia de cuarenta y dos líneas de alrededor de 1455
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le premier livre imprimé avec des caractères mobiles, la Bible de Gutenberg, ou Bible de quarante-deux lignes, datant d'environ 1455
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/eng/2.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/spa/2.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/fra/2.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The Middle Ages brought calligraphy to perfection, and it was natural therefore
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  La Edad Media trajo la caligrafía a la perfección, y por lo tanto era natural
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le Moyen Âge a apporté la calligraphie à la perfection, et il était donc naturel
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/eng/3.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/spa/3.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large/fra/3.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The earliest book printed with movable type, the aforesaid Gutenberg Bible, is printed in letters which are an exact imitation
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  El primer libro impreso con tipos móviles, la mencionada Biblia de Gutenberg, está impreso en letras que son una imitación exacta
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le premier livre imprimé avec des caractères mobiles, la Bible de Gutenberg susmentionnée, est imprimé en lettres qui sont une imitation exacte
  </em>
</div>
<br>

## SeamlessM4T-large finetuned (eng-spa) {#seamlessm4t-large-finetuned-eng-spa}

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/eng/0.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/spa/0.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/fra/0.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The quick brown fox jumps over the lazy dog.
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  El zorro marrón rápido salta sobre el perro perezoso.
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le renard brun rapide saute sur le chien paresseux.
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/eng/1.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/spa/1.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/fra/1.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The earliest book printed with movable types, the Gutenberg, or forty-two line Bible of about 1455
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  El primer libro impreso con tipos móviles, la Gutenberg, o Biblia de cuarenta y dos líneas de alrededor de 1455
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le premier livre imprimé avec des caractères mobiles, la Bible de Gutenberg, ou Bible de quarante-deux lignes, datant d'environ 1455
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/eng/2.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/spa/2.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/fra/2.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The Middle Ages brought calligraphy to perfection, and it was natural therefore
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  La Edad Media trajo la caligrafía a la perfección, y por lo tanto era natural
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le Moyen Âge a apporté la calligraphie à la perfection, et il était donc naturel
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">English </th>
      <th style="text-align: center">Spanish </th>
      <th style="text-align: center">French </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/eng/3.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/spa/3.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_spa/fra/3.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text (eng):</b> 
  <em>
  The earliest book printed with movable type, the aforesaid Gutenberg Bible, is printed in letters which are an exact imitation
  </em> <br>
  <b>Text (spa):</b> 
  <em>
  El primer libro impreso con tipos móviles, la mencionada Biblia de Gutenberg, está impreso en letras que son una imitación exacta
  </em> <br>
  <b>Text (fra):</b> 
  <em>
  Le premier livre imprimé avec des caractères mobiles, la Bible de Gutenberg susmentionnée, est imprimé en lettres qui sont une imitation exacte
  </em>
</div>
<br>

## SeamlessM4T-large finetuned (moh) {#seamlessm4t-large-finetuned-moh}

<table>
  <tbody>
    <tr>
      <th style="text-align: center">501-650-kawe0612.wav (Ground-Truth) </th>
      <th style="text-align: center">501-650-kawe0612.wav (10 epochs) </th>
      <th style="text-align: center">501-650-kawe0612.wav (20 epochs) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/ground-truth/am-kanienkeha-ionkwahtharak-501-650-kawe0612.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/10-epochs/am-kanienkeha-ionkwahtharak-501-650-kawe0612.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/20-epochs/am-kanienkeha-ionkwahtharak-501-650-kawe0612.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  kèn:'en tsitskó:tak kanaktà:ke
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">651-1056-kawe0755.wav (Ground-Truth) </th>
      <th style="text-align: center">651-1056-kawe0755.wav (10 epochs) </th>
      <th style="text-align: center">651-1056-kawe0755.wav (20 epochs) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/ground-truth/am-kanienkeha-ionkwahtharak-651-1056-kawe0755.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/10-epochs/am-kanienkeha-ionkwahtharak-651-1056-kawe0755.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/20-epochs/am-kanienkeha-ionkwahtharak-651-1056-kawe0755.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  tó: nitiothó:re', ronhátien iowisóntion nè:'e ki' shà:ka tenkate'khahahkwà:na'
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">251-500-kawe0401.wav (Ground-Truth) </th>
      <th style="text-align: center">251-500-kawe0401.wav (10 epochs) </th>
      <th style="text-align: center">251-500-kawe0401.wav (20 epochs) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/ground-truth/am-kanienkeha-ionkwahtharak-251-500-kawe0401.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/10-epochs/am-kanienkeha-ionkwahtharak-251-500-kawe0401.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/20-epochs/am-kanienkeha-ionkwahtharak-251-500-kawe0401.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  kanatí:re's, ka' nòn:wa niahón:ne' thí: ratiksa'okòn:'a?
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">251-500-kawe0305.wav (Ground-Truth) </th>
      <th style="text-align: center">251-500-kawe0305.wav (10 epochs) </th>
      <th style="text-align: center">251-500-kawe0305.wav (20 epochs) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/ground-truth/am-kanienkeha-ionkwahtharak-251-500-kawe0305.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/10-epochs/am-kanienkeha-ionkwahtharak-251-500-kawe0305.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/20-epochs/am-kanienkeha-ionkwahtharak-251-500-kawe0305.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  ahsonhtà:ke ken kahrónnion?
  </em>
</div>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">651-1056-kawe0696.wav (Ground-Truth) </th>
      <th style="text-align: center">651-1056-kawe0696.wav (10 epochs) </th>
      <th style="text-align: center">651-1056-kawe0696.wav (20 epochs) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/ground-truth/am-kanienkeha-ionkwahtharak-651-1056-kawe0696.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/10-epochs/am-kanienkeha-ionkwahtharak-651-1056-kawe0696.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/SeamlessM4T/seamlessM4T_large_finetuned_moh/20-epochs/am-kanienkeha-ionkwahtharak-651-1056-kawe0696.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  á:keh tsi niiononhwákte' khsinà:ke
  </em>
</div>
<br>

# Denoiser {#seamlessm4t-large-finetuned-eng-spa}

|                        | **FastSpeech2** | **FastSpeech2 + denoiser** | **FastSpeech2 + postnet** | **FastSpeech2 + postnet + denoiser** |
| :--------------------: | :-------------: | :------------------------: | :-----------------------: | :----------------------------------: |
| Mel-ceptral distortion |     5.2347      |           5.2297           |          5.2307           |              **5.2294**              |
|     F0 correlation     |     0.1808      |           0.1985           |          0.1902           |              **0.2014**              |
|          PESQ          |     1.2898      |           1.2858           |          1.2851           |              **1.2972**              |

<table>
  <tbody>
    <tr>
      <th style="text-align: center">LJ001-0007.wav (FastSpeech2) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/denoiser/output/LJ001-0007.wav" autoplay="">
        </audio></td>
    </tr>
    <tr>
      <th style="text-align: center">LJ001-0007.wav (FastSpeech2 + denoiser) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/denoiser/denoised-output/LJ001-0007.wav" autoplay="">
        </audio></td>
    </tr>
    <tr>
      <th style="text-align: center">LJ001-0007.wav (FastSpeech2 + postnet) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/denoiser/postnet-output/LJ001-0007.wav" autoplay="">
        </audio></td>
    </tr>
    <tr>
      <th style="text-align: center">LJ001-0007.wav (FastSpeech2 + postnet + denoiser) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/denoiser/denoised-postnet-output/LJ001-0007.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<div>
  <b>Text:</b> 
  <em>
  the earliest book printed with movable types, the Gutenberg, or "forty-two line Bible" of about fourteen fifty-five
  </em>
</div>
<br>

# 40 and 80 Mel bands

<style type="text/css">
.tg  {border:none;border-collapse:collapse;border-color:#ccc;border-spacing:0;}
.tg td{background-color:#fff;border-color:#ccc;border-style:solid;border-width:0px;color:#333;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#f0f0f0;border-color:#ccc;border-style:solid;border-width:0px;color:#333;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-baqh{text-align:center;vertical-align:top}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
.tg .tg-amwm{font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow"></th>
    <th class="tg-c3ow"></th>
    <th class="tg-c3ow"><span style="font-weight:bold">FastSpeech2</span></th>
    <th class="tg-c3ow"><span style="font-weight:bold">FastSpeech2 + denoiser</span></th>
    <th class="tg-c3ow"><span style="font-weight:bold">FastSpeech2 + postnet</span></th>
    <th class="tg-c3ow"><span style="font-weight:bold">FastSpeech2 + postnet + denoiser</span></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7btt" rowspan="3">80-mel</td>
    <td class="tg-c3ow">Mel-ceptral distortion</td>
    <td class="tg-c3ow">7.3128</td>
    <td class="tg-c3ow">7.3531</td>
    <td class="tg-c3ow">7.3203</td>
    <td class="tg-c3ow">7.3594</td>
  </tr>
  <tr>
    <td class="tg-c3ow">F0 correlation</td>
    <td class="tg-c3ow">0.0360</td>
    <td class="tg-c3ow">0.0418</td>
    <td class="tg-c3ow">0.0370</td>
    <td class="tg-c3ow">0.0385</td>
  </tr>
  <tr>
    <td class="tg-c3ow">PESQ</td>
    <td class="tg-c3ow">1.3170</td>
    <td class="tg-c3ow">1.2809</td>
    <td class="tg-c3ow">1.2939</td>
    <td class="tg-c3ow">1.2858</td>
  </tr>
  <tr>
    <td class="tg-amwm" rowspan="3">40-mel</td>
    <td class="tg-baqh">Mel-ceptral distortion</td>
    <td class="tg-baqh">7.3444</td>
    <td class="tg-baqh">7.3391</td>
    <td class="tg-baqh">7.3535</td>
    <td class="tg-baqh">7.3462</td>
  </tr>
  <tr>
    <td class="tg-baqh">F0 correlation</td>
    <td class="tg-baqh">0.0392</td>
    <td class="tg-baqh">0.0320</td>
    <td class="tg-baqh">0.0381</td>
    <td class="tg-baqh">0.0307</td>
  </tr>
  <tr>
    <td class="tg-baqh">PESQ</td>
    <td class="tg-baqh">1.2604</td>
    <td class="tg-baqh">1.2254</td>
    <td class="tg-baqh">1.2436</td>
    <td class="tg-baqh">1.2295</td>
  </tr>
</tbody>
</table>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">LJ015-0199.wav (40 mel) </th>
      <th style="text-align: center">LJ015-0199.wav (80 mel) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/40-mel/LJ015-0199.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/00-mel/LJ015-0199.wav" autoplay="">
        </audio></td>
    </tr>
    <tr>
      <th style="text-align: center">LJ024-0078.wav (40 mel) </th>
      <th style="text-align: center">LJ024-0078.wav (80 mel) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/40-mel/LJ024-0078.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/40-mel/LJ024-0078.wav" autoplay="">
        </audio></td>
    </tr>
    <tr>
      <th style="text-align: center">LJ037-0160.wav (40 mel) </th>
      <th style="text-align: center">LJ037-0160.wav (80 mel) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/40-mel/LJ037-0160.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/40-mel/LJ037-0160.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>

# EveryVoice vocoder {#everyvoice-vocoder}

This model was only trained with English data (around 445 hours from LJSpeech, LibriTTS and VCTK). We also test in unseen speakers and languages.

## English

<table>
  <tbody>
    <tr>
      <th style="text-align: center">LJ022-0180.wav (Ground truth) </th>
      <th style="text-align: center">LJ022-0180.wav (Universal vocoder) </th>
      <th style="text-align: center">LJ022-0180.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/LJ022-0180-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/LJ022-0180-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/LJ022-0180-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">LJ030-0054.wav (Ground truth) </th>
      <th style="text-align: center">LJ030-0054.wav (Universal vocoder) </th>
      <th style="text-align: center">LJ030-0054.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/LJ030-0054-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/LJ030-0054-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/LJ030-0054-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">7314_77782_000009_000003.wav (Ground truth) </th>
      <th style="text-align: center">7314_77782_000009_000003.wav (Universal vocoder) </th>
      <th style="text-align: center">7314_77782_000009_000003.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/7314_77782_000009_000003-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/7314_77782_000009_000003-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/eng/7314_77782_000009_000003-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

## Spanish

<table>
  <tbody>
    <tr>
      <th style="text-align: center">549.wav (Ground truth) </th>
      <th style="text-align: center">549.wav (Universal vocoder) </th>
      <th style="text-align: center">549.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/549-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/549-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/549-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">774.wav (Ground truth) </th>
      <th style="text-align: center">774.wav (Universal vocoder) </th>
      <th style="text-align: center">774.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/774-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/774-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/774-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">822.wav (Ground truth) </th>
      <th style="text-align: center">822.wav (Universal vocoder) </th>
      <th style="text-align: center">822.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/822-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/822-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/spa/822-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

## French

<table>
  <tbody>
    <tr>
      <th style="text-align: center">F10_a1_s050_v01.wav (Ground truth) </th>
      <th style="text-align: center">F10_a1_s050_v01.wav (Universal vocoder) </th>
      <th style="text-align: center">F10_a1_s050_v01.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/F10_a1_s050_v01-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/F10_a1_s050_v01-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/F10_a1_s050_v01-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">M07_a3_s076_v01.wav (Ground truth) </th>
      <th style="text-align: center">M07_a3_s076_v01.wav (Universal vocoder) </th>
      <th style="text-align: center">M07_a3_s076_v01.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/M07_a3_s076_v01-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/M07_a3_s076_v01-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/M07_a3_s076_v01-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">M07_a3_s095_v01.wav (Ground truth) </th>
      <th style="text-align: center">M07_a3_s095_v01.wav (Universal vocoder) </th>
      <th style="text-align: center">M07_a3_s095_v01.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/M07_a3_s095_v01-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/M07_a3_s095_v01-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/fra/M07_a3_s095_v01-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

## Xhosa

<table>
  <tbody>
    <tr>
      <th style="text-align: center">xho_0050_0251778038.wav (Ground truth) </th>
      <th style="text-align: center">xho_0050_0251778038.wav (Universal vocoder) </th>
      <th style="text-align: center">xho_0050_0251778038.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_0050_0251778038-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_0050_0251778038-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_0050_0251778038-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">xho_0050_2031808299.wav (Ground truth) </th>
      <th style="text-align: center">xho_0050_2031808299.wav (Universal vocoder) </th>
      <th style="text-align: center">xho_0050_2031808299.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_0050_2031808299-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_0050_2031808299-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_0050_2031808299-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

<table>
  <tbody>
    <tr>
      <th style="text-align: center">xho_4280_6127787822.wav (Ground truth) </th>
      <th style="text-align: center">xho_4280_6127787822.wav (Universal vocoder) </th>
      <th style="text-align: center">xho_4280_6127787822.wav (EveryVoice vocoder) </th>
    </tr>
    <tr>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_4280_6127787822-gt.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_4280_6127787822-universal.wav" autoplay="">
        </audio></td>
      <td style="text-align: center"><audio controls="controls">
          <source src="/files/audios/EveryVoice-vocoder/xho/xho_4280_6127787822-everyvoice.wav" autoplay="">
        </audio></td>
    </tr>
  </tbody>
</table>
<br>

# Acknowledgement

The synthetic speech samples were constructed using a [Spanish speaker dataset](https://discourse.mozilla.org/t/sharing-my-100h-of-single-speaker-spanish/45288) with the LJSpeech format collected and validated by [Carlos Fonseca](https://github.com/carlfm01).
