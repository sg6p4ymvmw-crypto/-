<!DOCTYPE html>  
<html lang=**"**ar**"** dir=**"**rtl**"**>  
<head>  
    <meta charset=**"**UTF-8**"**>  
    <meta name=**"**viewport**"** content=**"**width=device-width, initial-scale=1.0**"**>  
    <title>**مبادرة** **قلوب** **متسامحة** | **الابتدائية** **الخامسة** **بالحناكية**</title>  
    <link href=**"**https**:**//fonts.googleapis.com/css2?family=Cairo**:**wght@400;600;700;900&display=swap**"** rel=**"**stylesheet**"**>  
    <link rel=**"**stylesheet**"** href=**"**https**:**//cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css**"**>  
    <style>  
        **:**root {  
            --primary**:** #6c5ce7;  
            --secondary**:** #a29bfe;  
            --accent**:** #fd79a8;  
            --bg**:** #f8f9fa;  
            --card-bg**:** #ffffff;  
            --text**:** #2d3436;  
            --success**:** #00b894;  
        }  
        * {  
            box-sizing**:** border-box;  
            margin**:** 0;  
            padding**:** 0;  
            font-family**:** **'**Cairo**'**, sans-serif;  
        }  
        body {  
            background-color**:** var**(**--bg**)**;  
            color**:** var**(**--text**)**;  
            min-height**:** 100vh;  
            display**:** flex;  
            flex-direction**:** column;  
        }  
        header {  
            background**:** linear-gradient**(**135deg, var**(**--primary**)**, var**(**--secondary**))**;  
            color**:** white;  
            padding**:** 2.5rem 1rem;  
            text-align**:** center;  
            box-shadow**:** 0 4px 15px rgba**(**0,0,0,0.1**)**;  
        }  
        header h1 {  
            font-size**:** 2.3rem;  
            margin-bottom**:** 0.5rem;  
            font-weight**:** 900;  
        }  
        header p {  
            font-size**:** 1.1rem;  
            opacity**:** 0.95;  
            margin-bottom**:** 0.5rem;  
        }  
        .team-badge {  
            background**:** rgba**(**255, 255, 255, 0.2**)**;  
            padding**:** 0.4rem 1rem;  
            border-radius**:** 20px;  
            font-size**:** 0.95rem;  
            display**:** inline-block;  
            margin-top**:** 0.5rem;  
        }  
        .container {  
            max-width**:** 1000px;  
            margin**:** 2rem auto;  
            padding**:** 0 1rem;  
            flex**:** 1;  
            width**:** 100%;  
        }  
        .stats-grid {  
            display**:** grid;  
            grid-template-columns**:** repeat**(**auto-fit, minmax**(**200px, 1fr**))**;  
            gap**:** 1.5rem;  
            margin-bottom**:** 2rem;  
        }  
        .stat-card {  
            background**:** var**(**--card-bg**)**;  
            padding**:** 1.5rem;  
            border-radius**:** 15px;  
            text-align**:** center;  
            box-shadow**:** 0 5px 15px rgba**(**0,0,0,0.05**)**;  
            border-bottom**:** 4px solid var**(**--primary**)**;  
        }  
        .stat-card h3 {  
            font-size**:** 2rem;  
            color**:** var**(**--primary**)**;  
            margin-bottom**:** 0.5rem;  
        }  
        .stat-card p {  
            color**:** #636e72;  
            font-weight**:** 600;  
        }  
        .card {  
            background**:** var**(**--card-bg**)**;  
            border-radius**:** 20px;  
            padding**:** 2rem;  
            box-shadow**:** 0 10px 30px rgba**(**0,0,0,0.08**)**;  
            margin-bottom**:** 2rem;  
        }  
        .card h2 {  
            color**:** var**(**--primary**)**;  
            margin-bottom**:** 1.5rem;  
            font-size**:** 1.5rem;  
            display**:** flex;  
            align-items**:** center;  
            gap**:** 10px;  
        }  
        .form-group {  
            margin-bottom**:** 1.2rem;  
        }  
        label {  
            display**:** block;  
            margin-bottom**:** 0.5rem;  
            font-weight**:** 600;  
        }  
        input, select, textarea {  
            width**:** 100%;  
            padding**:** 0.8rem 1rem;  
            border**:** 2px solid #dfe6e9;  
            border-radius**:** 10px;  
            font-size**:** 1rem;  
            transition**:** all 0.3s;  
        }  
        input**:**focus, select**:**focus, textarea**:**focus {  
            border-color**:** var**(**--primary**)**;  
            outline**:** none;  
            box-shadow**:** 0 0 0 3px rgba**(**108, 92, 231, 0.1**)**;  
        }  
        button {  
            background**:** var**(**--primary**)**;  
            color**:** white;  
            border**:** none;  
            padding**:** 0.9rem 2rem;  
            border-radius**:** 10px;  
            font-size**:** 1.1rem;  
            font-weight**:** 700;  
            cursor**:** pointer;  
            transition**:** background 0.3s, transform 0.2s;  
            width**:** 100%;  
        }  
        button**:**hover {  
            background**:** #5649c0;  
            transform**:** translateY**(**-2px**)**;  
        }  
        .tree-grid {  
            display**:** grid;  
            grid-template-columns**:** repeat**(**auto-fill, minmax**(**280px, 1fr**))**;  
            gap**:** 1.5rem;  
            margin-top**:** 1.5rem;  
        }  
        .wish-card {  
            background**:** linear-gradient**(**135deg, #fff, #fdfbf7**)**;  
            border**:** 2px dashed var**(**--secondary**)**;  
            padding**:** 1.5rem;  
            border-radius**:** 15px;  
            position**:** relative;  
            box-shadow**:** 0 4px 10px rgba**(**0,0,0,0.03**)**;  
        }  
        .wish-card .name {  
            font-weight**:** 700;  
            color**:** var**(**--primary**)**;  
            margin-bottom**:** 0.5rem;  
            font-size**:** 1.1rem;  
        }  
        .wish-card .class-tag {  
            background**:** var**(**--secondary**)**;  
            color**:** white;  
            padding**:** 0.2rem 0.6rem;  
            border-radius**:** 20px;  
            font-size**:** 0.8rem;  
            display**:** inline-block;  
            margin-bottom**:** 0.8rem;  
        }  
        .wish-card .msg {  
            color**:** #2d3436;  
            font-size**:** 0.95rem;  
            line-height**:** 1.5;  
        }  
        /* **نافذة** **الشهادة** */  
        .modal {  
            display**:** none;  
            position**:** fixed;  
            top**:** 0; left**:** 0; width**:** 100%; height**:** 100%;  
            background**:** rgba**(**0,0,0,0.6**)**;  
            justify-content**:** center;  
            align-items**:** center;  
            z-index**:** 1000;  
            padding**:** 1rem;  
        }  
        .cert-container {  
            background**:** white;  
            padding**:** 2.5rem;  
            border-radius**:** 20px;  
            text-align**:** center;  
            max-width**:** 600px;  
            width**:** 100%;  
            border**:** 8px solid var**(**--primary**)**;  
            position**:** relative;  
        }  
        .cert-container h2 {  
            color**:** var**(**--primary**)**;  
            font-size**:** 2rem;  
            margin-bottom**:** 1rem;  
        }  
        .cert-container p {  
            font-size**:** 1.1rem;  
            margin**:** 1rem 0;  
        }  
        .cert-name {  
            font-size**:** 1.7rem;  
            color**:** #d63031;  
            font-weight**:** 900;  
            margin**:** 1.5rem 0;  
            border-bottom**:** 2px solid #eee;  
            padding-bottom**:** 0.5rem;  
        }  
        .close-btn {  
            background**:** var**(**--success**)**;  
            margin-top**:** 1rem;  
        }  
        footer {  
            text-align**:** center;  
            padding**:** 1.5rem;  
            background**:** #2d3436;  
            color**:** white;  
            margin-top**:** auto;  
            font-size**:** 0.9rem;  
        }  
    </style>  
</head>  
<body>  
  
    <header>  
        <h1>**مبادرة** **"قلوب** **متسامحة"** 💜</h1>  
        <p>**الابتدائية** **الخامسة** **بالحناكية** | **تحت** **إشراف** **القائدة:** **صلفة** **الحربي**</p>  
        <div class=**"**team-badge**"**>  
            **إعداد** **وتنفيذ** **المعلمات:** **دلال** **الجهني** | **ابتسام** **القحطاني** | **زهور** **الصاعدي**  
        </div>  
    </header>  
  
    <div class=**"**container**"**>  
        <!-- **إحصائيات** -->  
        <div class=**"**stats-grid**"**>  
            <div class=**"**stat-card**"**>  
                <h3 id=**"**totalWishes**"**>0</h3>  
                <p>**إجمالي** **المشاركات**</p>  
            </div>  
            <div class=**"**stat-card**"**>  
                <h3 id=**"**totalParticipants**"**>0</h3>  
                <p>**الطالبات** **والمنسوبات** **المشاركات**</p>  
            </div>  
            <div class=**"**stat-card**"**>  
                <h3>16-19 **نوفمبر**</h3>  
                <p>**فترة** **المبادرة**</p>  
            </div>  
        </div>  
  
        <!-- **نموذج** **المشاركة** -->  
        <div class=**"**card**"**>  
            <h2><i class=**"**fa-solid fa-seedling**"**></i> **شاركـي** **معنا** **في** **"شجرة** **التسامح"**</h2>  
            <form id=**"**participationForm**"**>  
                <div class=**"**form-group**"**>  
                    <label>**الاسم** **الثلاثي:**</label>  
                    <input type=**"**text**"** id=**"**fullName**"** required placeholder=**"اكتبي** **اسمك** **هنا**...**"**>  
                </div>  
                <div class=**"**form-group**"**>  
                    <label>**الصف** **الدراسي** **أو** **المسمى** **الوظيفي:**</label>  
                    <select id=**"**userClass**"** required>  
                        <option value=**""**>**اختر** **الفصل** **أو** **الفئة**...</option>  
                        <option value=**"الصف** **الأول** **الابتدائي"**>**الصف** **الأول** **الابتدائي**</option>  
                        <option value=**"الصف** **الثاني** **الابتدائي"**>**الصف** **الثاني** **الابتدائي**</option>  
                        <option value=**"الصف** **الثالث** **الابتدائي"**>**الصف** **الثالث** **الابتدائي**</option>  
                        <option value=**"الصف** **الرابع** **الابتدائي"**>**الصف** **الرابع** **الابتدائي**</option>  
                        <option value=**"الصف** **الخامس** **الابتدائي"**>**الصف** **الخامس** **الابتدائي**</option>  
                        <option value=**"الصف** **السادس** **الابتدائي"**>**الصف** **السادس** **الابتدائي**</option>  
                        <option value=**"معلمة** / **إدارية** **(منسوبات** **المدرسة)"**>**معلمة** / **إدارية** **(منسوبات** **المدرسة)**</option>  
                    </select>  
                </div>  
                <div class=**"**form-group**"**>  
                    <label>**عبارة** **التسامح** **أو** **بطاقة** **اللطف:**</label>  
                    <textarea id=**"**wishMessage**"** rows=**"**3**"** required placeholder=**"مثال:** **شكراً** **لأنكِ** **ساعدتني** **اليوم** / **سامحتكِ** **من** **قلبي**...**"**></textarea>  
                </div>  
                <button type=**"**submit**"**><i class=**"**fa-solid fa-paper-plane**"**></i> **إرسال** **المشاركة** **واستلام** **شهادة** **الشكر**</button>  
            </form>  
        </div>  
  
        <!-- **شجرة** **التسامح** **(عرض** **المشاركات)** -->  
        <div class=**"**card**"**>  
            <h2><i class=**"**fa-solid fa-tree**"**></i> **شجرة** **التسامح** **(لوحة** **المشاركات** **الحيّة)**</h2>  
            <div class=**"**tree-grid**"** id=**"**wishesContainer**"**>  
                <!-- **المشاركات** **تظهر** **هنا** **ديناميكياً** -->  
            </div>  
        </div>  
    </div>  
  
    <!-- **نافذة** **شهادة** **الشكر** **التلقائية** -->  
    <div class=**"**modal**"** id=**"**certModal**"**>  
        <div class=**"**cert-container**"**>  
            <h2>**شهادة** **شكر** **وتقدير** 🏆</h2>  
            <p>**تتقدم** **إدارة** **الابتدائية** **الخامسة** **بالحناكية** **وفريق** **المبادرة** **بالشكر** **الجزيل** **لـ:**</p>  
            <div class=**"**cert-name**"** id=**"**modalName**"**>**اسم** **المشاركة**</div>  
            <p>**لمشاركتها** **التفاعلية** **المتميزة** **في** **مبادرة** <strong>**"قلوب** **متسامحة"**</strong>.</p>  
            <p style=**"**font-size**:** 0.85rem; color**:** #636e72; margin-top**:** 10px;**"**>**إعداد:** **دلال** **الجهني،** **ابتسام** **القحطاني،** **زهور** **الصاعدي**</p>  
            <button class=**"**close-btn**"** onclick=**"**closeModal**()"**>**تم،** **حفظ** **الشهادة**</button>  
        </div>  
    </div>  
  
    <footer>  
        **جميع** **الحقوق** **محفوظة** © 2026 - **الابتدائية** **الخامسة** **بالحناكية** | **إعداد** **المعلمات:** **دلال** **الجهني،** **ابتسام** **القحطاني،** **زهور** **الصاعدي**  
    </footer>  
  
    <script>  
        const form = document.getElementById**('**participationForm**')**;  
        const wishesContainer = document.getElementById**('**wishesContainer**')**;  
        const totalWishesEl = document.getElementById**('**totalWishes**')**;  
        const totalParticipantsEl = document.getElementById**('**totalParticipants**')**;  
        const certModal = document.getElementById**('**certModal**')**;  
        const modalName = document.getElementById**('**modalName**')**;  
  
        let wishes = JSON.parse**(**localStorage.getItem**('**school_wishes**'))** || [  
            { name**:** **'أ**. **ابتسام** **القحطاني'**, class**:** **'معلمة** / **إدارية** **(منسوبات** **المدرسة)'**, msg**:** **'بارك** **الله** **جهود** **الجميع** **ونشر** **التسامح** **بين** **طيات** **مدارسنا**.**'** },  
            { name**:** **'ريم** **محمد** **العوفي'**, class**:** **'الصف** **السادس** **الابتدائي'**, msg**:** **'شكراً** **لجمال** **هذه** **المبادرة،** **سامحت** **زميلاتي** **بكل** **حب**.**'** }  
        ];  
  
        function updateUI**()** {  
            wishesContainer.innerHTML = **''**;  
            totalWishesEl.textContent = wishes.length;  
            totalParticipantsEl.textContent = wishes.length;  
  
            wishes.forEach**(**item => {  
                const card = document.createElement**('**div**')**;  
                card.className = **'**wish-card**'**;  
                card.innerHTML = `  
                    <div class=**"**name**"**><i class=**"**fa-solid fa-user-check**"**></i> ${item.name}</div>  
                    <span class=**"**class-tag**"**>${item.class}</span>  
                    <div class=**"**msg**"**>**"**${item.msg}**"**</div>  
                `;  
                wishesContainer.appendChild**(**card**)**;  
            }**)**;  
        }  
  
        form.addEventListener**('**submit**'**, function**(**e**)** {  
            e.preventDefault**()**;  
            const name = document.getElementById**('**fullName**')**.value;  
            const userClass = document.getElementById**('**userClass**')**.value;  
            const msg = document.getElementById**('**wishMessage**')**.value;  
  
            wishes.unshift**(**{ name, class**:** userClass, msg }**)**;  
            localStorage.setItem**('**school_wishes**'**, JSON.stringify**(**wishes**))**;  
              
            updateUI**()**;  
            form.reset**()**;  
  
            // **إظهار** **شهادة** **الشكر** **الفورية** **باسم** **المشاركة**  
            modalName.textContent = name;  
            certModal.style.display = **'**flex**'**;  
        }**)**;  
  
        function closeModal**()** {  
            certModal.style.display = **'**none**'**;  
        }  
  
        updateUI**()**;  
    </script>  
</body>  
</html>  
