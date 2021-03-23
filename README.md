## Tarcizio Barbosa

### About Me

```typescript
interface BioProperties {
  someDescription: string;
  currentWorking: string;
  currentLearning: Array<string>;
  reachme: object;
}

const tarcizioBarbosa: BioProperties = {
  someDescription: `🕺 Graduated from a year in production engineering, 
  I saw in the program an opportunity to solve the routine problems within my area of expertise. 
  I currentlyconsider myself a beginner developer.`,
  currentWorking: '✔ Quality Control Assistant',
  currentLearning: [
    'JavaScript',
    'TypeScript',
    'NodeJS',
    'TypeORM',
    'Python',
    'Power BI',
  ],
  reachme: {
    Linkedin: '🎈 www.linkedin.com/in/tarcizio-barbosa-552b2a208',
    Twitter: '💙 @t_tarcizio',
    Github: 'github.com/tarcizio-barbosa',
  },
};

function getBio(properties: BioProperties) {
  return properties;
}

getBio(tarcizioBarbosa);
```

## Leave a ✨ if you want to modify this README.

Last Edited On: 23/03/2021
