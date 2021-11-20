### Hi, I'm Tarcizio ![some-gif](https://media.giphy.com/media/uB6eLycBCOl68/giphy.gif)

```typescript
interface IAboutInfos {
  name: string;
  someDescription: string;
  currentWorking: string;
  askmeAbout: string[];
  funFact: string;
}

class TarcizioRepository implements ITarcizioRepository {
  someInfosAboutMe = [];

  async create({
    name = "Tarcizio",
    someDescription = "Graduated in Production Engineering. I saw in the program an opportunity to solve the problems",
    currentWorking = 'Quality Control Assistant at Dislog',
    askmeAbout = ['TypeScript', 'NodeJS', 'PrismaJS', 'NextJS'],
    funFact = 'World of Warcraft player and lover of stars, planets and galaxies',
  }: IAboutInfos): Promise<void> {
    const tarcizioAlreadyExists = this.someInfosAboutMe.find(
      (value) => value.name === name
    );

    if (tarcizioAlreadyExists) {
      throw new Erro("This is impossible! 🙀");
    }

    const tarcizio = new TarcizioModel();

    Object.assign(tarcizio, {
      name,
      someDescription,
      currentWorking,
      askmeAbout,
      funFact,
    });

    this.someInfosAboutMe.push(tarcizio);
  }
}

export { TarcizioRepository };

```

## Leave a ✨ if you want to modify this README and reach me on social media below.
[![LinkedIn](https://img.shields.io/badge/LinkedIn-tarcizio--barbosa-informational)](https://www.linkedin.com/in/tarcizio-barbosa/)
[![Twitter](https://img.shields.io/badge/Twitter-%40t__tarcizio-blue)](https://twitter.com/t_tarcizio)

Last Edited On: 19/11/2021
