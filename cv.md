# Agliullin Dmitry
| Source | Contact |
| ------ | ------ |
| 📞 **Phone** | +7 9224 221144 |
| 💾 **GitHub** | [dmitryAgli](https://github.com/dmitryAgli) |
| 📧 **E-mail** | [dmitry.agli@gmail.com](mailto:dmitry.agli@gmail.com) |
| ℹ️ **Address** | [Russia, Saint-Petersburg](https://en.wikipedia.org/wiki/Saint_Petersburg) |


## Some facts about me
- 19 years experiense in oil and gaz industry
- Took part in the implementation of more than 20 IT-projects in various roles
- Invented and developted web site with traffic more than 17000 users per day
- Session musician, playing in rock bands, writing music on keyboards

## Skills
- Requirements management and business analysis 
- HTML5, CSS3/SCSS, Bootstrap 4
- SEO optimisation
- JavaScript (ES6)
- SVG
- D3.js v3
- GreenSock.js
- Node.js + Express.js + Handlebars
- MVC
- MongoDB
- TDD: Mocha.js + Chai.js
- GraphQL/Apollo
- React/Redux/Redux-Saga
- Git 

## Code Examples
[full code you can see on my github](https://github.com/dmitryAgli/mini-bot-MIBO/blob/master/index.js)
~~~
        async function checkConditions(date,sm,sm_data,sm_marker) {
          if (sm_data !== empty_data) {
            const collection = db.collection('markers');
            let markerDoc = await collection.findOne({
              sm: sm_marker
            });
              
            if(!markerDoc) {
              markerDoc = await collection.insertOne({
                sm: sm_marker,
                date: ''
              })
            }

            if (markerDoc.date !== date) {
              markerDoc = await collection.updateOne({
                sm: sm_marker
              },{
                $set: {
                  date: date
                }
              });
              sendMails(date,sm,sm_data);
              res_data = `Email sent: / ${date} / ${sm} / ${sm_data}`;
            } else {
              res_data = "The email is have already sent";
            }
          }
        }
~~~
The code from codewars.com:
~~~
var maxSequence = function(arr){
  let max_so_far = max_ending_here = 0;
    arr.forEach((d)=> {
        max_ending_here = Math.max(0, max_ending_here + d);
        max_so_far = Math.max(max_so_far, max_ending_here);
    })
  return max_so_far;
}
~~~

## Experience
- ### 2009-2019 The Lead Engineer at Surgutneftegas
    -  role: Business analyst, JS Developer
    -  project: Information system "Alfa-Drilling. Version 3 ", 
    -  project: Development of a system for operational monitoring of technological parameters of well drilling
    -  Implementation of an algorithm for automatic recognition of operations while drilling wells
- ### 2019-2021 The Lead Business Analyst at Gazprom-neft
    - Participation in the implementation of more than 20 projects (waterfall, agile) as part of the digital transformation strategy for exploration and resource base development
- ### 2021 - now The Lead System Analyst at Innotech (bank VTB)

## Education
- ### 2009 Tyumen State Oil and Gas University, Tyumen
    - Institute of Cybernetics, Informatics and Communications, Automated control systems of technological processes in the oil and gas industry

## Languages
- #### Russian — Native
- #### English — B1 — Intermediate (certificate)
