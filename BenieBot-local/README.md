# BenieBot-Wordpress
Implementation code for wordpress, copy and paste in the body section:
```
<body>
<link rel="stylesheet" href="style.css"> 
<div class="disclaimer" style="display: none;">
    <button onclick="closeDisclaimer()"  class="closingbutton1" >×</button>
    <div class="chatbot__prechat-custom">
      <h2 class="title-general">General Disclaimer</h2>
      <p>Your cooperation is highly appreciated. In our continuous pursuit of excellence, we present our Beta Chatbot,
        Benie, to enhance your experience on our site:</p>
      <ul>
        <li>This is a beta version, subject to refinements.</li>
        <li>Your valuable feedback guides our enhancements.</li>
        <li>Minor imperfections may be present.</li>
        <li>Your cooperation is highly appreciated.</li>
        <li>When interacting with Benie, please do not include any personal information.</li>
      </ul>
      <p>Your interaction with Benie, the chatbot, is instrumental in our quest to deliver the best possible service.
      </p>
      <span class="chatbot__error" id="js-chatbot-error" role="alert" aria-atomic="true"
        data-error-agree="You must agree to the disclaimers to activate the Virtual Assistant."></span>
      <p></p>
      <input type="checkbox" name="" id="agreementCheckbox" class="custom-checkbox"> I agree
      <div class="ContinueBot">
        <button class="styleButton" id="openNewWindow">Continue</button>
      </div>
    </div>
  </div>

  <img src="chatbot.png" class="chatbot_icon" id="chaatbot_icon"> 
  

  <div class="beniebot">
    <button onclick="closeBenieBot()" class="closingbutton2">×</button>
	<button onclick="refresh()" class="refresh">⟳</button>
    <iframe class= "beniebotIframe" id="beniebotIframe" src="beniebot.html" width="100%"
      height="100%" frameborder="0" loading="lazy"></iframe>
  </div>
</body>
<script src="index.js">
</script>
\```
