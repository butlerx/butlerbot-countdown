# butlerbot-countdown

countdown plugin for butlerbot


## Install

```sh
yarn add butlerbot-countdown
```
Create a file in the plugin dir as follows

```js
import countdown from 'butlerbot-countdown';
export default countdown({
  development: {
    letterOptions: {
      vowels: {
        A: 15,
        E: 21,
        I: 13,
        O: 13,
        U: 5,
      },
      consonants: {
        B: 2,
        C: 3,
        D: 6,
        F: 2,
        G: 3,
        H: 2,
        J: 1,
        K: 1,
        L: 5,
        M: 4,
        N: 8,
        P: 4,
        Q: 1,
        R: 9,
        S: 9,
        T: 9,
        V: 1,
        W: 1,
        X: 1,
        Y: 1,
        Z: 1,
      },
    },

    numberOptions: {
      large: ['25', '50', '75', '100'],
      small: [
        '1',
        '2',
        '3',
        '4',
        '5',
        '6',
        '7',
        '8',
        '9',
        '10',
        '1',
        '2',
        '3',
        '4',
        '5',
        '6',
        '7',
        '8',
        '9',
        '10',
      ],
    },

    roundOptions: {
      letters: [1, 2, 4, 5, 7, 8, 10, 11, 12, 13],
      numbers: [3, 6, 9, 14],
      lettersRoundMinutes: 2,
      numbersRoundMinutes: 5,
      conundrumRoundMinutes: 2,
      secondsBeforeConundrum: 15,
      minimumVowels: 3,
      minimumConstant: 3,
    },

    gameOptions: {
      setTopic: true,
      topicBase: '|| Dev Bot || Expect spam || Expect breakings',
      minutesBeforeStart: 2,
      roundMinutes: 2,
      maxIdleCount: 3,
    },

    pluginOptions: {
      channels: ['#butlerbot'],
      channelsToExclude: [],
      channelsToJoin: ['#butlerbot'],
    },
  },

  production: {
    letterOptions: {
      vowels: {
        A: 15,
        E: 21,
        I: 13,
        O: 13,
        U: 5,
      },
      consonants: {
        B: 2,
        C: 3,
        D: 6,
        F: 2,
        G: 3,
        H: 2,
        J: 1,
        K: 1,
        L: 5,
        M: 4,
        N: 8,
        P: 4,
        Q: 1,
        R: 9,
        S: 9,
        T: 9,
        V: 1,
        W: 1,
        X: 1,
        Y: 1,
        Z: 1,
      },
    },

    numberOptions: {
      large: ['25', '50', '75', '100'],
      small: [
        '1',
        '2',
        '3',
        '4',
        '5',
        '6',
        '7',
        '8',
        '9',
        '10',
        '1',
        '2',
        '3',
        '4',
        '5',
        '6',
        '7',
        '8',
        '9',
        '10',
      ],
    },

    roundOptions: {
      letters: [1, 2, 4, 5, 7, 8, 10, 11, 12, 13],
      numbers: [3, 6, 9, 14],
      lettersRoundMinutes: 2,
      numbersRoundMinutes: 5,
      conundrumRoundMinutes: 2,
      secondsBeforeConundrum: 15,
      minimumVowels: 3,
      minimumConstant: 3,
    },

    gameOptions: {
      setTopic: true,
      topicBase: '|| wiki: https://github.com/butlerx/butlerbot/wiki/Countdown',
      notifyUsers: false,
      minutesBeforeStart: 2,
      maxIdleCount: 3,
    },

    pluginOptions: {
      channels: ['#butlerbot'],
      channelsToExclude: [],
      channelsToJoin: ['#butlerbot'],
    },
  },
});
```
