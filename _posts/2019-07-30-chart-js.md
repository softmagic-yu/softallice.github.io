---
layout: post
title:  "Accumulated experience of social living"
author: sal
categories: [ Jekyll, tutorial ]
image: assets/images/ilsan/4.jpg
---
The die cut has also been employed in the non-juvenile sphere as well, a recent example being Jonathan Safran Foer’s ambitious Tree of Codes. 

As for this particular rendition of Charles Perrault’s classic tale, the text and design is by Lydia Very (1823-1901), sister of Transcendentalist poet Jones Very. The gruesome ending of the original - which sees Little Red Riding Hood being gobbled up as well as her grandmother - is avoided here, the gore giving way to the less bloody aims of the morality tale, and the lesson that one should not disobey one’s mother.

The first mass-produced book to deviate from a rectilinear format, at least in the United States, is thought to be this 1863 edition of Red Riding Hood, cut into the shape of the protagonist herself with the troublesome wolf curled at her feet. Produced by the Boston-based publisher Louis Prang, this is the first in their “Doll Series”, a set of five “die-cut” books, known also as shape books — the other titles being Robinson Crusoe, Goody Two-Shoes (also written by Red Riding Hood author Lydia Very), Cinderella, and King Winter. 

An 1868 Prang catalogue would later claim that such “books in the shape of a regular paper Doll... originated with us”. 

> It would seem the claim could also extend to die cut books in general, as we can’t find anything sooner, but do let us know in the comments if you have further light to shed on this! Such books are, of course, still popular in children’s publishing today, though the die cutting is not now limited to mere outlines, as evidenced in a beautiful 2014 version of the same Little Red Riding Hood story. 


<div style="width:100%;">
<canvas id="radar-chart" width="600" height="800"></canvas>
</div>

<script>
    var notations = {
        0:"",
        1:"no",
        20:"Theory",
        50:"proficient",
        70:"Great",
        90:"outstanding",
            }

    new Chart(document.getElementById("radar-chart"), {
        type: 'radar',
        
        data: {
            labels: ["GNU/Linux", "Android Development", "Core Java", "Frontend HTML/CSS", "UI / UX", "Blogging", "Database", "Javascript", "Windows", "CMS(Wordpress)"],
            datasets: [{
                label: "2017",
                fill: true,
                backgroundColor: "rgba(51,133,255,0.2)",
                borderColor: "rgba(51,133,255,1)",
                pointBorderColor: "#fff",
                pointBackgroundColor: "rgba(51,133,255,1)",
                data: [33, 49, 50, 67, 39, 80, 60, 50, 90,80]
            }, {
                label: "2018",
                fill: true,
                backgroundColor: "rgba(255,99,132,0.2)",
                borderColor: "rgba(255,99,132,1)",
                pointBorderColor: "#fff",
                pointBackgroundColor: "rgba(255,99,132,1)",
                pointBorderColor: "#fff",
                data: [60, 67, 80, 68, 50, 90, 80, 60, 90,81]
            }]
        },


        options: {
            scale: {
                responsive: true,
                ticks: {
                    display: true,
                    min:0,
                    beginAtZero: true,
                    max: 100, 
                    userCallback: function (value, index, values) {
                        if( typeof notations[value]!="undefined")
                        {
                             return notations[value];
                         }
                    else {
                      return value;
                           }

                },
                },

                gridLines: {
                    display: true,
                    color: [
                        "rgba(245, 245,220,1)",
                        "rgba(0, 0,255,0.1)",
                        "rgba(165, 42,42,0.1)",
                        "rgba(0, 255,255,0.1)",
                        "rgba(0, 0,139,0.3)",
                        "rgba(0, 139,139,0.1)",
                        "rgba(169, 169,169,1)",
                        "rgba(0, 100,0,0.1)",
                        "rgba(189, 22,107,0.1)",
                        "rgba(139, 0,139,0.1)",
                        "rgba(139, 0,139,0.1)",
                        "rgba(139, 0,139,0.1)",


                    ], 
                },

                angleLines: {
                    display: true,
                    color: "red",
                },
                pointLabels: {
                    // callback: function(value, index, values) {
                    //     return '$' + value;
                    // }
                    fontColor: '#' + Math.random().toString(16).slice(2, 8).toUpperCase(),
                },
            },
            legend: {
                display: true
            },
            title: {
                display: false,
                // text: 'Skill Set'
            },
        }
    });
</script>