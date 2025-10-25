# HAVENIS AI – Netlify Upload Paket

Inhalt
- index.html (Landingpage, Netlify Forms integriert)
- thanks.html (Erfolgsseite nach Formular-Submit)
- netlify.toml (Security-Header)
- robots.txt

Deploy (manuell)
1) Alle Dateien in einen Ordner legen und als ZIP packen
2) Netlify Dashboard → Add new site → Deploy manually → ZIP hochladen

Netlify Forms
- Forms sind bereits markiert (name="contact" / name="newsletter", data-netlify, honeypot, action="/thanks")
- Nach dem ersten Submit unter Site settings → Forms → Form notifications:
  - E-Mail-Notification für **contact** an havenis-ai@web.de
  - E-Mail-Notification für **newsletter** an havenis-ai@web.de

Hinweise
- Reply-To: Netlify setzt die Reply-To auf das Feld `email` im Formular, so dass Antworten an den Absender gehen.
- Double-Opt-In (Newsletter): Optional via Brevo/Mailchimp über Webhook/Zapier/Make.
- Impressum/Datenschutz: Inhalte in index.html bereits enthalten (UG i.G., Fürstenwalde).