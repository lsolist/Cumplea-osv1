<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lista de Cumpleaños</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
    <style>
        body {
            background: #f4f4f4;
            text-align: center;
            font-family: Arial, sans-serif;
        }
        .container {
            max-width: 600px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.2);
            margin-top: 50px;
        }
        .highlight {
            background-color: #ffeb3b !important;
        }
    </style>
</head>
<body>
    <div class="container animate__animated animate__fadeIn">
        <h2>Lista de Cumpleaños</h2>
        <div class="mb-3">
            <input type="text" id="name" class="form-control" placeholder="Nombre">
            <input type="month" id="date" class="form-control mt-2">
            <button class="btn btn-primary mt-3" onclick="addBirthday()">Agregar</button>
        </div>
        <ul id="birthdayList" class="list-group"></ul>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", loadBirthdays);

        function addBirthday() {
            const name = document.getElementById("name").value;
            const date = document.getElementById("date").value;
            if (name && date) {
                const list = document.getElementById("birthdayList");
                const item = document.createElement("li");
                item.className = "list-group-item animate__animated animate__fadeIn";
                item.innerHTML = `<strong>${name}</strong> - ${formatDate(date)} 
                <button class='btn btn-danger btn-sm float-end' onclick='removeBirthday(this)'>Eliminar</button>`;
                
                list.appendChild(item);
                saveBirthday(name, date);
                alert("Cumpleaños agregado exitosamente!");
                
                document.getElementById("name").value = "";
                document.getElementById("date").value = "";
                sortBirthdays();
            }
        }
        
        function formatDate(date) {
            const [year, month] = date.split("-");
            return `${month}/${year}`;
        }
        
        function saveBirthday(name, date) {
            let birthdays = JSON.parse(localStorage.getItem("birthdays")) || [];
            birthdays.push({ name, date });
            localStorage.setItem("birthdays", JSON.stringify(birthdays));
        }
        
        function loadBirthdays() {
            const list = document.getElementById("birthdayList");
            const birthdays = JSON.parse(localStorage.getItem("birthdays")) || [];
            list.innerHTML = "";
            birthdays.forEach(({ name, date }) => {
                const item = document.createElement("li");
                item.className = "list-group-item animate__animated animate__fadeIn";
                item.innerHTML = `<strong>${name}</strong> - ${formatDate(date)} 
                <button class='btn btn-danger btn-sm float-end' onclick='removeBirthday(this)'>Eliminar</button>`;
                
                list.appendChild(item);
            });
            sortBirthdays();
        }
        
        function removeBirthday(button) {
            const item = button.parentElement;
            item.remove();
            let birthdays = JSON.parse(localStorage.getItem("birthdays")) || [];
            birthdays = birthdays.filter(b => `${b.name} - ${formatDate(b.date)}` !== item.innerText.replace("Eliminar", "").trim());
            localStorage.setItem("birthdays", JSON.stringify(birthdays));
        }
        
        function sortBirthdays() {
            const list = document.getElementById("birthdayList");
            Array.from(list.children)
                .sort((a, b) => new Date(a.innerText.split(" - ")[1]) - new Date(b.innerText.split(" - ")[1]))
                .forEach(item => list.appendChild(item));
        }
    </script>
</body>
</html>
