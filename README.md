<!DOCTYPE html>
<html lang="en">
<meta charset="UTF-8">

<script type="text/javascript" src="https://www.geogebra.org/apps/deployggb.js"></script>

<head>
    <title>Elvar's webpage</title>
    <style>
        * {
            margin: 0;
            padding: 0;
        }

        body {
            background: rgb(0,206,209);
        }

        .container {
            border: 1px solid grey;
            margin: 2rem;
		background:white
        }

        [data-tab-info] {
            display: none;
        }

        .active[data-tab-info] {
            display: block;
        }

        .tab-content {
            margin-top: 1rem;
	    margin-bottom:1rem;
            padding-left: 1rem;
	    padding-right: 1rem;
            font-size: 20px;
            font-family: Times new roman, serif;
            
        }

        .tabs {
            border-bottom: 1px solid grey;
            background-color: white;
            font-size: 25px;
            color: black;
            display: flex;
            margin: 0;
	font-family:Times new Roman, serif;
        }

        .tabs span {
            background: rgb(0,206,209);
            padding: 15px;
            border: 1px solid grey;
        }

        .tabs span:hover {
            background: rgb(0,139,139);
            cursor: pointer;
            color: black;
        }
	h1, h2, h3, h4, h5, h6{
  		margin-top:20px;
  		margin-bottom:10px;
}
	h1{
		text-align:center;
		font-family:Optima,serif;
	}
    </style>
</head>

<body>
	<h1>Elvar Wang Atlason</h1>
    <!-- Body Container -->
    <div class="container">

        <!-- Tabs Detail -->
        <div class="tabs">
            <span data-tab-value="#tab_1">About me</span>
            <span data-tab-value="#tab_2">Flexible polyhedra</span>
        </div>

        <!-- Tab content -->
        <div class="tab-content">
            <div class="tabs__tab active" id="tab_1" data-tab-info>
<p>I am a PhD student at University College London studying differential geometry. My supervisor is <a href="https://www.homepages.ucl.ac.uk/~ucahoan/" style="color: blue">Aleksander Doan</a>.  <br>
Before that, I studied mathematics at the University of Cambridge.<br>

I grew up in Reykjavík, Iceland. My mum is Faroese, and my middle name Wang is her surname. The similarity to the common Chinese surname is a coincidence. My last name means Atli's son.
</p>




<img src="EWA-profile-picture.png" alt="(Iceland, 2019)" height="250" border="0">


<a target="_blank" href="http://projecteuler.net">
	    <img src="https://projecteuler.net/profile/elvar.png" alt="my Project Euler profile" >
</a>

<h2> Research </h2>

<p>I study the interplay between analysis and geometry. Recently, I have been working on ideas related to the Fueter equation and Floer homology.<br>

I have also studied flexible polyhedra, where I have used symmetric quadrilaterals to construct new examples. See the tab above for some of the models I have constructed.



<h2> Teaching </h2>

<p>I lecture <a href = "https://www.ucl.ac.uk/mathematical-physical-sciences/sites/mathematical_physical_sciences/files/math0039.pdf" style = "color:blue"> MATH0039</a> at UCL alongside Teymour Gray. This is an ancillary course on differentiation and integration. We also lectured the course in 2024.<br>

In Michaelmas term of 2024, I taught Icelandic at the University of Cambridge for the <a href = "https://www.asnc.cam.ac.uk/currentstudents/icelandic/index.htm" style = "color:blue"> Anglo-Saxon, Norse and Celtic department</a>.<br>

I teach the problem solving classes at UCL, and prepare the team for the International Mathematics Competition for University students, <a href = "https://www.imc-math.org.uk/" style = "color:blue">IMC</a>.<br> I also take part in the training of the Icelandic team for the International Maths Olympiad, <a href = "https://www.imo-official.org/" style = "color:blue">IMO</a>, and have served as the deputy leader for Iceland.

</p>





            </div>
            <div class="tabs__tab" id="tab_2" data-tab-info>



<p> If you make a paper model of a convex polyhedron, it will not flex, despite the fact that every edge functions as a hinge. By counting the degrees of freedom, polyhedra can be seen to be generically rigid. However, under certain symmetry conditions, polyhedra can be made to flex.

<h2> A flexible dodecahedron</h2>
Below is an example of a flexible polyhedron with 12 faces, discovered by me in the summer of 2025. It is the simplest possible flexible polyhedron by number of faces. For an explanation, see <a href = "https://arxiv.org/pdf/2510.06897" style = "color:blue"> my paper</a>.<br>
The model below is made using geogebra, and is completely interactive.
</p>




<div id="ggb-element"></div>




<script>
    var dodecahedron = {"material_id":"pb4nqczx", "appName": "3d", "width": 1400, "height": 1400, "showToolBar": false, "showAlgebraInput": false, "showMenuBar": false, scale:0.4, enableRightClick:false};
    var applet = new GGBApplet(dodecahedron, true);
    window.addEventListener("load", function() {
        applet.inject('ggb-element');
    });
</script>

<p>
If you want an even more interactive model, you can make the flexible dodecahedron out of paper using the net below. Gluing instructions are given by labels on the edges. Mountain folds are solid and valley folds are dashed.
</p>

<img src="Flexible_dodecahedron_net.png" alt="(A net for a flexible dodecahedron)" width=100% border="0">


<h2>The Foxtrot</h2>
<p>
This polyhedrom relies on a method called twinning to construct new flexible components (crinkles). See <a href = "https://arxiv.org/pdf/2510.05280" style = "color:blue"> here</a> for a paper by myself and <a href = "https://www3.eng.cam.ac.uk/~sdg/" style = "color:blue">Simon D. Guest</a> on the topic. That paper also discusses the history and relevant background.
</p>
<div id="ggb-foxtrot"></div>

<script>
    var foxtrot = {"material_id":"fq3vdnmy", "appName": "3d", "width": 700, "height": 700, "showToolBar": false, "showAlgebraInput": false, "showMenuBar": false, scale:0.8, enableRightClick:false };
    var applet2 = new GGBApplet(foxtrot, true);
    window.addEventListener("load", function() {
        applet2.inject('ggb-foxtrot');
    });
</script>


            </div>
        </div>
    </div>
    <script type="text/javascript">

        // function to get each tab details
        const tabs = document.querySelectorAll('[data-tab-value]')
        const tabInfos = document.querySelectorAll('[data-tab-info]')

        tabs.forEach(tab => {
            tab.addEventListener('click', () => {
                const target = document
                    .querySelector(tab.dataset.tabValue);
                tabInfos.forEach(tabInfo => {
                    tabInfo.classList.remove('active')
                })
                target.classList.add('active');
            })
        })
    </script>
</body>

<foot>


<p>
<center>
Elvar Wang Atlason<br>

Email: Elvar (d o t) Atlason (d o t) 23 (a t) ucl (d o t) ac (d o t) uk</center>
<br></p>

</foot>

</html>
