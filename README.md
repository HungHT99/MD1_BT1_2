# MD1_BT1_2
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
<h1> Nhap vao so thang de kiem tra so ngay</h1>
<input id="soThang" type="text">
<button id="soNgay" value="So Ngay" onclick="tinhSoNgay()">Tinh So Ngay</button>
<p> So ngay trong thang do la</p>
<p id="hienThi"></p>
<script>
    function tinhSoNgay() {
        let x = +document.getElementById('soThang').value;

        switch (x) {
            case 1:
            case 3:
            case 5:
            case 7:
            case 8:
            case 10:
            case 12:
                document.getElementById('hienThi').innerHTML = '31 ngay ';
                break;
            case 4:
            case 6:
            case 9:
            case 11:
                document.getElementById('hienThi').innerHTML = '30 ngay';
                break;
            case 2:
                document.getElementById('hienThi').innerHTML = '28 hoac 29 ngay';
                break;
        }

    }
</script>
</body>
</html>
