#  Hi! 👋 

```javascript
 class Specifications {
  constructor(
    public specializeIn: string,
    public purpose: string
  ) {}
}

class Favorites {
  constructor(
    public technology: string,
    public openSource: string,
    public games: string,
    public so: string
  ) {}
}

class Metadata {
  constructor(
    public name: string,
    public nationality: string,
    public specifications: Specifications,
    public favorites: Favorites
  ) {}
}

export class Person {
  private apiVersion: string;
  private kind: string;
  private metadata: Metadata;

  constructor(apiVersion: string, metadata: Metadata) {
    this.apiVersion = apiVersion;
    this.kind = "Human";
    this.metadata = metadata;
  }

  // Getters (encapsulación)
  getApiVersion(): string {
    return this.apiVersion;
  }

  getKind(): string {
    return this.kind;
  }

  getMetadata(): Metadata {
    return this.metadata;
  }

  // Método de dominio (ejemplo)
  describe(): string {
    return `${this.metadata.name} is a ${this.metadata.nationality} ${this.metadata.specifications.specializeIn}`;
  }
}

// Uso
const rogelio = new Person(
  "v32",
  new Metadata(
    "Rogelio Interino",
    "Mexican",
    new Specifications(
      "Web Developer",
      "Learn new programming languages and more about operating systems"
    ),
    new Favorites("🕸️", "💻", "🕹️", "GNU/Linux")
  )
);

console.log(rogelio.describe());
```
