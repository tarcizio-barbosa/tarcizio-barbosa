![some-gif](https://wmunpogjgutrfetkhfql.supabase.in/storage/v1/object/public/candidate-pictures/my-images/giphy2.gif)![some-gif](https://wmunpogjgutrfetkhfql.supabase.in/storage/v1/object/public/candidate-pictures/my-images/giphy2.gif)![some-gif](https://wmunpogjgutrfetkhfql.supabase.in/storage/v1/object/public/candidate-pictures/my-images/giphy2.gif)

### Hi, I'm Tarcizio

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

## Leave a ✨ if you want to modify this README.

Last Edited On: 26/10/2021
