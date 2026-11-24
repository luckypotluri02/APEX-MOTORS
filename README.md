# APEX-MOTORS
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>APEX MOTORS — Drive beyond</title>
    <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Space+Grotesk:wght@500;600;700&display=swap" rel="stylesheet">
    <style>
        * { box-sizing: border-box; }
        html { scroll-behavior: smooth; }
        body { margin: 0; background: #101216; color: #f4f5f7; font-family: 'DM Sans', sans-serif; }
        a { text-decoration: none; color: inherit; }
        
        .nav { height: 78px; padding: 0 7%; display: flex; align-items: center; justify-content: space-between; background: #101216; position: sticky; top: 0; z-index: 5; border-bottom: 1px solid #292d34; }
        .logo { font: 700 25px 'Space Grotesk', sans-serif; letter-spacing: 3px; }
        .logo span { color: #e4a64f; }
        .links { display: flex; gap: 28px; color: #b8bbc2; font-size: 13px; }
        .links a:hover { color: #e4a64f; }
        
        .btn { display: inline-block; background: #e4a64f; color: #151515; font-weight: 800; padding: 13px 20px; border-radius: 3px; font-size: 12px; letter-spacing: .5px; }
        
        .hero { min-height: 590px; display: flex; align-items: center; padding: 70px 7%; background: linear-gradient(90deg,#0d1015 0%,#0d1015e8 35%,#0d101540 100%), url('https://images.unsplash.com/photo-1503376780353-7e6692767b70?auto=format&fit=crop&w=1800&q=90') center/cover; }
        .hero small { color: #e4a64f; letter-spacing: 3px; font-weight: 800; }
        .hero h1 { font: 700 clamp(48px, 6vw, 78px)/.98 'Space Grotesk', sans-serif; max-width: 650px; margin: 18px 0; }
        .hero p { color: #c1c4ca; max-width: 460px; line-height: 1.8; }
        .hero .btn { margin-top: 18px; }
        
        .stats { display: grid; grid-template-columns: repeat(3, 1fr); background: #191d23; padding: 28px 7%; gap: 20px; }
        .stat b { font: 700 25px 'Space Grotesk', sans-serif; color: #e4a64f; }
        .stat span { display: block; color: #999fa8; font-size: 12px; margin-top: 5px; }
        
        .section { padding: 85px 7%; }
        .eyebrow { color: #e4a64f; font-size: 11px; letter-spacing: 3px; font-weight: 800; }
        .section h2 { font: 700 40px 'Space Grotesk', sans-serif; margin: 12px 0; }
        .intro { color: #a9adb5; line-height: 1.7; }
        
        .cars { display: grid; grid-template-columns: repeat(3, 1fr); gap: 20px; margin-top: 38px; }
        .car { background: #191d23; border: 1px solid #2a3039; border-radius: 6px; overflow: hidden; }
        .car img { width: 100%; height: 210px; object-fit: cover; }
        .carbody { padding: 20px; }
        .carhead { display: flex; justify-content: space-between; gap: 10px; align-items: center; }
        .car h3 { font: 600 20px 'Space Grotesk', sans-serif; margin: 0; }
        .price { color: #e4a64f; font-weight: 700; font-size: 14px; }
        .car p { color: #a9adb5; font-size: 13px; line-height: 1.6; }
        .specs { display: flex; gap: 16px; border-top: 1px solid #303640; padding-top: 14px; margin-top: 15px; color: #d2d4d9; font-size: 11px; flex-wrap: wrap; }
        
        .compare { width: 100%; border-collapse: collapse; margin-top: 28px; background: #191d23; font-size: 13px; }
        .compare th, .compare td { padding: 16px; text-align: left; border-bottom: 1px solid #303640; }
        .compare th { color: #e4a64f; font-weight: 700; }
        .compare td { color: #c6c9cf; }
        
        .test { background: linear-gradient(120deg, #1e252d, #14181e); display: grid; grid-template-columns: 1fr 1fr; gap: 50px; align-items: center; }
        .test img { width: 100%; height: 350px; object-fit: cover; border-radius: 5px; }
        .form { display: grid; gap: 12px; margin-top: 22px; }
        .form input, .form select { width: 100%; padding: 14px; background: #101419; border: 1px solid #3a414b; color: #fff; border-radius: 3px; }
        .form button { border: 0; cursor: pointer; }
        
        .note { font-size: 12px; color: #9ca2ac; margin-top: 12px; }
        
        .footer { padding: 35px 7%; background: #0a0c0f; color: #9ca2ac; display: flex; justify-content: space-between; gap: 20px; flex-wrap: wrap; font-size: 13px; }
        .footer b { color: #fff; }
        
        @media(max-width: 850px) {
            .cars { grid-template-columns: 1fr 1fr; }
            .test { grid-template-columns: 1fr; }
            .links { gap: 14px; }
        }
        @media(max-width: 560px) {
            .links { display: none; }
            .hero { min-height: 540px; }
            .stats { grid-template-columns: 1fr 1fr; }
            .cars { grid-template-columns: 1fr; }
            .section { padding: 65px 6%; }
            .section h2 { font-size: 33px; }
            .compare { font-size: 11px; }
            .compare th, .compare td { padding: 10px; }
            .nav { padding: 0 6%; }
        }
    </style>
</head>
<body>

    <nav class="nav">
        <a class="logo" href="#">APEX<span>.</span></a>
        <div class="links">
            <a href="#models">Models</a>
            <a href="#performance">Performance</a>
            <a href="#compare">Compare</a>
            <a href="#test">Test drive</a>
        </div>
        <a class="btn" href="#test">BOOK A TEST DRIVE</a>
    </nav>

    <header class="hero">
        <div>
            <small>ENGINEERED TO INSPIRE</small>
            <h1>Own the road.<br>Define the drive.</h1>
            <p>Discover a collection of performance, design and everyday refinement. Find the Apex that feels like you.</p>
            <a class="btn" href="#models">EXPLORE THE RANGE ↗</a>
        </div>
    </header>

    <div class="stats">
        <div class="stat"><b>3.8 sec</b><span>0–100 km/h · featured performance model</span></div>
        <div class="stat"><b>620 km</b><span>Up to claimed range · electric concept</span></div>
        <div class="stat"><b>24/7</b><span>Connected ownership support</span></div>
    </div>

    <section class="section" id="models">
        <div class="eyebrow">THE COLLECTION</div>
        <h2>Find your perfect machine.</h2>
        <p class="intro">From agile city drives to grand touring comfort, explore the lineup.</p>
        
        <div class="cars">
            <article class="car">
                <img src="https://images.unsplash.com/photo-1503376780353-7e6692767b70?auto=format&fit=crop&w=900&q=85" alt="Silver sports coupe">
                <div class="carbody">
                    <div class="carhead">
                        <h3>Apex GT</h3>
                        <span class="price">₹78.5 Lakh*</span>
                    </div>
                    <p>A confident grand tourer with sculpted lines and responsive power.</p>
                    <div class="specs">
                        <span>⚡ 3.8s 0–100</span>
                        <span>◉ 2.9L Turbo</span>
                        <span>✦ 2 Seats</span>
                    </div>
                </div>
            </article>

            <article class="car">
                <img src="https://images.unsplash.com/photo-1519641471654-76ce0107ad1b?auto=format&fit=crop&w=900&q=85" alt="Premium SUV on road">
                <div class="carbody">
                    <div class="carhead">
                        <h3>Apex Terra</h3>
                        <span class="price">₹52.9 Lakh*</span>
                    </div>
                    <p>Versatile space, elevated comfort and capability for every journey.</p>
                    <div class="specs">
                        <span>⚡ 6.4s 0–100</span>
                        <span>◉ AWD</span>
                        <span>✦ 5 Seats</span>
                    </div>
                </div>
            </article>

            <article class="car">
                <img src="https://images.unsplash.com/photo-1593941707882-a5bba14938c7?auto=format&fit=crop&w=900&q=85" alt="Modern electric vehicle">
                <div class="carbody">
                    <div class="carhead">
                        <h3>Apex Eon</h3>
                        <span class="price">₹41.2 Lakh*</span>
                    </div>
                    <p>Quiet electric confidence, intuitive technology and a clean design.</p>
                    <div class="specs">
                        <span>⚡ 4.9s 0–100</span>
                        <span>◉ EV</span>
                        <span>✦ 5 Seats</span>
                    </div>
                </div>
            </article>
        </div>
        <p class="note">*Illustrative concept pricing for this student website project. Not an actual offer.</p>
    </section>

    <section class="section" id="performance" style="background:#171b21">
        <div class="eyebrow">BUILT AROUND THE DRIVER</div>
        <h2>Every detail has a purpose.</h2>
        <p class="intro">Driver-focused interiors, intelligent assistance and considered engineering come together for a more connected drive.</p>
    </section>

    <section class="section" id="compare">
        <div class="eyebrow">AT A GLANCE</div>
        <h2>Compare the lineup.</h2>
        <table class="compare">
            <thead>
                <tr>
                    <th>Model</th>
                    <th>Body style</th>
                    <th>Powertrain</th>
                    <th>Starting price*</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Apex GT</td>
                    <td>Coupe</td>
                    <td>Turbo petrol</td>
                    <td>₹78.5 Lakh</td>
                </tr>
                <tr>
                    <td>Apex Terra</td>
                    <td>SUV</td>
                    <td>Petrol / AWD</td>
                    <td>₹52.9 Lakh</td>
                </tr>
                <tr>
                    <td>Apex Eon</td>
                    <td>Electric sedan</td>
                    <td>Electric</td>
                    <td>₹41.2 Lakh</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section class="section test" id="test">
        <div>
            <div class="eyebrow">YOUR NEXT CHAPTER STARTS HERE</div>
            <h2>Take the wheel.</h2>
            <p class="intro">Book a test drive and experience the lineup with our team. Submit the form and we'll be in touch.</p>
            
            <form class="form" onsubmit="event.preventDefault();document.getElementById('msg').textContent='Thank you! Your demo request has been recorded.';">
                <input required placeholder="Your name" aria-label="Your name">
                <input type="email" required placeholder="Email address" aria-label="Email address">
                <select aria-label="Choose a model">
                    <option>Choose a model</option>
                    <option>Apex GT</option>
                    <option>Apex Terra</option>
                    <option>Apex Eon</option>
                </select>
                <button class="btn" type="submit">REQUEST A TEST DRIVE</button>
            </form>
            <p class="note" id="msg">Demo form only — no information is sent to a server.</p>
        </div>
        <img src="https://images.unsplash.com/photo-1492144534655-ae79c964c9d7?auto=format&fit=crop&w=1100&q=85" alt="Luxury car detail">
    </section>

    <footer class="footer">
        <div>
            <b class="logo">APEX<span>.</span> MOTORS</b>
            <p>Drive beyond the expected.</p>
        </div>
        <div>
            Vijayawada · Andhra Pradesh<br>
            hello@apexmotors.example<br>
            <span style="color:#e4a64f">Student project concept website</span>
        </div>
    </footer>

</body>
</html>
```[cite: 1]
