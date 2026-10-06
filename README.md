SUPPORT CONVERSATION SIMULATOR FOR RISE 360
===========================================

Files
-----
SupportConversationSimulator-Rise360.html
  A self-contained, responsive HTML component. It needs no external libraries,
  fonts, images, API calls, or server-side code.

What it does
------------
1. /scenario updates the issue bullet and customer message.
2. The issue and customer message stay synchronized in the agent inbox and
   customer mobile preview.
3. /reply appends an agent response to both previews.
4. Reset restores the example scenario.

Recommended Rise 360 integration
--------------------------------
Rise 360's Embed block expects externally hosted content. Upload the HTML file
(or the folder containing it) to an HTTPS-accessible host, then add an Embed
block in Rise and paste an iframe that points to the hosted file.

Example iframe, replacing YOUR_HOSTED_URL with the real HTTPS URL:

<iframe
  src="YOUR_HOSTED_URL/SupportConversationSimulator-Rise360.html"
  title="Support Conversation Simulator"
  width="100%"
  height="1100"
  style="border:0; display:block;"
  allow="clipboard-write"
></iframe>

If your hosting platform provides an embed snippet, use that snippet directly
in Rise instead. The component is responsive and can also be opened directly
in a browser for testing.

Important
---------
- The simulator is client-side only. Changes reset when the page is reloaded.
- The component does not send or store learner data.
- If the host blocks iframe embedding with CSP or X-Frame-Options, use a host
  that permits embedding from your Rise environment.
- Keep the HTML on HTTPS so it can be embedded in a secure Rise course.
