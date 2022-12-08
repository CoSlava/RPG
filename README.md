# coad549f7b4c49ae211d67710

Quick start:

```
$ npm install
$ npm start
````

Head over to https://vitejs.dev/ to learn more about using vite


////////////////////////* Extended classes: *\\\\\\\\\\\\\\\\\\\\\\\\\\\\


class Player {
    constructor(name, country) {
        this.name = name;
        this.country = country;
    }
    
    introduce() {
        console.log(`${this.name} was born in ${this.country}`);
    }
}

const messi = new Player("Messi", "Argentina");

messi.introduce();

class TennisPlayer extends Player {
    constructor(name, country, age) {
        super(name, country);
        this.age = age;
    }
    
    playTennis() {
        console.log(`${this.name} is ${this.age} years old and knows how to play Tennis`);
    }
}

const roger = new TennisPlayer( "Roger Federer", "Spain", 38);

roger.introduce();
roger.playTennis();
