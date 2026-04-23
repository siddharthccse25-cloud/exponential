# exponential
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Metadata -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Settings Panel for Web Application">
    <meta name="author" content="Student Project">

    <title>Settings Panel</title>

    <!-- Internal CSS -->
    <style>
        body {
            margin: 0;
            font-family: "Segoe UI", Arial, sans-serif;
            background: #eef2f7;
        }

        header {
            background: #1f2937;
            color: white;
            text-align: center;
            padding: 15px;
        }

        main {
            max-width: 700px;
            margin: 40px auto;
            background: #ffffff;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }

        h1, h2 {
            margin: 0 0 10px;
        }

        p {
            color: #555;
        }

        /* Tabs */
        input[type="radio"] {
            display: none;
        }

        nav {
            display: flex;
            margin-bottom: 20px;
            border-bottom: 2px solid #ddd;
        }

        nav label {
            flex: 1;
            padding: 12px;
            text-align: center;
            cursor: pointer;
            background: #f3f4f6;
            font-weight: bold;
            transition: 0.3s;
        }

        input:checked + label {
            background: #2563eb;
            color: #fff;
        }

        section {
            display: none;
        }

        #tab1:checked ~ #account,
        #tab2:checked ~ #notifications,
        #tab3:checked ~ #privacy {
            display: block;
        }

        /* Form Styling */
        form {
            margin-top: 15px;
        }

        label {
            display: block;
            margin-top: 10px;
            font-weight: 600;
        }

        input, select {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border-radius: 5px;
            border: 1px solid #ccc;
        }

        footer {
            text-align: center;
            margin-top: 20px;
            font-size: 14px;
            color: #777;
        }
    </style>
</head>

<body>

    <header>
        <h1><strong>Siddharth Chaudhari</strong></h1>
        <p><em>Manage your account, notifications, and privacy</em></p>
    </header>

    <main>

        <!-- Tabs -->
        <input type="radio" id="tab1" name="tab" checked>
        <label for="tab1">Account</label>

        <input type="radio" id="tab2" name="tab">
        <label for="tab2">Notifications</label>

        <input type="radio" id="tab3" name="tab">
        <label for="tab3">Privacy</label>

        <nav></nav>

        <!-- Account Section -->
        <section id="account">
            <h2>Account Settings</h2>
            <p><small>Update your personal details</small></p>

            <form>
                <label>Username</label>
                <input type="text" placeholder="Enter username">

                <label>Email</label>
                <input type="email" placeholder="Enter email">

                <label>Password</label>
                <input type="password" placeholder="Enter password">
            </form>
        </section>

        <!-- Notifications Section -->
        <section id="notifications">
            <h2>Notification Settings</h2>
            <p><small>Control how you receive alerts</small></p>

            <form>
                <label><input type="checkbox"> Email Notifications</label>
                <label><input type="checkbox"> SMS Notifications</label>
                <label><input type="checkbox"> Push Notifications</label>
            </form>
        </section>

        <!-- Privacy Section -->
        <section id="privacy">
            <h2>Privacy Settings</h2>
            <p><small>Manage your privacy preferences</small></p>

            <form>
                <label>Profile Visibility</label>
                <select>
                    <option>Public</option>
                    <option>Private</option>
                </select>

                <label><input type="checkbox"> Show Profile</label>
                <label><input type="checkbox"> Allow Messages</label>
            </form>
        </section>

        <footer>
            <p><strong>© 2026 Web App Project</strong></p>
        </footer>

    </main>

</body>
</html>
