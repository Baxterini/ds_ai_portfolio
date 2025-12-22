# n8n Image Recognition — AI Image Description via Webhook

Projekt pokazuje prostą, ale praktyczną automatyzację w **n8n**, która przyjmuje **URL obrazka** przez webhook, wysyła go do analizy przez model AI (vision), a następnie zwraca **ustrukturyzowaną odpowiedź JSON** z opisem.

---

## Co robi ten workflow?

- Przyjmuje zapytanie na endpoint webhooka z parametrem `image_url`
- Waliduje wejście (czy link istnieje / ma sens)
- Pobiera obraz (HTTP Request)
- Analizuje zawartość obrazu przez AI (node *Analyze image*)
- Zwraca odpowiedź do klienta (node *Respond to Webhook*)

---

## Przykład odpowiedzi (JSON)

Zwracane pola:
- `ok` — status wykonania
- `image_url` — źródłowy URL obrazka
- `description` — opis wygenerowany przez AI

---

## Dlaczego to ważne?

To gotowy wzorzec do zastosowań „real-life”, np.:
- automatyczne opisy zdjęć produktowych (e-commerce)
- moderacja treści / wstępna kategoryzacja obrazów
- generowanie alt-textów (SEO / accessibility)
- integracje: Slack / email / CRM / Notion / Google Sheets

---

## Technologie

- **n8n** — workflow automation
- **Webhook + HTTP Request** — wejście i pobranie obrazu
- **AI Vision model** — analiza zdjęcia i generowanie opisu
- **JSON output** — prosty format do integracji z innymi systemami

---

## Screenshots

### Workflow
![Workflow](../img/workflow%20n8n.png)

### API Response
![API Response](../img/output%20n8n.png)

### Example Image
![Example Image](../img/screen%20n8n.png)
