# WAT test page

Self-contained HTML page to test the Website Auditing Tool: consent banner, trackers set per category, rejection, withdrawal. `?mode=noncompliant` reproduces a non-compliant site (trackers before consent, rejection ignored).


## Testing locally

To ensure that the consent banner and trackers behave correctly (especially regarding cookie storage), it is recommended to test the page using a local web server.

### Using Python
If you have Python installed, you can start a local HTTP server directly from this directory. Run the following command in your terminal:

```bash
python3 -m http.server 8000
```

Then, open your browser and navigate to [http://localhost:8000](http://localhost:8000).

### Using Node.js
Alternatively, if you have Node.js installed, you can use `serve` or `http-server`:

```bash
npx serve .
# or
npx http-server -p 8000
```

Navigate to [http://localhost:8000](http://localhost:8000) or the URL provided in your terminal.

## GDPR & Privacy Notice

Although the site can run in a "non-compliant" mode that sets cookies without consent, it does not actually collect, process, or send any information outside the browser.