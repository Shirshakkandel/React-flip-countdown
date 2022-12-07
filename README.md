# **Coming-soon using @leenguyen/react-flip-clock-countdown** 

# Preview
![Page Preview](/public/preview.png)

[Npm link of package](https://www.npmjs.com/package/@leenguyen/react-flip-clock-countdown)

## Guild to install
1. install repo
2. install package using yarn 
3. open website using command yarn start.

```javascript
//App.js
import FlipClockCountdown from '@leenguyen/react-flip-clock-countdown';
import '@leenguyen/react-flip-clock-countdown/dist/index.css';
import './styles.css';

const App = ()=> {
  return (
   <FlipClockCountdown className="flip-clock"
    to={new Date().getTime() + 24 * 3600 * 1000 + 5000} />
  )
}

```

```css
//styles.css
  .flip-clock {
     --fcc-flip-duration: 0.5s; /* transition duration when flip card */
  --fcc-digit-block-width: 30px; /* width of digit card */
  --fcc-digit-block-height: 60px; /* height of digit card, highly recommend in even number */
  --fcc-digit-font-size: 30px; /* font size of digit */
  --fcc-digit-color: #000000; /* color of digit */
  --fcc-label-font-size: 14px; /* font size of label */
  --fcc-label-color: #fff; /* color of label */
  --fcc-background: #ffffff; /* background of digit card */
  --fcc-divider-color: #000000; /* color of divider */
  --fcc-divider-height: 1px; /* height of divider */
  --fcc-separator-size: 6px; /* size of colon */
  --fcc-separator-color: #fff; /* color of colon */
  }

/* screens bigger than 900px */
@media (min-width: 900px) {
  .page h1 {
    font-size: 4rem;
  }
  .page h3 {
    max-width: 600px;
  }
  .flip-clock {
    --fcc-digit-block-width: 80px;
    --fcc-digit-block-height: 120px;
    --fcc-digit-font-size: 60px;
    --fcc-label-font-size: 20px;
  }
}

```