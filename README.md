<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shine</title>
    <style>
        :root{
            --bg1: #0b8f5a;
            --bg2: #cfffe3;
            --accent1: #60e3a2;
            --accent2: #2ee6a9;
            --card-bg: rgba(255,255,255,0.92);
            --glass: rgba(255,255,255,0.12);
            --text: #053825;
        }
        body{
            margin:0;
            font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
            color:var(--text);
            background: linear-gradient(135deg, #e6fff5 0%, #d4fbe6 45%, #bff3d3 100%);
            min-height:100vh;
            -webkit-font-smoothing:antialiased;
            -moz-osx-font-smoothing:grayscale;
        }

        header{
            display:flex;
            align-items:center;
            justify-content:space-between;
            padding:18px 28px;
            backdrop-filter: blur(6px);
            background: linear-gradient(180deg, rgba(255,255,255,0.12), rgba(255,255,255,0.04));
        }
        .brand{
            display:flex;
            gap:12px;
            align-items:center;
        }
        .logo{
            width:46px;
            height:46px;
            border-radius:2px;
            box-shadow: 0 6px 3px rgba(0,0,0,0.08);
            display:flex;
            align-items:center;
            justify-content:center;
            font-weight:700;
            color:#053825;
            font-size:18px;
        }
        nav a{
            margin-left:14px;
            text-decoration:none;
            color: rgba(5,56,37,0.9);
            font-weight:600;
        }
        .container{
            max-width:1100px;
            margin:36px auto;
            padding:32px;
        }

        .hero{
            display:flex;
            gap:28px;
            align-items:center;
            background: linear-gradient(135deg, rgba(255,255,255,0.36), rgba(255,255,255,0.06));
            border-radius:18px;
            padding:28px;
            box-shadow: 0 10px 30px rgba(5,56,37,0.06);
            flex-wrap:wrap;
        }
        .hero .text{
            flex:1 1 360px;
        }
        .hero h1{
            margin:0 0 12px 0;
            font-size:clamp(28px, 4vw, 48px);
            line-height:1.05;
            color:#043826;
        }
        .hero p{
            margin:0 0 18px 0;
            color:rgba(4,56,38,0.8);
            font-size:16px;
        }
        .cta{
            display:inline-flex;
            gap:12px;
        }
        .btn{
            padding:10px 18px;
            border-radius:12px;
            border:0;
            cursor:pointer;
            font-weight:700;
            box-shadow: 0 8px 20px rgba(0,0,0,0.06);
            transition:transform .18s ease, box-shadow .18s ease;
        }
        .btn.primary{
            background: linear-gradient(90deg,var(--accent2),var(--accent1));
            color:#063422;
        }
        .btn.ghost{
            background: transparent;
            color: #053825;
            border:1px solid rgba(5,56,37,0.08);
        }
        .btn:active{ transform:translateY(1px) }

        .hero .visual{
            flex:0 1 320px;
            border-radius:14px;
            padding:14px;
            background: linear-gradient(180deg, rgba(255,255,255,0.28), rgba(255,255,255,0.06));
        }
        .cards{
            display:grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap:18px;
            margin-top:22px;
        }
        .card{
            background: var(--card-bg);
            padding:18px;
            border-radius:12px;
            box-shadow: 0 6px 18px rgba(5,56,37,0.04);
            transition: transform .18s ease, box-shadow .18s ease;
        }
         .songs{
            background: var(--card-bg);
            padding:18px;
            border-radius:12px;
            box-shadow: 0 6px 18px rgba(5,56,37,0.04);
            transition: transform .18s ease, box-shadow .18s ease;
        }
         .songs:hover{
            transform:translateY(-6px);
            box-shadow: 0 18px 40px rgba(5,56,37,0.08);
        }
        .card:hover{
            transform:translateY(-6px);
            box-shadow: 0 18px 40px rgba(5,56,37,0.08);
        }
        .card h3{ margin:0 0 8px 0; }
        .grid-row{
            display:grid;
            grid-template-columns: 1fr 1fr;
            gap:12px;
            margin-top:18px;
        }
        footer{
            margin-top:28px;
            text-align:center;
            padding:24px;
            color: rgba(5,56,37,0.7);
            font-size:14px;
        }

        /* responsive */
        @media (max-width:640px){
            header{ padding:12px 16px }
            .container{ padding:18px }
        }
    </style>
</head>
<body>
    <header>
        <div class="brand">
            <div class="logo"><img src="Black cat.jpg" alt="" width="46px"></div>
            <div>
                <div style="font-weight:800">Shine</div>
                <div style="font-size:12px;color:rgba(5,56,37,0.6)"></div>
            </div>
        </div>
        <nav aria-label="Main">
            <a href="#features">Cats</a>
            <a href="#examples">About me</a>
            <a href="#contact">contact me</a>
        </nav>
    </header>

    <main class="container">
        <section class="hero" aria-labelledby="hero-heading">
            <div class="text">
                <h1 id="hero-heading">Wellcome to my page</h1>
                <p></p>
                <div class="cta">
                   
                </div>

                <div class="cards" id="features" style="margin-top:22px">
                    <div class="card">
                        <h3>Cats</h3>
                        <img src="eb84eeb4-c5d3-40bf-bb18-8f610c046075.jpg" alt="cat_1" width="75px"> 
                        <img src="0185e827-9578-4ea0-b682-76a06c7a6c3a.jpg" alt="cat_2" width="100px">
                        <img src="Котенок в костюме акулы.jpg" alt="cat_3" width="100px">
                    </div>
                    <div class="songs" id="features" style="margin-top: 22px">
                    <h3>Favorite song</h3>
                    <iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/track/3xA3MGG3sVpZSsnHXvdYMn?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                    </div>
                </div>
            </div>
        </section>
                    <div class="card">
                        <h3>About me</h3>
                        <p>I'm student from Charlottenlund vgs</p>
                    </div>
                    <div class="card" id="examples">
                        <h3>Facts</h3>
                        <p>I have a cat, his name is Nikas</p>
                    </div>
                </div>
            </div>

        </section>

        

        <section id="contact" style="margin-top:28px">
            <h2 style="margin:0 0 12px 0">Contact me</h2>
            <a href="https://www.instagram.com/nakedbibi/"><img src="Ícone do aplicativo Instagram Logotipo da mídia social Ilustração em vetor _ vetor Premium gerado com IA.jpg" alt="instagram" width="50px"></a>
        </section>

        <footer>
            © Made by Sofiia (snllix)
        </footer>
    </main>

    <script>
        const header = document.querySelector('header');
        window.addEventListener('scroll', () => {
            header.style.boxShadow = window.scrollY > 20 ? '0 8px 30px rgba(5,56,37,0.06)' : 'none';
        });
    </script>
</body>
</html>
