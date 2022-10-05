Humam

- 🔭 Currently working on https://www.theodinproject.com

- 🌱 Currently learning Front-End Programming

- 📫 Contact me on: hu666mam@gmail.com


<html>
<head>
    <style> * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family:'Karla', sans-serif;
    background: #fafafa;
}

.container {
    width: 650px;
    height: 300px;
    display: flex;
    justify-content: space-around;
    align-items: flex-start;
    background-color: #F5F5F5;
}

.left-side {
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    flex: 1;
}

.name {
    font-family: 'Karla';
    font-weight: 800;
    font-size: 30px;
    color: #121212;
}
.description {
    font-size: 25px;
    font-family: 'Karla';
    font-weight: 800;
    color: #30475E;
}
.age {
    font-family: 'Inter';
    font-weight: 400;
    font-size: 18px;
    color: #121212;
}

.line {
    width: 100%;
    height: 2px;
    background-color: #30475E;
    margin: 15px 0;
}
.bottom-section {
    color: #F05454;
    font-style: normal;
    font-weight: 600;
    font-size: 18px;
    line-height: 25px;
}
.right-side {
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    flex: 3;
    margin: 20px;
}

.profil {
    height: 150px;
    width: 150px;
    margin: 20px;

}

.social-media {
    display: flex;
    justify-content: center;
    gap: 10px;
}
</style>
</head>
<body>
    <div class="container">
        <div class="left-side">
            <img class="profil" src="images/profil.jpg">
            <div class="social-media">
                <img class="social-media-icon" src="images/github-icon.png"/>
                <img  src="images/linkdin-icon.png"/>
                <img  src="images/ig-icon.png"/>
                <img  src="images/twitter-icon.png"/>
            </div>
        </div>
        <div class="right-side">
            <div class="top-section">
                <p class="name">Empty</p>
                <p class="description">Empty</p>
                <p class="age">Empty</p>
            </div>
            <div class="line"></div>
            <div class="bottom-section">
                <div class="gmail"> Gmail: Empty </div>
                <div class="phone"> Phone: Empty</div>
            </div>
        </div>
    </div>
    <script>
    let info = {
    firstName: "Humam",
    secondName: "Kharbouch",
    description: "Front-End Developer",
    ageEl: "22",
    gmail: "huumaminho@gmail.com",
    phone: "0639013151",
}

let nameEl = document.querySelector(".name")
let descriptionEl = document.querySelector(".description")
let ageEl = document.querySelector(".age")
let gmailEl = document.querySelector(".gmail")
let phoneEl = document.querySelector(".phone")

nameEl.textContent = (info.firstName) + " " + (info. secondName) ;
descriptionEl.textContent = (info.description) ;
ageEl.textContent = (info.ageEl) + " years old" ;
gmailEl.textContent = (info.gmail) ;
phoneEl.textContent = (info.phone) ;

 let parentEl = document.querySelector(".social-media-icon").parentElement;
 let imgEl = parentEl.innerHtml;
 parentEl.innerHtml = '<a href="https://github.com/Humaminho">' + imgEl + '</a>';

// (".social-media-icon").wrap("<a href='https://github.com/Humaminho'></a>")
</script>
</body>
</html>
