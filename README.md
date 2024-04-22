<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تحويل بيانات إلى ملف في Google Drive</title>
</head>
<body>
    <h1>أدخل الرمز الخاص بك ورقم السلة:</h1>
    <input type="text" id="code" placeholder="الرمز الخاص بك"><br><br>
    <input type="text" id="basket" placeholder="رقم السلة"><br><br>
    <button onclick="uploadToDrive()">تحميل إلى Google Drive</button>

    <script>
        function uploadToDrive() {
            // استخراج البيانات من الحقول
            var code = document.getElementById("code").value;
            var basket = document.getElementById("basket").value;

            // قم بتشكيل البيانات كما تريدها
            var dataToSave = "الرمز: " + code + "\n" + "رقم السلة: " + basket;

            // استدعاء دالة لرفع البيانات إلى Google Drive
            saveToGoogleDrive(dataToSave);
        }

        function saveToGoogleDrive(data) {
            // هنا يجب استخدام API من Google Drive لحفظ البيانات
            // لكن هذا خارج نطاق النموذج البسيط هنا
            // يمكنك البحث عن كيفية استخدام API من Google Drive وتنفيذ ذلك هنا
            console.log("البيانات التي سيتم حفظها: " + data);
            alert("تم حفظ البيانات في Google Drive بنجاح!");
        }
    </script>
</body>
</html>
