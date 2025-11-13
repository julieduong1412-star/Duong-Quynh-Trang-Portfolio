<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Duong Quynh Trang - Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
        }

        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 40px;
            text-align: center;
            position: relative;
        }

        .profile-img-container {
            width: 150px;
            height: 150px;
            margin: 0 auto 20px;
            position: relative;
            cursor: pointer;
        }

        .profile-img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            background: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            color: #667eea;
        }

        .upload-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.6);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.3s;
            color: white;
            font-size: 14px;
        }

        .profile-img-container:hover .upload-overlay {
            opacity: 1;
        }

        #imageInput {
            display: none;
        }

        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        .subtitle {
            font-size: 1.2em;
            opacity: 0.9;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .content {
            padding: 40px;
        }

        .section {
            margin-bottom: 40px;
        }

        .section-title {
            font-size: 1.8em;
            color: #667eea;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid #667eea;
        }

        .objective {
            background: #f8f9ff;
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #667eea;
            font-style: italic;
        }

        .experience-item {
            margin-bottom: 30px;
            padding-left: 20px;
            border-left: 2px solid #e0e0e0;
        }

        .job-title {
            font-size: 1.2em;
            font-weight: bold;
            color: #333;
            margin-bottom: 5px;
        }

        .company {
            color: #667eea;
            font-weight: 600;
        }

        .date-location {
            color: #666;
            font-size: 0.9em;
            margin-bottom: 10px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }

        .skill-item {
            background: #f8f9ff;
            padding: 15px;
            border-radius: 8px;
            border-left: 3px solid #667eea;
        }

        .skill-name {
            font-weight: 600;
            color: #333;
        }

        .education-item {
            background: #f8f9ff;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 15px;
        }

        .degree {
            font-weight: bold;
            font-size: 1.1em;
            color: #333;
        }

        .hobbies {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .hobby-tag {
            background: #667eea;
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9em;
        }

        @media (max-width: 600px) {
            .header {
                padding: 40px 20px;
            }

            h1 {
                font-size: 2em;
            }

            .content {
                padding: 20px;
            }

            .contact-info {
                flex-direction: column;
                gap: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="profile-img-container" onclick="document.getElementById('imageInput').click()">
                <div class="profile-img" id="profileImg">👤</div>
                <div class="upload-overlay">Click để tải ảnh</div>
                <input type="file" id="imageInput" accept="image/*">
            </div>
            <h1>Duong Quynh Trang</h1>
            <p class="subtitle">Customer Support & Data Entry Specialist</p>
            <div class="contact-info">
                <div class="contact-item">📧 julieduong1412@gmail.com</div>
                <div class="contact-item">📱 0389590207</div>
                <div class="contact-item">📍 Hanoi, Vietnam</div>
            </div>
        </div>

        <div class="content">
            <div class="section">
                <h2 class="section-title">About Me</h2>
                <div class="objective">
                    Secure a responsible career opportunity to expand my learnings, knowledge, and skills and making a significant contribution to the success of the company.
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Professional Experience</h2>
                
                <div class="experience-item">
                    <div class="job-title">Data Entry Specialist & Customer Support Representative</div>
                    <div class="company">Leapsteam CO., LTD</div>
                    <div class="date-location">March 2025 - Present | Hanoi</div>
                    <ul>
                        <li>Support international customers via chat for travel company Triptogo</li>
                        <li>Enter and update product data into international website CMS</li>
                        <li>Handle inquiries and provide detailed information on tour packages</li>
                        <li>Ensure data accuracy and formatting compliance with international standards</li>
                    </ul>
                </div>

                <div class="experience-item">
                    <div class="job-title">Customer Service & Content Moderation Specialist</div>
                    <div class="company">Leapsteam CO., LTD</div>
                    <div class="date-location">October 2024 - April 2025 | Hanoi</div>
                    <ul>
                        <li>Managed customer inquiries via email and ticketing systems (Zendesk, Freshdesk)</li>
                        <li>Reviewed and moderated website content for compliance</li>
                        <li>Collaborated with technical and legal teams for issue resolution</li>
                    </ul>
                </div>

                <div class="experience-item">
                    <div class="job-title">Sales Representative</div>
                    <div class="company">CÔNG TY TNHH SOTECH</div>
                    <div class="date-location">March 2023 - June 2023 | Hanoi</div>
                    <ul>
                        <li>Conducted telesales and managed online sales platforms</li>
                        <li>Created product content and maintained customer relationships</li>
                        <li>Consistently met and exceeded monthly KPIs</li>
                    </ul>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Skills</h2>
                <div class="skills-grid">
                    <div class="skill-item">
                        <div class="skill-name">💻 Computer Skills</div>
                        Windows, Troubleshooting
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">📊 Office Skills</div>
                        MS Office, Google Workspace
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">🤖 AI Tools</div>
                        Task Automation, AI Platforms
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">📞 Call Center Software</div>
                        CRM, Zendesk, Freshdesk
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">🛒 E-commerce</div>
                        Platform Management, CMS
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">💬 Communication</div>
                        English, Team Collaboration
                    </div>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Education</h2>
                <div class="education-item">
                    <div class="degree">Bachelor of Business English</div>
                    <div class="company">Thuong Mai University</div>
                    <div class="date-location">August 2018 - May 2022 | GPA: 3.26</div>
                    <div>🏆 Comprehensive Student Award, Course K54</div>
                    <div>👥 Class Monitor of K54N6, English Faculty</div>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Interests</h2>
                <div class="hobbies">
                    <span class="hobby-tag">📚 Writing & Reading</span>
                    <span class="hobby-tag">🎵 Music & Novels</span>
                    <span class="hobby-tag">🍜 Food & Culture</span>
                    <span class="hobby-tag">📜 History & Politics</span>
                </div>
            </div>
        </div>
    </div>

    <script>
        const imageInput = document.getElementById('imageInput');
        const profileImg = document.getElementById('profileImg');

        imageInput.addEventListener('change', function(e) {
            const file = e.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(event) {
                    profileImg.innerHTML = '';
                    profileImg.style.backgroundImage = `url(${event.target.result})`;
                    profileImg.style.backgroundSize = 'cover';
                    profileImg.style.backgroundPosition = 'center';
                }
                reader.readAsDataURL(file);
            }
        });
    </script>
</body>
</html>
