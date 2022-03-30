![Profile Foto](./img/565940248.jpg)

# Suhov Oleg

***

### Contacts: 

***

### Tel: +998903219090
### Gmail: aheronlcv@gmail.com
### Discord: Oleja(Aheron666)

***

## About my self:

##### Straightforwardness, ambition, perfectionism, adherence to principles, communication skills, a great desire to get into the IT, 2021/06 i dischared from my job and devoted all time to training IT courses, main priorities: gaining work experience, pumping my own skills in the Front-End, mastering new skills and a new profession. I am ready to try my hand at both programming and project management, I want to connect my life with IT, because, unlike primary education, the choice of this direction was more conscious, I am ready to work and train for free to obtain the necessary knowledge and experience!
## Skills

- HTML/CSS/SASS  - Two month in ITStep accedemy
- JavaScript (ES6+) - Beginning lavel (four month in ITStep accedemy)
- React JS - Beginning lavel (ItGid courses)

*** 

## Code example

```class Timer {
  constructor(count) {
    this.count = this.breakCount = this.seconds = this.minute = count;
    this.timer;
    this.breakTime;
  }

  setSession() {
    const timerFunction = (event) => {
      let eventTarget = event.target.parentNode;
      if (eventTarget.id === 'changeSessionTime') return false;
      if (eventTarget.id === 'arrowUp') {
        this.count += 5;
        changeSessionTime.innerHTML = this.count + ' min';
      }
      if (eventTarget.id === 'arrowDown') {
        this.count -= 5;
        changeSessionTime.innerHTML = this.count + ' min';
        if (this.count <= 0) {
          this.count = 0;
          changeSessionTime.innerHTML = '0 min';
        }
      }
      timerCount.innerHTML = this.count + ':00';
      if (this.count < 10) {
        timerCount.innerHTML = '0' + this.count + ':00';
      }
      this.seconds = this.count * 60;
    };

    setSessionTime.addEventListener('click', timerFunction);
  }

  setBreak() {
    const breakFunction = (event) => {
      let eventTarget = event.target.parentNode;
      if (eventTarget.id === 'changeBreakTime') return false;
      if (eventTarget.id === 'BreakArrowUp') {
        this.breakCount += 1;
        changeBreakTime.innerHTML = this.breakCount + ' min';
      }
      if (eventTarget.id === 'BreakArrowDown') {
        this.breakCount -= 1;
        changeBreakTime.innerHTML = this.breakCount + ' min';
        if (this.breakCount <= 0) {
          this.breakCount = 0;
          changeBreakTime.innerHTML = '0 min';
        }
      }
      this.breakTime = this.breakCount * 60;
    };

    setBreakTime.addEventListener('click', breakFunction);
  }

  startTimer() {
    let count = 0;
    let minute;
    let seconds = 0;
    let timerSoundBreak = new Audio(
      './audio/effekt-obratnogo-otscheta-dlya-metallicheskih-hitov-43186 (mp3cut.net).mp3'
    );
    let timerSoundSession = new Audio(
      './audio/effekt-obratnogo-otscheta-dlya-metallicheskih-udarov-40144 (mp3cut.net).mp3'
    );
    const timerStart = () => {
      if (this.seconds > 0 && this.breakTime > 0) {
        clearInterval(this.timer);
        this.timer = setInterval(() => {
          this.seconds -= 1;
          this.minute = Math.floor(this.seconds / 60);
          if (this.seconds < 0 && count === 0) {
            this.seconds = this.breakTime;
            count = 1;
            timerSoundBreak.play();
          }
          if (this.seconds < 0 && count === 1) {
            this.seconds = this.count * 60;
            count = 0;
            timerSoundSession.play();
          }
          seconds -= 1;
          if (seconds < 0) {
            seconds = 59;
          }
          minute = this.minute;
          if (seconds < 10) seconds = '0' + seconds;
          if (minute < 10) minute = '0' + minute * 1;
          timerCount.innerHTML = minute + ':' + seconds;
        }, 1000);
      }
    };
    btnStart.addEventListener('click', timerStart);
  }

  timerPause() {
    pauseButton.style.display = 'none';
    const hidePause = () => {
      if (
        pauseButton.style.display === 'none' &&
        this.seconds != 0 &&
        this.breakCount != 0
      ) {
        pauseButton.style.display = 'inline-block';
        startButton.style.display = 'none';
      } else {
        pauseButton.style.display = 'none';
        startButton.style.display = 'inline-block';
        clearInterval(this.timer);
      }
    };
    const setBreak = () => {
      if (this.breakCount === 0 && this.seconds > 0)
        alert('Please enter Break Time');
      if (this.seconds === 0) alert('Please enter Session Time');
    };

    btnStart.addEventListener('click', hidePause);
    btnStart.addEventListener('click', setBreak);
  }

  resetButton() {
    const clearTimer = () => {
      timerCount.innerHTML = '00:00';
      changeSessionTime.innerHTML = changeBreakTime.innerHTML = '0 min';
      pauseButton.style.display = 'none';
      startButton.style.display = 'inline-block';
      clearInterval(this.timer);
      this.seconds = this.count = this.breakCount = 0;
    };

    btnReset.addEventListener('click', clearTimer);
  }
  timerSounds() {
    const sessionEndSound = () => {};
  }
}

let timer = new Timer(0);
timer.setSession();
timer.startTimer();
timer.timerPause();
timer.setBreak();
timer.resetButton();
```

## Experience

I have practical experience in doing homework and projects in courses, I also prepared several projects for my portfolio:

- [Pomodoro timer JS](https://github.com/Aheron666/pomodoro-timer-js.git).
- [Landing page JS](https://github.com/Aheron666/Landing-page.git).
- [Login pages JS](https://github.com/Aheron666/Login-page.git).
- [Canvas & Cookie JS](https://github.com/Aheron666/Canvas-cookie-elements.git).
- [Timer JS](https://github.com/Aheron666/Timer-JS.git).

## Education

- #### Gubkin University of Oil & Gas
- #### ITStep Accedemy
- #### ItGid ReactJS

## Languages 

- #### English - B1





