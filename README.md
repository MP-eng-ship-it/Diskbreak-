
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pricing Cards</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: -apple-system, BlinkMacSystemFont, sans-serif;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            min-height: 100vh;
            padding: 50px 20px;
        }
        h1 {
            color: white;
            text-align: center;
            margin-bottom: 50px;
            font-size: 36px;
        }

        .pricing-container {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
            max-width: 1000px;
            margin: 0 auto;
        }

        .pricing-card {
            background: white;
            border-radius: 20px;
            padding: 40px 30px;
            width: 300px;
            text-align: center;
            position: relative;
            transition: transform 0.3s;
        }
        .pricing-card:hover {
            transform: translateY(-10px);
        }

        .pricing-card.featured {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            transform: scale(1.05);
        }
        .pricing-card.featured:hover {
            transform: scale(1.05) translateY(-10px);
        }

        .badge {
            position: absolute;
            top: -12px;
            left: 50%;
            transform: translateX(-50%);
            background: #FF9500;
            color: white;
            padding: 5px 20px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
        }

        .plan-name {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 10px;
        }
        .pricing-card:not(.featured) .plan-name { color: #333; }

        .price {
            font-size: 48px;
            font-weight: 800;
            margin: 20px 0;
        }
        .pricing-card:not(.featured) .price { color: #667eea; }
        .price span {
            font-size: 16px;
            font-weight: 400;
            opacity: 0.7;
        }

        .features {
            list-style: none;
            margin: 30px 0;
            text-align: left;
        }
        .features li {
            padding: 10px 0;
            border-bottom: 1px solid rgba(0,0,0,0.1);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .pricing-card.featured .features li {
            border-color: rgba(255,255,255,0.2);
        }
        .features li:last-child {
            border: none;
        }
        .pricing-card:not(.featured) .features li { color: #666; }

        .check {
            color: #34C759;
            font-weight: bold;
        }
        .pricing-card.featured .check { color: #90EE90; }

        .btn {
            display: block;
            padding: 15px 30px;
            border: none;
            border-radius: 10px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.2s;
            width: 100%;
        }
        .pricing-card:not(.featured) .btn {
            background: #667eea;
            color: white;
        }
        .pricing-card.featured .btn {
            background: white;
            color: #667eea;
        }
        .btn:hover {
            transform: scale(1.02);
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
        }
    </style>
</head>
<body>
    <h1>Choose Your Plan</h1>

    <div class="pricing-container">
        <div class="pricing-card">
            <div class="plan-name">Starter</div>
            <div class="price">$9<span>/mo</span></div>
            <ul class="features">
                <li><span class="check">&#10003;</span> 5 Projects</li>
                <li><span class="check">&#10003;</span> 10GB Storage</li>
                <li><span class="check">&#10003;</span> Basic Support</li>
                <li><span class="check">&#10003;</span> API Access</li>
            </ul>
            <button class="btn">Get Started</button>
        </div>

        <div class="pricing-card featured">
            <div class="badge">POPULAR</div>
            <div class="plan-name">Professional</div>
            <div class="price">$29<span>/mo</span></div>
            <ul class="features">
                <li><span class="check">&#10003;</span> Unlimited Projects</li>
                <li><span class="check">&#10003;</span> 100GB Storage</li>
                <li><span class="check">&#10003;</span> Priority Support</li>
                <li><span class="check">&#10003;</span> Advanced Analytics</li>
            </ul>
            <button class="btn">Get Started</button>
        </div>

        <div class="pricing-card">
            <div class="plan-name">Enterprise</div>
            <div class="price">$99<span>/mo</span></div>
            <ul class="features">
                <li><span class="check">&#10003;</span> Unlimited Everything</li>
                <li><span class="check">&#10003;</span> 1TB Storage</li>
                <li><span class="check">&#10003;</span> 24/7 Support</li>
                <li><span class="check">&#10003;</span> Custom Integrations</li>
            </ul>
            <button class="btn">Contact Sales</button>
        </div>
    </div>
</body>
<img width="1024" height="1024" alt="A21680E9-2429-4B75-ABD2-04EC7FB01F01" src="https://github.com/user-attachments/assets/42c236cc-3121-4864-968e-5cefe5c370cb" />
