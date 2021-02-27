Uliana Sadykova
===============

----------------------------------------------------------
phone:                                       +380954037296  
Email:                             ulanasadikova@gmail.com  
linkedin:                  www.linkedin.com/in/ulyalana124  

----------------------------------------------------------

About me
--------
I am student in Ukrainian academy of printing(Computer Sciense).
My goal is to became front-end developer.

Skills
----------
* HTML5
* CSS3
* Sass
* Bootstrap
* JavaScript(ES6+)

--------------------

Code Example
------------

```javascript
function timer(id, deadline) {
    function getTimeRemaining(endtime) {
        const t = Date.parse(endtime) - Date.parse(new Date()),
            days = Math.floor((t / (1000 * 60 * 60 * 24))),
            seconds = Math.floor((t / 1000) % 60),
            minutes = Math.floor((t / 1000 / 60) % 60),
            hours = Math.floor((t / (1000 * 60 * 60) % 24));

        return {
            'total': t,
            'days': days,
            'hours': hours,
            'minutes': minutes,
            'seconds': seconds
        };
    }

    function getZero(num) {
        if (num >= 0 && num < 10) {
            return '0' + num;
        } else {
            return num;
        }
    }

    function setClock(selector, endtime) {

        const timer = document.querySelector(selector),
            days = timer.querySelector("#days"),
            hours = timer.querySelector('#hours'),
            minutes = timer.querySelector('#minutes'),
            seconds = timer.querySelector('#seconds'),
            timeInterval = setInterval(updateClock, 1000);

        updateClock();

        function updateClock() {
            const t = getTimeRemaining(endtime);

            days.innerHTML = getZero(t.days);
            hours.innerHTML = getZero(t.hours);
            minutes.innerHTML = getZero(t.minutes);
            seconds.innerHTML = getZero(t.seconds);

            if (t.total <= 0) {
                clearInterval(timeInterval);
            }
        }
    }

    setClock(id, deadline);
}

export {timer};
```

Experience
----------

Education
---------
**Ukrainian Academy of Printing**  
Bachelor's degree, Computer science  
2020 - 2023  

**Technical college of national university "Lviv Polytechnic"**  
Associate's degree, Software Engineering  
2016 - 2020

Languages
---------
English - A2

