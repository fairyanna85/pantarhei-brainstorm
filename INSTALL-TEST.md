# Install test (T-CREATE-8)

| Path | Result | Notes |
|---|---|---|
| Claude Code plugin manifest | PASS | `claude plugin validate .` → "Validation passed". Advisory notes: `homepage`/`repository` hold `<owner>` placeholders (not https; resolved in Phase 4); listing icon needs a square PNG 512–2048 px (current `social-preview.png` is 1280×640). Both are listing-only and do not change the result. |
| Claude Code live install (`/plugin marketplace add`) | NOT RUN | Needs the public GitHub repo (blocked by Phase 0.1/0.2). |
| Claude apps ZIP upload | NOT RUN, manual | Steps from support.claude.com: Customize > Skills > + > Create skill > Upload a skill. See E-9: the help article states a 200-character `description` limit; only a real upload settles it. |
| Hermes Agent install | NOT RUN, manual | Needs the public repo URL. |
| Generic Agent Skills client | NOT RUN, manual | Copy `skills/pantarhei-brainstorm/` into the client's skills folder. |
