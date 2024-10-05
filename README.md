<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>给小骷髅兵的神秘邀请函</title>
    <style>
        /* 保持原有的样式不变 */
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Noto+Serif+SC:wght@400;700&family=Cormorant+Garamond:ital,wght@1,600&display=swap');
        body {
            font-family: 'Noto Serif SC', serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #fff0f5;
            line-height: 1.8;
        }
        .container {
            background-color: white;
            padding: 50px;
            border-radius: 20px;
            box-shadow: 0 0 30px rgba(255,20,147,0.2);
            max-width: 800px;
            text-align: justify;
            position: relative;
            overflow: hidden;
        }
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: #ff69b4;
            transform: rotate(45deg);
            opacity: 0.6;
        }
        .heart::before,
        .heart::after {
            content: '';
            width: 20px;
            height: 20px;
            background-color: #ff69b4;
            border-radius: 50%;
            position: absolute;
        }
        .heart::before {
            left: -10px;
        }
        .heart::after {
            top: -10px;
        }
        h1 {
            font-family: 'Playfair Display', serif;
            color: #ff1493;
            text-align: center;
            margin-bottom: 30px;
            font-size: 3em;
            letter-spacing: 2px;
        }
        p {
            text-indent: 2em;
            margin-bottom: 20px;
        }
        .signature {
            text-align: right;
            margin-top: 40px;
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.8em;
            color: #ff1493;
            font-weight: 600;
        }
        .border {
            border: 2px solid #ffc0cb;
            border-radius: 15px;
            padding: 20px;
            margin-top: 20px;
        }
        #passwordForm {
            text-align: center;
            margin-bottom: 20px;
        }
        #password {
            padding: 10px;
            font-size: 16px;
            border: 2px solid #ffc0cb;
            border-radius: 5px;
        }
        #submitPassword {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #ff1493;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        #content {
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="heart" style="top: 20px; right: 40px;"></div>
        <div class="heart" style="bottom: 30px; left: 50px;"></div>
        <div class="heart" style="top: 50%; right: 60px;"></div>
        <h1>Sharon宝贝</h1>
        <div id="passwordForm">
            <p>我亲爱的小骷髅兵，请输入我们的特别日子来解锁这封信 (格式：MMDD)</p>
            <input type="password" id="password" placeholder="输入密码">
            <button id="submitPassword">解锁我的心意</button>
        </div>
        <div id="content">
            <div class="border">
                <p>虽然说是情书，但我实在不知从何开始。为了保持情感的真挚，我特意没有借鉴任何网上的告白或是书本上的句子，只是让思绪自由流淌，想到哪里写到哪里。</p>
                
                <p>说好要补的表白，断断续续已经过去了一个月。回想起最初在车上那断断续续的表白，对未来的困惑和对新关系的畏惧，如今已在我们日日夜夜的真心相谈中逐渐消散。在这段关系的"试用期"里，我看到了许多你未曾向他人展现的一面，而我越看越觉得，你的每一秒对我来说都弥足珍贵。不知不觉间，我的生活已离不开你的存在，我后知后觉地意识到，我对你的爱意竟是如此深切。</p>
                
                <p>在写下这封信时，我的脑海中总是浮现出你在角落里微笑着迎接下课的我的样子。我对那微笑深深着迷，却又难以用华丽的辞藻来形容内心的感动。这种不再孤单的感受，比我想象中还要美好许多。</p>
                
                <p>就像我们一起画的那幅画，你的世界里不仅有一个孤单的小女孩坐在船上，还有许许多多有趣的元素——吃豆人、哥斯拉，还有泡泡糖机。我不知你是否和我感同身受，但我希望你能明白，无论你的小船划到哪里，这些都会一直陪伴着你。</p>
                
                <p>是你带我领略了这辈子可能独自无法见识的美景，是你让我了解到人与人之间更多的差异性，也是你让我对这个我已经有些放弃的世界重新燃起了热情。</p>
                
                <p>你一直说想被我坚定地选择，这封信就是我日思夜想，绞尽脑汁得出的结果。我可能不太善于表达内心的情绪，也可能无法给你带来像你给我的那样的感动，但我真诚地希望你能接受这份指向我们未来生活的邀请函。</p>
                
                <p>希望你能接纳我这颗笨拙却炽热的心。我爱你，请让我有幸能陪你度过余生的每一天。</p>
            </div>
            <div class="signature">
                <p>你的宝贝凯文</p>
            </div>
        </div>
    </div>
    <script>
        document.getElementById('submitPassword').addEventListener('click', function() {
            var password = document.getElementById('password').value;
            if(password === "0902") {
                document.getElementById('passwordForm').style.display = 'none';
                document.getElementById('content').style.display = 'block';
            } else {
                alert('💀嘟嘟哒嘟嘟哒💀');
            }
        });
    </script>
</body>
</html>
