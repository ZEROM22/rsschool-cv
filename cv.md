# Aleksandr Saliakhov

---
## Contact information:
**Phone:** +7 951 961 0973 \ +995 55 112 2941<br>
**E-mail:** salyahov.sasha@mail.ru<br>
**Telegram:** @asalyahov

---
## About me:
I am 26 years old, currently I work in SAP EWM technical support, but I have always dreamed of working as a programmer.<br>
He graduated from the university with a technical degree, after which he began working with SAP, studying programming in his spare time and doing his own projects using technologies such as React, Bootstrap, MUI, NodeJS, Express, Socket.IO, Mongoose.<br>
At the moment I am studying at the RS School, the main goal for myself is to learn from people who already work in this field, and to close knowledge gaps.
### My strengths
- Independence
- Ability to deal with a problem
- I learn new things quickly
- Desire to learn and grow in the IT field

---
## Skills and Proficiency:
- **Language**: HTML, CSS, JavaScript
- **Framework**: React, Redux, Bootstrap, MUI
- **Backend**: Node.js, Express, Socket.IO
- **Database**: Mongoose, SQLite
- **Pattern**: OOP, MVC
- **Version control**: Git, GitHub
- **Methodology**: Agile, BEM Methodology

---
### Code example:
**Human readable duration format**<br>
***Description:***<br>
Your task in order to complete this Kata is to write a function which formats a duration, given as a number of seconds, in a human-friendly way.<br>
The function must accept a non-negative integer. If it is zero, it just returns **"now"**. Otherwise, the duration is expressed as a combination of **years**, **days**, **hours**, **minutes** and **seconds**.
It is much easier to understand with an example:
>For seconds = 62, your function should return 
    "1 minute and 2 seconds"
For seconds = 3662, your function should return
    "1 hour, 1 minute and 2 seconds"

***Solution:***
```javascript
function formatDuration (seconds) {
  if (!seconds) return "now"
  
  const y = Math.floor(seconds / 31536000);
  const d = Math.floor((seconds - (y * 31536000)) / 86400);
  const h = Math.floor((seconds - (y * 31536000 + d * 86400)) / 3600);
  const m = Math.floor((seconds - (y * 31536000 + d * 86400 + h * 3600)) / 60);
  const s = seconds - (y * 31536000) - (d * 86400) - (h * 3600) - (m * 60);
  
  const array = [y,d,h,m,s];
  const name = [" year"," day"," hour"," minute"," second"];

  const output = [];
  
  array.forEach((t,i)=>{
    if (t) t > 1 ? output.push(t + name[i]+"s") : output.push(t + name[i]);
  })

  if (output.length === 1) return output[0];
  else {
    let lastItem = output.pop();
    return output.join(", ") + " and " + lastItem;
  }
}
```

---
### Experience:
**TeamIdea (LLC TIMIDEA GROUP)**
***SAP EWM Consultant***
*August 2022 - current time*
* Support for the operation of the SAP system
* Escalation of problematic incidents
* Primary processing and routing of incoming requests

**SIBINTEK LLC IC**
***SAP Purchasing Lead Specialist***
*October 2020 — August 2022*
* Support for the operation of the SAP system
* Implementation of improvements
* Testing
* User Accompaniment
* Incident resolution

**My pet projects:**
- Chat room creation function (design copied from Persona 5 video game):<br>
https://persona-chat.herokuapp.com
- Payment form with validation on the client and server side with saving in mongo atlas (cloud database):<br>
https://payment-page.herokuapp.com
- List of video games for the current year with sorting and filters, RESTful backend, using 3rd party API:<br>
https://gamelist-current-year.herokuapp.com
- Calendar with the ability to add / remove events for the required period of time (test task for a vacancy):<br>
https://calendar-uchi.herokuapp.com
- SPA application on React, completed tasks are stored in branches, in each of which new functionality was added. Assignment for the course “Immersion in React” from Y_LAB University:<br>
https://github.com/ZEROM22/react-webinar-2

---
### Education:
* **University**: Nizhnevartovsk State University, Faculty of Technology and Engineering, Master's Degree


---
### Courses:
- YLab University Course ["Immersion in React"](https://ylab.io/upload/certificates/reactjs/vuvX1f0LDBU1FGxIGfta.pdf)
- RS Schools Course «JavaScript/Front-end» (in progress)

---
### Languages:
* **Russian** - Native
* **English** - A2