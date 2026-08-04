## Hi, I'm Sanika 👋

Full-stack developer in Toronto. I build things end to end — design, backend, auth, deploy — and I care about what happens after the demo works.

**Open to junior / new-grad roles.**

---

### 🌿 Sattvic — Ayurvedic meal planner

**[sattvic.vercel.app](https://sattvic.vercel.app)** · [source](https://github.com/sam21270/sattvic)

Answer nine questions instead of keeping a food diary. It plans your week around your Ayurvedic constitution, counts the protein, and decides dinner before you get home.

`Next.js 16` `React 19` `TypeScript` `Tailwind 4` `MongoDB` `NextAuth v5` `Groq / Claude`

Built and shipped solo. The parts I'm proudest of aren't the features:

- **Blocked an SSRF hole** in the recipe importer — it fetched any URL a caller passed, so `169.254.169.254` would have returned cloud metadata. Now every redirect hop is re-checked against loopback, RFC1918, link-local and CGNAT ranges.
- **Cut the data I store.** Friend requests were writing the sender's email and real name into the recipient's record. Neither is needed to accept a request, so both are gone from the schema — plus a script to purge what was already written.
- **Locked down the browser** with a CSP, per-IP rate limiting on the AI routes, and profiles that are private until you opt in.

---

### Also built

**[online-doctor-app](https://github.com/sam21270/online-doctor-app)** — medical appointment platform with separate patient, doctor and admin portals.

**[rahul-electroplaters](https://github.com/sam21270/rahul-electroplaters)** — business site built and deployed for a real client.

---

### Working with

TypeScript · React · Next.js · Node · MongoDB · Tailwind · Vercel

### Currently learning

Shipping a real app to real people taught me more than any tutorial. What I've been
digging into, mostly because production made me:

- **Web security** — CSP and what it actually blocks, SSRF and why you re-check every
  redirect hop, IDOR, rate limiting, and deciding authorisation from the session
  instead of trusting anything the client sends
- **Privacy by design** — storing the minimum, defaulting profiles to private, and
  writing the script that deletes someone completely when they ask
- **Auth** — OAuth with NextAuth, session handling, and the difference between "signed
  in" and "allowed to read this"
- **Databases** — schema design in MongoDB, and scoping Atlas roles to least privilege
- **Testing** — unit tests for the logic that fails silently: scoring, access rules,
  the blocked-address list
- **Debugging production** — reading runtime logs to find things that only break once
  deployed, which is a completely different skill from fixing them locally
- **LLM integration** — turning "2 rotis, dal and a glass of buttermilk" into structured
  macros, and handling the times the model returns nonsense
- **Responsive CSS** — mostly by getting it wrong on a phone first

📫 [LinkedIn](https://www.linkedin.com/in/sanikashah-dev/)
