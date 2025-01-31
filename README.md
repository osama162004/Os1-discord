<!DOCTYPE html>

<html lang="ar">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>طلب موديراتور - سيرفر ديسكورد</title>

    <style>

        /* تنسيق عام للصفحة */

        body {

            font-family: 'Tajawal', Arial, sans-serif;

            background: linear-gradient(135deg, #1a1a1a, #000000);

            color: #ffffff;

            max-width: 800px;

            margin: 0 auto;

            padding: 20px;

            direction: rtl;

        }



        /* تنسيق العنوان الرئيسي */

        h1 {

            text-align: center;

            color: #00ffcc;

            font-size: 2.5rem;

            margin-bottom: 20px;

            text-shadow: 0 0 10px #00ffcc, 0 0 20px #00ffcc;

        }



        /* تنسيق النموذج */

        form {

            background-color: rgba(0, 0, 0, 0.8);

            padding: 20px;

            border-radius: 10px;

            border: 2px solid #00ffcc;

            box-shadow: 0 0 15px rgba(0, 255, 204, 0.5);

        }



        /* تنسيق مجموعات النموذج */

        .form-group {

            margin-bottom: 20px;

        }



        .form-group label {

            display: block;

            margin-bottom: 8px;

            font-weight: bold;

            color: #00ffcc;

        }



        .form-group input,

        .form-group textarea,

        .form-group select {

            width: 100%;

            padding: 10px;

            border: 2px solid #00ffcc;

            border-radius: 8px;

            font-size: 1rem;

            background-color: #1a1a1a;

            color: #ffffff;

            transition: border-color 0.3s ease, box-shadow 0.3s ease;

        }



        .form-group input:focus,

        .form-group textarea:focus,

        .form-group select:focus {

            border-color: #00ffcc;

            box-shadow: 0 0 10px rgba(0, 255, 204, 0.5);

            outline: none;

        }



        /* تنسيق الزر */

        button {

            display: block;

            width: 100%;

            background-color: #00ffcc;

            color: #1a1a1a;

            padding: 12px;

            border: none;

            border-radius: 8px;

            font-size: 1.1rem;

            cursor: pointer;

            transition: background-color 0.3s ease, box-shadow 0.3s ease;

        }



        button:hover {

            background-color: #00e6b8;

            box-shadow: 0 0 15px rgba(0, 255, 204, 0.8);

        }



        /* تنسيق النص داخل النصarea */

        textarea {

            resize: vertical;

            min-height: 100px;

        }



        /* تنسيق القائمة المنسدلة */

        select {

            appearance: none;

            background: url('data:image/svg+xml;utf8,<svg fill="%2300ffcc" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg"><path d="M7 10l5 5 5-5z"/></svg>') no-repeat right 10px center;

            background-size: 16px;

        }



        /* تنسيق للهاتف المحمول */

        @media (max-width: 600px) {

            h1 {

                font-size: 2rem;

            }



            form {

                padding: 15px;

            }



            .form-group input,

            .form-group textarea,

            .form-group select {

                font-size: 0.9rem;

            }



            button {

                font-size: 1rem;

            }

        }

    </style>

    <!-- خط Tajawal للعربية -->

    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700&display=swap" rel="stylesheet">

</head>

<body>

    <h1>طلب انضمام كـ موديراتور</h1>

    <form id="applicationForm" action="https://formspree.io/f/mpwqrdqg" method="POST">

        <div class="form-group">

            <label for="name">الاسم الكامل:</label>

            <input type="text" id="name" name="الاسم_الكامل" required>

        </div>



        <div class="form-group">

            <label for="age">العمر:</label>

            <input type="number" id="age" name="العمر" min="13" required>

        </div>



        <div class="form-group">

            <label for="discord">اسم المستخدم في ديسكورد:</label>

            <input type="text" id="discord" name="اسم_المستخدم_ديسكورد" placeholder="اسم المستخدم#1234" required>

        </div>



        <div class="form-group">

            <label for="experience">الخبرة السابقة:</label>

            <textarea id="experience" name="الخبرة_السابقة" rows="4" required></textarea>

        </div>



        <div class="form-group">

            <label for="reason">سبب التقديم:</label>

            <textarea id="reason" name="سبب_التقديم" rows="4" required></textarea>

        </div>



        <div class="form-group">

            <label for="availability">عدد الساعات المتاحة يوميًا:</label>

            <select id="availability" name="الساعات_المتاحة" required>

                <option value="1-2">1-2 ساعات</option>

                <option value="3-4">3-4 ساعات</option>

                <option value="5+">5 ساعات أو أكثر</option>

            </select>

        </div>



        <button type="submit">إرسال الطلب</button>

    </form>

</body>

</html>
