# new_students_form
New Students form
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form</title>
    <style>
        label {
            display: block;
            margin-bottom: 5px;
        }
        input[type="text"],
        input[type="date"],
        select,
        input[type="tel"],
        input[type="email"] {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border-radius: 5px;
            border: 1px solid #ccc;
            box-sizing: border-box;
        }
        input[type="radio"] {
            margin-bottom: 10px;
        }
        button {
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button.cancel {
            background-color: #dc3545;
        }
    </style>
</head>
<body>

<form action="submit-registration.php" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="dob">Date of Birth:</label>
    <input type="date" id="dob" name="dob" required>

    <label>Gender:</label>
    <label for="male"><input type="radio" id="male" name="gender" value="male" required> Male</label>
    <label for="female"><input type="radio" id="female" name="gender" value="female" required> Female</label>

    <label for="address">Address:</label>
    <input type="text" id="address" name="address" required>

    <label for="telephone">Telephone:</label>
    <input type="tel" id="telephone" name="telephone" required>

    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required>

    <label for="course">Course:</label>
    <select id="course" name="course" required>
        <option value="">Select a Course</option>
        <option value="Computer Science">Computer Science</option>
        <option value="Engineering">Engineering</option>
        <option value="Business">Business</option>
    </select>

    <button type="submit">Register</button>
    <button type="button" class="cancel">Cancel</button>
</form>

</body>
</html>
