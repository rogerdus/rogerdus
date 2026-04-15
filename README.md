<h1 align="center">Hi 👋, I'm Rogelio</h1>
<h3 align="center">💻 Web Developer from Mexico 🇲🇽</h3>

---

## 🧑‍💻 About Me (as code)

```ts
class Developer {
  constructor(
    public name: string,
    public nationality: string,
    public role: string,
    public purpose: string,
    public favorites: {
      technology: string;
      openSource: string;
      games: string;
      os: string;
    }
  ) {}

  introduce() {
    return `Hi! 👋 I'm ${this.name}, a ${this.nationality} ${this.role}.`;
  }
}

const me = new Developer(
  "Rogelio Interino",
  "Mexican 🇲🇽",
  "Web Developer",
  "Learning new programming languages and exploring operating systems",
  {
    technology: "🕸️",
    openSource: "💻",
    games: "🕹️",
    os: "GNU/Linux 🐧",
  }
);
