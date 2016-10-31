Notes:

Make all changes in a text editor like Sublime Text and then copy them into RightOnInteractive.
ROI will frequently drop tags entirely or default them to a different tag, especially if you edit it in ROI directly.


In the Quote section of apprentice profiles, avoid using contractions. The apostrophe reads as an unclosed element that can break the page.
_________________________________

1. To add a new track, add a | filter:search.Java | or whatever to the ng-repeat under the container-box class, line 202, like so:


<div ng-repeat="apprentice in apprentices | orderBy:propertyName:reverse | filter:search.JS | filter:search.Net | filter:search.Java |filter:search.Relocate">

2. Add a new checkbox div class to the filter span, line 180:

<div class="checkbox">
    <label>
        <input type="checkbox" value="" ng-model="search.Java" ng-true-value="'JavaMember'" ng-false-value="">
        Java
    </label>
</div>

3. Change the template:

Below badges:

Class: '.Java',
JavaString: "MemberofJava",



(template of Java Student below)





_________________________________
Template of .NET student,

Gold / Red / Purple Badge,
knows C# and PHP,
willing to relocate
_________________________________

{
    FirstName: 'Bob',
    LastName: 'Ross',
    Info: 'Bob is a .NET student who has a lot of potential.',
    Quote: '“Bob is a genius.” - Tiffany Trusty, Eleven Fifty Director of Apprenticeship',
    Relocate: 'No',
    Photo: 'https://d39a28rhl1iwx3.cloudfront.net/dy/fred_miles_500px.jpg',
    Languages: ['C#','PHP'],
    Links: [{
        Link: 'https://www.linkedin.com/in/bob-ross',
        Site: 'LinkedIn',
        Icon: 'fa fa-linkedin-square fa-3x linkedinpush'
    }, {
        Link: 'http://bob-ross.github.io/',
        Site: 'Portfolio',
        Icon: 'fa fa-desktop fa-3x info-icon'
    }, {
        Link: 'http://www.slideshare.net/bob-ross/bob-rossresumedocx',
        Site: 'Resume',
        Icon: 'fa fa-file-text fa-3x info-icon'
    }],
    Badge: [{
        Img:'https://d39a28rhl1iwx3.cloudfront.net/dy/gold-01.png',
        Title: 'Gold Badge Proficient',
        Class: "gold-badge"
      },{
        Img:'https://d39a28rhl1iwx3.cloudfront.net/dy/red-01.png',
        Title: 'Red Badge Proficient',
        Class: "red-badge"
      },{
          Img:'https://d39a28rhl1iwx3.cloudfront.net/dy/purple-01.png',
          Title: 'Purple Badge Proficient',
          Class: "purple-badge"
        }],
    Class: '.NET',
    JSString: "MemberofNet",
    RelocateString: "TotallyWillingToRelocate",
    ReloStyle: 'fa fa-plane fa-rotate-90 pull-right'
},


_________________________________
Template of JavaScript student,

Gold / Red Badge,
knows JavaScript,
NOT willing to relocate
_________________________________



{   FirstName: 'Frida',
    LastName:'Kahlo',
    Info: 'Frida is a great front-end developer. ',
    Quote: '“Frida is going to be a star.” - James Handshoe, Eleven Fifty Instructor ',
    Relocate: 'No',
    Photo: 'https://d39a28rhl1iwx3.cloudfront.net/dy/frida_kahlo_500px.jpg',
    Languages: ['JavaScript'],
    Links: [{
        Link: 'https://www.linkedin.com/in/frida-kahlo',
        Site: 'LinkedIn',
        Icon: 'fa fa-linkedin-square fa-3x linkedinpush'
    }, {
        Link: 'https://frida-kahlo.github.io/',
        Site: 'Portfolio',
        Icon: 'fa fa-desktop fa-3x info-icon'
    }, {
        Link: 'https://docs.google.com/document/frida-kahlo-resume/',
        Site: 'Resume',
        Icon: 'fa fa-file-text fa-3x info-icon'

    }],
    Badge: [{
        Img:'https://d39a28rhl1iwx3.cloudfront.net/dy/gold-01.png',
        Title: 'Gold Badge Proficient',
        Class: "gold-badge"
      },{
        Img:'https://d39a28rhl1iwx3.cloudfront.net/dy/red-01.png',
        Title: 'Red Badge Proficient',
        Class: "red-badge"
      }],
    Class: '.JS',
    JSString: "MemberofJS",
    ReloStyle: ''
},

_________________________________
Template of JavaScript student,

Gold Badge,
knows Java,
NOT willing to relocate
_________________________________

{   FirstName: 'Louise',
    LastName:'Bourgeoise',
    Info: 'Louise has a passion for structure. ',
    Quote: '“I hate spiders.” - Paul O'Connor, Eleven Fifty Instructor ',
    Relocate: 'No',
    Photo: 'https://d39a28rhl1iwx3.cloudfront.net/dy/louise_bourgeoise_500px.jpg',
    Languages: ['Java'],
    Links: [{
        Link: 'https://www.linkedin.com/in/louise-bourgeoise,
        Site: 'LinkedIn',
        Icon: 'fa fa-linkedin-square fa-3x linkedinpush'
    }, {
        Link: 'https://louise-bourgeoise.github.io/',
        Site: 'Portfolio',
        Icon: 'fa fa-desktop fa-3x info-icon'
    }, {
        Link: 'https://docs.google.com/document/louise-bourgeoise-resume/',
        Site: 'Resume',
        Icon: 'fa fa-file-text fa-3x info-icon'

    }],
    Badge: [{
        Img:'https://d39a28rhl1iwx3.cloudfront.net/dy/gold-01.png',
        Title: 'Gold Badge Proficient',
        Class: "gold-badge"
      }],
    Class: 'Java',
    JavaString: "MemberofJava",
    ReloStyle: ''
},
