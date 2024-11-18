<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wesele Boho - Wiadomości dla Pary Młodej</title>
    <style>
        /* Ogólne stylowanie */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fffaf0; /* Jasny kremowy */
            color: #5e4429; /* Brązowy */
        }
        header {
            background-color: #f4e3d7; /* Beżowy */
            padding: 20px;
            text-align: center;
        }
        header h1 {
            margin: 0;
            font-size: 2.5rem;
            color: #8d6e63; /* Przydymiony brąz */
        }
        nav {
            background-color: #f4e3d7;
            padding: 10px 20px;
            display: flex;
            justify-content: center;
            gap: 15px;
        }
        nav a {
            text-decoration: none;
            color: #5e4429;
            font-weight: bold;
            padding: 8px 15px;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        nav a:hover {
            background-color: #dec2a6; /* Jasny złoty */
        }
        section {
            padding: 30px 20px;
        }
        h2 {
            color: #8d6e63;
            font-size: 2rem;
            margin-bottom: 15px;
        }
        p {
            font-size: 1rem;
            line-height: 1.6;
        }
        form {
            display: flex;
            flex-direction: column;
            gap: 10px;
            max-width: 500px;
            margin: 0 auto;
        }
        input, textarea, select, button {
            padding: 10px;
            border: 1px solid #c5a07a;
            border-radius: 5px;
            font-size: 1rem;
        }
        button {
            background-color: #dec2a6;
            color: #5e4429;
            font-weight: bold;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #8d6e63;
            color: #fff;
        }
        footer {
            background-color: #f4e3d7;
            text-align: center;
            padding: 10px;
            font-size: 0.9rem;
            margin-top: 30px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Witamy na naszym weselu!</h1>
    </header>

    <nav>
        <a href="#message">Wiadomości</a>
        <a href="#menu">Menu</a>
        <a href="#reservation">Rezerwacja</a>
        <a href="#confirm">Potwierdź obecność</a>
    </nav>

    <section id="message">
        <h2>Prześlij nam wiadomość</h2>
        <p>Podziel się swoimi myślami, życzeniami lub ciepłymi słowami z Parą Młodą.</p>
        <form action="https://your-backend-server.com/send-message" method="POST">
            <textarea name="message" placeholder="Twoja wiadomość..." rows="5" required></textarea>
            <input type="text" name="name" placeholder="Twoje imię (opcjonalne)">
            <button type="submit">Wyślij</button>
        </form>
    </section>

    <section id="menu">
        <h2>Menu weselne</h2>
        <p>Sprawdź, co przygotowaliśmy dla Was w dniu naszego wesela:</p>
        <ul>
            <li>Przystawki: Carpaccio z buraka, deska serów.</li>
            <li>Daniew główne: Polędwiczki w sosie grzybowym, pieczone warzywa.</li>
            <li>Desery: Tort weselny, tarta z owocami.</li>
        </ul>
    </section>

    <section id="reservation">
        <h2>Rezerwacja miejsc noclegowych</h2>
        <p>Zarezerwuj miejsce noclegowe, jeśli planujesz zostać z nami na dłużej:</p>
        <form action="https://your-backend-server.com/reserve" method="POST">
            <label for="hotel">Wybierz hotel:</label>
            <select name="hotel" id="hotel">
                <option value="hotel-a">Hotel A</option>
                <option value="hotel-b">Hotel B</option>
                <option value="hotel-c">Hotel C</option>
            </select>
            <input type="text" name="name" placeholder="Twoje imię i nazwisko" required>
            <input type="number" name="guests" placeholder="Liczba osób" required>
            <button type="submit">Rezerwuj</button>
        </form>
    </section>

    <section id="confirm">
        <h2>Potwierdzenie obecności</h2>
        <p>Prosimy o potwierdzenie swojej obecności do dnia 28 lipca 2025:</p>
        <form action="https://your-backend-server.com/confirm" method="POST">
            <input type="text" name="name" placeholder="Twoje imię i nazwisko" required>
            <input type="number" name="guests" placeholder="Liczba osób" required>
            <button type="submit">Potwierdź</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Nasze Wesele</p>
    </footer>
</body>
</html>
