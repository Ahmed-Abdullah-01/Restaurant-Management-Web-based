<style>
    @keyframes gradientBG {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }

    @keyframes fadeIn {
        from { opacity: 0; transform: translateY(20px); }
        to { opacity: 1; transform: translateY(0); }
    }

    @keyframes float {
        0% { transform: translateY(0px); }
        50% { transform: translateY(-10px); }
        100% { transform: translateY(0px); }
    }

    @keyframes glow {
        0% { box-shadow: 0 0 5px rgba(30, 60, 114, 0.2); }
        50% { box-shadow: 0 0 20px rgba(30, 60, 114, 0.4); }
        100% { box-shadow: 0 0 5px rgba(30, 60, 114, 0.2); }
    }

    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        line-height: 1.6;
        color: #333;
        max-width: 800px;
        margin: 0 auto;
        padding: 20px;
        background: #f0f2f5;
    }

    .header {
        text-align: center;
        padding: 30px;
        background: linear-gradient(-45deg, #1e3c72, #2a5298, #1e3c72, #2a5298);
        background-size: 400% 400%;
        animation: gradientBG 15s ease infinite;
        color: white;
        border-radius: 15px;
        margin-bottom: 30px;
        box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        animation: glow 3s infinite;
    }

    .project-title {
        font-size: 2.8em;
        margin: 0;
        padding: 10px;
        color: #ffffff;
        text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        animation: fadeIn 1s ease-out;
    }

    .subtitle {
        font-size: 1.3em;
        color: #e0e0e0;
        margin: 10px 0;
        animation: fadeIn 1s ease-out 0.3s backwards;
    }

    .section {
        background: #ffffff;
        padding: 25px;
        border-radius: 12px;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        margin-bottom: 25px;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
        animation: fadeIn 0.8s ease-out;
    }

    .section:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 15px rgba(0,0,0,0.1);
    }

    .section-title {
        color: #1e3c72;
        border-bottom: 3px solid #1e3c72;
        padding-bottom: 10px;
        margin-bottom: 20px;
        font-size: 1.8em;
        position: relative;
    }

    .section-title::after {
        content: '';
        position: absolute;
        bottom: -3px;
        left: 0;
        width: 50px;
        height: 3px;
        background: #2a5298;
        transition: width 0.3s ease;
    }

    .section:hover .section-title::after {
        width: 100px;
    }

    .team-member {
        display: inline-block;
        margin: 10px;
        padding: 20px;
        background: #f8f9fa;
        border-radius: 10px;
        width: calc(50% - 20px);
        box-sizing: border-box;
        transition: all 0.3s ease;
        border: 1px solid #e9ecef;
        animation: float 6s ease-in-out infinite;
    }

    .team-member:hover {
        background: #e9ecef;
        transform: scale(1.02);
    }

    .team-member:nth-child(2) {
        animation-delay: 0.5s;
    }

    .supervisor {
        background: linear-gradient(135deg, #e8f4f8 0%, #d1e7f0 100%);
        padding: 20px;
        border-radius: 10px;
        margin: 15px 0;
        transition: all 0.3s ease;
        animation: fadeIn 1s ease-out;
    }

    .supervisor:hover {
        transform: translateX(10px);
        box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }

    .footer {
        text-align: center;
        margin-top: 40px;
        padding: 25px;
        background: linear-gradient(135deg, #f5f5f5 0%, #e8e8e8 100%);
        border-radius: 12px;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        animation: fadeIn 1s ease-out;
    }

    ul {
        list-style-type: none;
        padding-left: 0;
    }

    li {
        padding: 8px 0;
        position: relative;
        padding-left: 25px;
        transition: transform 0.3s ease;
    }

    li:hover {
        transform: translateX(10px);
    }

    li::before {
        content: '→';
        position: absolute;
        left: 0;
        color: #1e3c72;
        transition: transform 0.3s ease;
    }

    li:hover::before {
        transform: translateX(5px);
    }

    strong {
        color: #1e3c72;
        font-weight: 600;
    }

    @media (max-width: 600px) {
        .team-member {
            width: 100%;
            margin: 10px 0;
        }
        
        .project-title {
            font-size: 2em;
        }
    }
</style>

<div class="header">
    <h1 class="project-title">Restaurant Management System</h1>
    <p class="subtitle">A Database Project</p>
</div>

<div class="section">
    <h2 class="section-title">Project Overview</h2>
    <p>This is a comprehensive Restaurant Management System developed as a database project. The system includes features for menu management, order processing, reservation handling, and customer management.</p>
</div>

<div class="section">
    <h2 class="section-title">Team Members</h2>
    <div class="team-member">
        <strong>Ahmed Abdullah</strong><br>
        Roll Number: 23P-0522
    </div>
    <div class="team-member">
        <strong>Ehtasham Arif</strong><br>
        Roll Number: 23P-0567
    </div>
</div>

<div class="section">
    <h2 class="section-title">Supervisors</h2>
    <div class="supervisor">
        <strong>Yasir Arfat</strong><br>
        <strong>Shoaib Khan</strong>
    </div>
</div>

<div class="section">
    <h2 class="section-title">Institution</h2>
    <p>Fast National University of Computer and Emerging Sciences (FAST-NUCES)<br>
    Peshawar Campus</p>
</div>

<div class="section">
    <h2 class="section-title">Project Features</h2>
    <ul>
        <li>User Authentication System</li>
        <li>Menu Management</li>
        <li>Order Processing</li>
        <li>Reservation System</li>
        <li>Admin Dashboard</li>
        <li>Customer Management</li>
        <li>Employee Management</li>
        <li>Sales Reports and Analytics</li>
    </ul>
</div>

<div class="section">
    <h2 class="section-title">Technical Stack</h2>
    <ul>
        <li>Frontend: HTML, CSS, JavaScript, Bootstrap</li>
        <li>Backend: PHP</li>
        <li>Database: MySQL</li>
        <li>Server: XAMPP</li>
    </ul>
</div>

<div class="footer">
    <p>© 2024 Restaurant Management System | 4th Semester Database Project</p>
</div>
