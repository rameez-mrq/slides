<!-- # Slide 1 -->
<!-- .slide: data-background="white" data-transition="fade" data-auto-animate-->
<div class = "r-stack" style="position : absolute; top : 20%;">
<h2 class ="fragment fade-in-then-out" >Humanising Dialogue Agents</h2>
<h2 class ="fragment fade-in-then-out">Hey chatbot! why so serious?</h2>
<h2 data-id = "title" class ="fragment fade-in">Can chatbots exhibit mixed <span class = "fragment highlight-red">attributes?</span></h2>
</div>

<p style = "position: fixed; bottom: 2em">Rameez Qureshi</p>

<img data-id = "image1" src="media\logos\ADAPT_Logo_CMYK.png" style="position : absolute; bottom : 0; right : 0; width: 150px">
<img data-id = "image2" src="media\logos\tcd.png" style="position : absolute; bottom : 0; left : 0; width: 150px">
----

<h2 data-id = "title" style="position : absolute; top : 10%; font-size : 50px">attributes?</h2>

<ul>
    <li  style = "margin: 15px 0">Knowledgeable</li>
    <li  style = "margin: 15px 0">Empathatic</li>
    <li  style = "margin: 15px 0">Engaging</li>
    <li class = "fragment">And others...</li>
</ul>

----
<table style="font-size : 35px;  border: 1px solid white;">
    <thead>
        <tr>
            <th>Attribute</th>
            <th>Dataset</th>
            <th>Published Work</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Knowledge</td>
            <td>Wikipedia</td>
            <td>Wizard of Wikipedia: Knowledge-Powered Conversational agents, <em>Dinan et al.</em></td>
        </tr>
        <tr>
            <td>Empathy</td>
            <td>Empathetic Dialogues</td>
            <td>Towards Empathetic Open-domain Conversation Models: a New Benchmark and Dataset , <em>Rashkin et al.</em></td>
        </tr>
        <tr>
            <td>Engaging</td>
            <td>ConvAI2</td>
            <td> Conversational Intelligence Challenge 2,<em> Dinan et al.</em> </td>
        </tr>
    </tbody>
</table>
----
Wizard of Wikipedia: Knowledge-Powered Conversational agents<br><br>
<small>Dinan, Emily, Stephen Roller, Kurt Shuster, Angela Fan, Michael Auli, and Jason Weston.
</small>
--
<style type="text/css">
    .reveal p {
      text-align: left;
    }
    .reveal ul {
      display: block;
    }
    .reveal ol {
      display: block;
    }  
  </style>
  

<!-- .slide: data-auto-animate-->

Topic <!-- .element: class="fragment"-->

Apprentice <!-- .element: class="fragment"-->

Wizard <!-- .element: class="fragment"-->

--

# Dataset

<table>
    <thead>
        <tr>
            <td>Wizard of Wikipedia Task</td>
            <td>Train</td>
            <td>Valid</td>
            <td>Test Seen</td>
            <td>Test Unseen</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Number of Utterances</td>
            <td>166,787</td>
            <td>17,715</td>
            <td>8,715</td>
            <td>8,782</td>
        </tr>
        <tr>
            <td>Number of Dialogues</td>
            <td>18,430</td>
            <td>1,948</td>
            <td>965</td>
            <td>968</td>
        </tr>
        <tr>
            <td>Number of Topics</td>
            <td>1,247</td>
            <td>599</td>
            <td>533</td>
            <td>58</td>
        </tr>
        <tr>
            <td>Average Turns per Dialogue</td>
            <td>9.0</td>
            <td>9.1</td>
            <td>9.0</td>
            <td>9.1</td>
        </tr>
    </tbody>
</table>

Knowledge Database:
- 5.4M articles
- 93M sentences

--
<!-- .slide: data-background="white" data-transition="fade" data-auto-animate-->
# Architecture
<figure>
<img src="\pres\figures\7april22\wow_arch.png">
<figcaption style="font-size: medium;"><b>Generative Transformer Memory Network</b>: An IR system provides knowledge candidates from Wikipedia. Dialogue Context and Knowledge are encoded using a shared encoder. In the Two-stage model, the dialogue and knowledge are re-encoded after knowledge selection.</figcaption>
</figure>
--

<img  src="\pres\figures\7april22\WOW.png" style="max-width: 130%; padding: 0;">


----
Towards Empathetic Open-Domain Conversation Models:<br>A New Benchmark and Dataset<br><br>
<small>Rashkin, Hannah, Eric Michael Smith, Margaret Li, and Y.-Lan Boureau.</small>

--
# Empathetic Dialogue bot
<!-- .slide: data-background="white" data-transition="fade" data-auto-animate-->
<img  src="\pres\figures\7april22\emp_arch.png" style="max-width: 50%; padding: 0;">

--
# Dataset

<table><thead><tr><th>Conversations</th><th>24,850</th></tr></thead><tbody><tr><td>Participant</td><td>810</td></tr><tr><td>Avg. Utterance</td><td>4.31</td></tr></tbody></table>

--
# Architecture
<!-- .slide: data-background="white" data-transition="fade" data-auto-animate-->
<img src="\pres\figures\7april22\emp_arch_1.png" style="max-width: 70%; padding: 0;">
<!-- <figcaption style="font-size: medium;">Left: In the retrieval set-up, each candidate y is tokenized into y1, y2, · · · and encoded into vector hy by the candidate encoder. The system outputs the candidate y∗ that maximizes dot product hx · hy. Right: In the generative set-up, the encoded context hx is used as input to the decoder to generate start symbol </s> and tokens y1, y2, · · · . The model is trained to minimize the negative loglikelihood of target sequence  ̄ y conditioned on context.</figcaption> -->

--
<img src="\pres\figures\7april22\emp.png" style="max-width: 130%; padding: 0;">


----

Can You Put it All Together:<br>Evaluating Conversational Agents' Ability to Blend Skills<br><br>
<small>Smith, Eric Michael, Mary Williamson, Kurt Shuster, Jason Weston, and Y.-Lan Boureau.
</small>


--
Skills Attributed:

- Knowledge
- Empathy 
- Personality

--


# Dataset

<table><thead><tr><th>Conversations</th><th>6,808</th></tr></thead><tbody><tr><td>Participants</td><td>2,679</td></tr><tr><td>Avg. Utterance</td><td>11.2</td></tr></tbody></table>

--
<!-- <table style="border-collapse:collapse;border-spacing:0" class="tg"><thead><tr><th style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">Mode Count</th><th style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">Conversation</th><th style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">Pct (%)</th></tr></thead><tbody><tr><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">1</td><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">51</td><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">6.9%</td></tr><tr><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">2</td><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">167</td><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">22.6%</td></tr><tr><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">3</td><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">290</td><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">39.2%</td></tr><tr><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">4</td><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">232</td><td style="border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">31.4%</td></tr></tbody></table> -->
<table style="text-align: center;"><thead><tr><th>Skills Count</th><th>Conversation</th><th>Pct (%)</th></tr></thead><tbody ><tr><td>1</td><td>51</td><td>6.9%</td></tr><tr><td>2</td><td>167</td><td>22.6%</td></tr><tr><td>3</td><td>290</td><td>39.2%</td></tr><tr><td>4</td><td>232</td><td>31.4%</td></tr></tbody></table>
<figcaption style="font-size: large;">Breakdown of conversations by number of modes, showing that most BST dataset conversations exhibit multiple modes.</figcaption>
--
Two types of models

- Multi-task Single-Skills
- Multi-task Two-Stage



--
<!-- .slide: data-background="white" data-transition="fade" data-auto-animate-->
# Hits@1
<img src="\pres\figures\7april22\blend_res.png" style="max-width: 130%; padding: 0;">


--

<!-- .slide: data-background="white" data-transition="fade" data-auto-animate-->

<img src="\pres\figures\7april22\blen_res_human.png" style="max-width: 130%; padding: 0;">
<figcaption style="font-size: large;"><b>Human Evaluation</figcaption>
--

<img src="\pres\figures\7april22\conv_blender.png" style="max-width: 130%; padding: 0;">

--

<!-- .slide: data-background-iframe="pres\figures\7april22\Smith et al. - 2020 - Can You Put it All Together Evaluating Conversati.pdf#view=FitH" -->
<!-- <iframe src="pres\figures\7april22\Smith et al. - 2020 - Can You Put it All Together Evaluating Conversati.pdf" width="120%" height="500em"> -->
----
## Current Work


--

# Motivation

<blockquote style="text-align: justify; width: 100%; font-style: normal;">The model should be able to <span class = "fragment highlight-red" data-fragment-index="1">showcase multiple attributes</span> in a single reply as per the situation. Therefore, the architecture should be capable of <span class = "fragment highlight-blue" data-fragment-index="2">percieving</span> the current intent/emotion of the user and <span class = "fragment highlight-blue" data-fragment-index="2">taking action</span> accordingly.</blockquote>

--

Merging Knowledge

<img src="\pres\figures\7april22\arch_worl.png" style="max-width: 80%; padding: 0;">


--
Perceiving-Acting

<img src="\pres\figures\7april22\arch_wrl.png" style="max-width: 80%; padding: 0;">


--
<img src="\pres\figures\7april22\conv_proposed.png" style="max-width: 130%; padding: 0;">


----
## Challenges
--

Different Encoders require different inputs based on different datasets.


--
<!-- .slide: data-background-iframe="https://parl.ai/" -->

<div style="position: absolute; width: 40%; bottom: 0; right: 0; box-shadow: 0 1px 4px rgba(0,0,0,0.5), 0 5px 25px rgba(0,0,0,0.2); background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; font-size: 20px; text-align: left; margin-bottom: 0%; margin-right: 0em;">
    <h2>ParlAI Framework</h2>
    <p>As all the SOTA dialogue models follow ParlAI strucuture, therefore the proposed model has to be written with ParlAI subclasses.</p>
</div>

--
Train DRL Agent, or Decoder, or both simultaneously?

----

Thank you!<p class ="fragment fade-in" style="position: absolute;  bottom: 0;">Questions?</p>

----

References

- <sub>Dinan, Emily, Stephen Roller, Kurt Shuster, Angela Fan, Michael Auli, and Jason Weston. "Wizard of Wikipedia: Knowledge-Powered Conversational Agents." ArXiv:1811.01241 [Cs], February 21, 2019. http://arxiv.org/abs/1811.01241.</sub>
- <sub>Rashkin, Hannah, Eric Michael Smith, Margaret Li, and Y.-Lan Boureau. "Towards Empathetic Open-Domain Conversation Models: A New Benchmark and Dataset." ArXiv:1811.00207 [Cs], August 28, 2019. http://arxiv.org/abs/1811.00207.</sub>
- <sub>Roller, Stephen, Emily Dinan, Naman Goyal, Da Ju, Mary Williamson, Yinhan Liu, Jing Xu, et al. "Recipes for Building an Open-Domain Chatbot." ArXiv:2004.13637 [Cs], April 30, 2020. http://arxiv.org/abs/2004.13637.</sub>
- <sub>Smith, Eric Michael, Mary Williamson, Kurt Shuster, Jason Weston, and Y.-Lan Boureau. "Can You Put It All Together: Evaluating Conversational Agents" Ability to Blend Skills." ArXiv:2004.08449 [Cs], April 17, 2020. http://arxiv.org/abs/2004.08449.</sub>

