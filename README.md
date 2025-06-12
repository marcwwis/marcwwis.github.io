<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marc Wisniewski - Design Leadership Portfolio</title>
    <!-- Google Fonts - Inter for a clean, modern look -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- Tailwind CSS CDN for utility-first styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom CSS for finer control, overrides, and animations */
        body {
            font-family: 'Inter', sans-serif;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
        html {
            scroll-behavior: smooth;
        }
        /* Custom gradient background for hero section */
        .hero-gradient-bg {
            background: linear-gradient(135deg, #6B46C1 0%, #4C1D95 100%); /* Deeper, richer purple gradient */
        }
        /* Style for the unlock button with a subtle hover effect */
        .unlock-button {
            transition: all 0.3s ease-in-out;
            background-size: 200% auto;
            background-image: linear-gradient(to right, #8B5CF6 0%, #7C3AED 50%, #8B5CF6 100%);
        }
        .unlock-button:hover {
            background-position: right center; /* Shift gradient on hover */
            transform: translateY(-2px); /* Slight lift */
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }
        /* Style for project cards */
        .project-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        /* Hidden by default, shown by JS */
        .project-section {
            display: none;
        }

        /* Message Box Styling */
        .message-box-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.6);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 1000;
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.3s ease, visibility 0.3s ease;
        }
        .message-box-overlay.show {
            opacity: 1;
            visibility: visible;
        }
        .message-box {
            background-color: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.25);
            text-align: center;
            max-width: 400px;
            width: 90%;
            transform: translateY(-20px);
            opacity: 0;
            transition: transform 0.3s ease, opacity 0.3s ease;
        }
        .message-box-overlay.show .message-box {
            transform: translateY(0);
            opacity: 1;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- Header & Navigation -->
    <header class="bg-white shadow-lg py-5 sticky top-0 z-50">
        <nav class="w-full max-w-screen-2xl mx-auto flex flex-col md:flex-row justify-between items-center px-6 md:px-12">
            <div class="text-3xl font-semibold text-gray-900 mb-4 md:mb-0">Marc Wisniewski</div>
            <ul class="flex flex-wrap justify-center space-x-8 text-lg">
                <li><a href="#leadership" class="text-gray-700 hover:text-purple-700 font-medium transition duration-300 transform hover:scale-105">Leadership</a></li>
                <li><a href="#projects" class="text-gray-700 hover:text-purple-700 font-medium transition duration-300 transform hover:scale-105">Projects</a></li>
                <li><a href="#resume" class="text-gray-700 hover:text-purple-700 font-medium transition duration-300 transform hover:scale-105">Resume</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero-gradient-bg text-white py-28 px-6 sm:px-12 lg:px-16">
        <div class="w-full max-w-screen-2xl mx-auto flex flex-col md:flex-row items-center justify-center text-center md:text-left">
            <div class="md:w-1/3 mb-12 md:mb-0 md:mr-20 lg:mr-32 flex justify-center">
                <!-- Placeholder for user photo with enhanced styling -->
                <img src="https://placehold.co/280x280/F3F4F6/6B46C1/png?text=Your+Photo" alt="Marc Wisniewski" class="rounded-full w-72 h-72 object-cover shadow-2xl border-4 border-white transform hover:scale-105 transition-transform duration-300">
            </div>
            <div class="md:w-2/3">
                <h1 class="text-6xl sm:text-7xl lg:text-8xl font-bold leading-tight mb-8 animate-fade-in-up">Transformative <br class="hidden sm:inline">Design Leader</h1>
                <p class="text-xl sm:text-2xl leading-loose mb-8 animate-fade-in-up delay-200">For over two decades, I have helped organizations build teams and develop digital product and web experiences that engage users, drive revenue, and future-proof digital solutions.</p>
                <p class="text-lg sm:text-xl mt-6 animate-fade-in-up delay-400 leading-relaxed">My commitment to design transcends wireframes, visual designs, and prototypes. I lead teams that design transformative business solutions for clients by listening, simplifying, and preparing for disruption across all fronts.</p>
            </div>
        </div>
    </section>

    <!-- Design Leadership Capabilities -->
    <section id="leadership" class="py-24 px-6 sm:px-12 lg:px-16 bg-white">
        <div class="w-full max-w-screen-2xl mx-auto">
            <h2 class="text-5xl sm:text-6xl font-bold text-center mb-20 text-gray-900">My Design Leadership Capabilities</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-12">
                <div class="bg-purple-50 p-10 rounded-xl shadow-lg border border-purple-100 transform hover:scale-105 transition duration-300">
                    <h3 class="text-2xl font-semibold mb-5 text-purple-800">Strategic Vision & Execution</h3>
                    <p class="text-gray-700 leading-loose">Expert in setting and executing design strategies that align with key business objectives, leveraging AI and automation to boost productivity and innovation globally.</p>
                </div>
                <div class="bg-purple-50 p-10 rounded-xl shadow-lg border border-purple-100 transform hover:scale-105 transition duration-300">
                    <h3 class="text-2xl font-semibold mb-5 text-purple-800">Team Building & Culture</h3>
                    <p class="text-gray-700 leading-loose">Manages and cultivates high-performing multidisciplinary design teams (100+ professionals), fostering a fearless, positive, and experimental culture that thrives on innovation.</p>
                </div>
                <div class="bg-purple-50 p-10 rounded-xl shadow-lg border border-purple-100 transform hover:scale-105 transition duration-300">
                    <h3 class="text-2xl font-semibold mb-5 text-purple-800">Design Operations & Best Practices</h3>
                    <p class="text-gray-700 leading-loose">Champions agile and design best practices across diverse enterprise tool portfolios, driving efficiency and elevating design craft and quality through scalable operations models.</p>
                </div>
                <div class="bg-purple-50 p-10 rounded-xl shadow-lg border border-purple-100 transform hover:scale-105 transition duration-300">
                    <h3 class="text-2xl font-semibold mb-5 text-purple-800">Cross-Functional Collaboration</h3>
                    <p class="text-gray-700 leading-loose">Forges strong relationships with internal and external partners, enabling knowledge sharing and promoting seamless integration across disciplines to break down silos.</p>
                </div>
                <div class="bg-purple-50 p-10 rounded-xl shadow-lg border border-purple-100 transform hover:scale-105 transition duration-300">
                    <h3 class="text-2xl font-semibold mb-5 text-purple-800">Innovation & Future-Proofing</h3>
                    <p class="text-gray-700 leading-loose">Committed to designing transformative business solutions by anticipating disruption and evolving digital experiences, ensuring long-term relevance and success.</p>
                </div>
                <div class="bg-purple-50 p-10 rounded-xl shadow-lg border border-purple-100 transform hover:scale-105 transition duration-300">
                    <h3 class="text-2xl font-semibold mb-5 text-purple-800">Key Expertise Areas</h3>
                    <ul class="list-disc list-inside text-gray-700 space-y-3 leading-loose">
                        <li>Artificial Intelligence</li>
                        <li>Agile & Lean Methods</li>
                        <li>Creative Direction</li>
                        <li>Design Thinking</li>
                        <li>Design Operations</li>
                        <li>Front-End Development</li>
                        <li>Product Management</li>
                        <li>User-Centered Design</li>
                        <li>User Research</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section (Password Protected) -->
    <section id="projects" class="py-24 px-6 sm:px-12 lg:px-16 bg-gray-100">
        <div class="w-full max-w-screen-2xl mx-auto">
            <h2 class="text-5xl sm:text-6xl font-bold text-center mb-20 text-gray-900">Portfolio Samples</h2>

            <div id="password-form" class="text-center mb-12 p-10 bg-white rounded-xl shadow-lg">
                <p class="mb-8 text-xl text-gray-700 leading-relaxed">Enter password to view detailed project case studies:</p>
                <div class="flex flex-col sm:flex-row justify-center items-center space-y-6 sm:space-y-0 sm:space-x-6">
                    <input type="password" id="project-password" placeholder="Password" class="p-4 border-2 border-purple-300 rounded-lg shadow-sm focus:outline-none focus:ring-4 focus:ring-purple-200 text-lg w-full sm:w-80">
                    <button onclick="checkPassword()" class="unlock-button px-10 py-4 bg-purple-700 text-white font-bold rounded-lg shadow-xl hover:bg-purple-800 transition duration-300 text-lg w-full sm:w-auto">Unlock Projects</button>
                </div>
            </div>

            <!-- Message Box Overlay -->
            <div id="message-box-overlay" class="message-box-overlay">
                <div class="message-box">
                    <p id="message-box-text" class="text-xl font-semibold mb-8"></p>
                    <button onclick="closeMessageBox()" class="px-8 py-3 bg-purple-600 text-white rounded-lg hover:bg-purple-700 transition duration-300">OK</button>
                </div>
            </div>

            <div id="project-content" class="project-section space-y-24">
                <!-- Project 1: W3 INTRANET UNIFICATION -->
                <div class="bg-white p-10 sm:p-14 rounded-xl shadow-xl border border-gray-200 project-card">
                    <h3 class="text-3xl sm:text-4xl font-semibold text-purple-700 mb-8">W3 Intranet Unification: Increasing productivity for over 280,000 IBMers</h3>
                    <img src="https://placehold.co/1000x560/E0E0E0/6B46C1/png?text=W3+Intranet+Project+Image" alt="W3 Intranet Unification Project" class="w-full h-auto rounded-lg mb-10 shadow-md">
                    <p class="text-gray-700 mb-8 leading-loose text-lg">This project streamlined IBM’s intranet experience by unifying four key platforms (w3 main intranet, BluePages, Help@IBM, and w3 Search) into a single cohesive system, enhancing productivity and usability for 280,000+ IBMers. Recognized with the Nielsen Norman Best Intranet Award.</p>
                    <p class="text-gray-800 font-semibold mb-4 text-lg">Key Highlight:</p>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Demonstrates "Platform Thinking" – integrating distinct tools into a unified system to eliminate silos and foster collaborative product teams.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Problem: Silos and Inconsistency</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-10 space-y-3 leading-loose text-lg">
                        <li>Disjointed intranet with inconsistent experiences, disconnected features, difficult navigation, siloed functionalities, and prior failed unification attempts due to complexity and resistance.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Solution: Approach to Designing a Unified Intranet</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Achieved through iterative prototyping (for stakeholder buy-in), leveraging the w3 Design System for consistency, streamlining navigation, maintaining essential functionality, and developing a native mobile app.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">Collaboration, Upskilling, and Support:</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Partnered with leadership to establish a shared vision, built the necessary staffing plan, developed training workshops (for 13 designers, 30+ developers), and owned the design direction for the entire unified experience.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Impact: Measurable Success</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-10 space-y-3 leading-loose text-lg">
                        <li><strong>51.4 NPS</strong> (after one year)</li>
                        <li><strong>142M monthly active users</strong> (12.7% increase)</li>
                        <li><strong>89.7% users completing key tasks</strong></li>
                        <li><strong>5.4M monthly search queries</strong> (72% increase)</li>
                        <li>**Impact on CIO Organization:** Reduced design/developer support, improved team morale and collaboration, enhanced integration opportunities, reliable metrics for user behavior, and established a foundation for future evolution (e.g., AI integration).</li>
                    </ul>
                </div>

                <!-- Project 2: ASKIBM -->
                <div class="bg-white p-10 sm:p-14 rounded-xl shadow-xl border border-gray-200 project-card">
                    <h3 class="text-3xl sm:text-4xl font-semibold text-purple-700 mb-8">AskIBM: Bringing AI to a Global Workforce</h3>
                    <img src="https://placehold.co/1000x560/E0E0E0/6B46C1/png?text=AskIBM+Project+Image" alt="AskIBM Project" class="w-full h-auto rounded-lg mb-10 shadow-md">
                    <p class="text-gray-700 mb-8 leading-loose text-lg">A generative AI-powered assistant (watsonx and Granite LLM) for 280,000+ IBM employees, streamlining access to intranet and tools via a unified chat interface. Offers intelligent, context-aware solutions from document analysis to IT/HR support.</p>
                    <p class="text-gray-800 font-semibold mb-4 text-lg">Key Highlight:</p>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Showcases expertise in AI Strategy & Implementation – leveraging AI to solve real-world challenges and create user-centric solutions that transform workflows and deliver measurable impact.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Problem: Designing an AI that Works for Everyone</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-10 space-y-3 leading-loose text-lg">
                        <li>Challenges included educating IBMers on AI usage, fragmented tools (hundreds of independent watsonx chat experiences), ensuring scalability and consistency across platforms, and lost productivity due to routine tasks and information searches.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Solution: A Collaborative Approach to Redefining Productivity</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Iterative and user-driven process, including in-depth research, iterative prototyping to validate AI functionalities, a unified strategy integrating 13 specialized assistants, and a "Contribution First Framework" for reusable patterns.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The watsonx Challenge:</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">A company-wide initiative (3,400+ submissions) inviting employees to create custom workflows with AskIBM, leading to 43 highly productive workflows released for broader use and valuable feedback for product refinement.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Impact: Transforming Work at Every Level</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-10 space-y-3 leading-loose text-lg">
                        <li><strong>10k reported hours saved</strong> by IBMers</li>
                        <li><strong>504k average monthly prompts/queries</strong> (since July 2024)</li>
                        <li><strong>13 dedicated assistants</strong> federated</li>
                        <li><strong>3.4k+ community-built workflows</strong></li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">Concepts & Vision: Where it's going</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Focus on seamlessly integrating AI into existing workflows (search, dashboards, news) and interfaces, leveraging an iterative approach while overcoming technical hurdles and preserving the current ecosystem.</p>
                </div>

                <!-- Project 3: A UNIFIED DESIGN SYSTEM & LANGUAGE -->
                <div class="bg-white p-10 sm:p-14 rounded-xl shadow-xl border border-gray-200 project-card">
                    <h3 class="text-3xl sm:text-4xl font-semibold text-purple-700 mb-8">Carbon for IBMers: A Complete Design System Migration</h3>
                    <img src="https://placehold.co/1000x560/E0E0E0/6B46C1/png?text=Design+System+Project+Image" alt="Design System Project" class="w-full h-auto rounded-lg mb-10 shadow-md">
                    <p class="text-gray-700 mb-8 leading-loose text-lg">Transformed IBM's internal CIO design system by migrating the intranet to Carbon, IBM's official design system. This initiative streamlined resources, enhanced design consistency, and created a unified framework for internal tools and applications.</p>
                    <p class="text-gray-800 font-semibold mb-4 text-lg">Key Highlight:</p>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Emphasizes Systems Thinking, team coordination, and fostering a "contribution-first" mindset for scalable products and brand alignment. Required deep technical expertise in design systems.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Problem: The costs of maintaining an internal design system</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-10 space-y-3 leading-loose text-lg">
                        <li>Duplication of efforts (drained resources), outdated components and inconsistent patterns due to lack of investment (poor adoption), reinvention of the wheel (no shared updates), and scalability issues with growing product demands.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Solution: Inside the migration</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Redirected the internal design system team's focus to Carbon, established documentation and guidelines, conducted workshops and training, developed tailored Pattern Asset Libraries (Figma & Storybook), optimized processes, and fostered a contribution-first mindset with Carbon.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">Carbon for IBMers Figma Library:</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Centralized hub for design assets, components, templates, and patterns, ensuring consistency and efficiency.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">Carbon for IBMers Storybook:</h4>
                    <p class="text-gray-700 mb-10 leading-loose text-lg">Living repository for coded components, bridging design and development for consistent, reusable patterns.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">The Impact: After the migration</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-10 space-y-3 leading-loose text-lg">
                        <li><strong>68 NPS</strong> (14pt increase) after one year</li>
                        <li><strong>50% reported time savings</strong></li>
                        <li><strong>142M monthly visitors to homepage</strong> post-migration (12.7% increase)</li>
                        <li><strong>5 new initiatives/projects</strong> pursued due to efficiency gains.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-5">Continued Impact:</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-10 space-y-3 leading-loose text-lg">
                        <li>15 new components contributed to Carbon by internal teams, improved brand alignment, unified user experience, significantly improved accessibility, and strategic influence within the broader IBM ecosystem.</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Resume Section -->
    <section id="resume" class="py-24 px-6 sm:px-12 lg:px-16 bg-white">
        <div class="w-full max-w-screen-xl mx-auto"> <!-- Slightly narrower for resume readability -->
            <h2 class="text-5xl sm:text-6xl font-bold text-center mb-20 text-gray-900">My Resume</h2>

            <div class="bg-gray-100 p-10 sm:p-14 rounded-xl shadow-xl border border-gray-200">
                <h3 class="text-3xl sm:text-4xl font-semibold text-purple-700 mb-4">Marc Wisniewski</h3>
                <p class="text-xl font-medium text-gray-700 mb-6">Design Leader</p>
                <p class="text-gray-600 mb-10 text-lg">
                    marcwis@gmail.com | 914.471.3924 | <a href="https://linkedin.com/in/marcwis" target="_blank" class="text-purple-600 hover:underline hover:text-purple-800 transition duration-300">linkedin.com/in/marcwis</a>
                </p>

                <h4 class="text-2xl font-semibold text-gray-800 mb-5">Summary:</h4>
                <p class="text-gray-700 mb-10 leading-loose text-lg">Transformative Design Leader with a track record of digital growth, innovation, and success. For over two decades, I have helped organizations build teams and develop digital product and web experiences that engage users, drive revenue, and future-proof digital solutions. My commitment to design transcends wireframes, visual designs, and prototypes; I lead teams that design transformative business solutions for clients by listening, simplifying, and preparing for disruption across all fronts.</p>

                <h4 class="text-2xl font-semibold text-gray-800 mb-5">Expertise:</h4>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-y-3 text-gray-700 mb-10 text-lg">
                    <span>• Artificial Intelligence</span>
                    <span>• Agile & Lean Methods</span>
                    <span>• Creative Direction</span>
                    <span>• Design Thinking</span>
                    <span>• Design Operations</span>
                    <span>• Front-End Development</span>
                    <span>• Product Management</span>
                    <span>• User-Centered Design</span>
                    <span>• User Research</span>
                </div>

                <h4 class="text-2xl font-semibold text-gray-800 mb-6">Professional Experience:</h4>

                <!-- IBM Section -->
                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <h5 class="text-xl font-bold text-gray-800 mb-3">IBM</h5>
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Head of Design - IBM CIO AI, Automation & Data Platform</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2021 - Present</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Oversees strategic direction and daily operations of a 100+ multidisciplinary Design organization enhancing IBMer productivity through design and technology.</li>
                        <li>Partners with CIO leadership on design strategies aligning with key CIO objectives (AI, automation, productivity).</li>
                        <li>Cultivates a fearless, positive, and experimental team culture.</li>
                        <li>Champions agile and design best practices across 10+ enterprise tool portfolios.</li>
                        <li>Fosters knowledge sharing and networking with external design partners.</li>
                        <li>Maintains team awareness of enterprise design trends.</li>
                        <li>Leads design & user research tool strategy for 2,500+ designers and researchers worldwide.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Design Producer – CIO Office</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2018 - 2021</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Led Design practice within the CIO Office, delivering exceptional digital and physical experiences for IBMers.</li>
                        <li>Drove design and delivery of a robust design operations model for optimal organizational and people growth.</li>
                        <li>Championed and participated in improving the "design" function across the CIO through thought leadership, excellence, education, and mentorship.</li>
                        <li>Built a high-performing team by attracting top talent and fostering development for Managers and Designers.</li>
                        <li>Elevated design craft and quality via a centralized best practices library.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Executive, Design - Digital Business Group</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2015 - 2018</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Managed day-to-day operations of User Experience Design, User Research, and Adoption teams focused on world-class digital experiences for IBM clients.</li>
                        <li>Led design, development, and delivery of a robust UX framework for ibm.com (60M pages, 37 languages, 140 locales).</li>
                        <li>Drove web experience simplification program (sunsetted 5M+ legacy pages).</li>
                        <li>Led design, development, and delivery of web standards and adoption tooling for ibm.com authors.</li>
                        <li>Drove critical enhancements to ibm.com information architecture and taxonomy.</li>
                        <li>Led design, development, and delivery of reusable Drupal/WordPress templates.</li>
                        <li>Drove critical UX improvements via quantitative/qualitative insights, yielding increases in NPS, satisfaction, engagement, and conversion.</li>
                        <li>Won multiple internal (Best of IBM) and external industry awards.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Manager, Global Creative Director - CIO Office</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2013 - 2015</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Managed multidisciplinary UX team driving enhancements across IBM’s digital client experience.</li>
                        <li>Oversaw tone and direction of all internal/external agency design work published on ibm.com.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Product Owner, Senior Technical Staff Member – M&C Design Lab</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2011 - 2013</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Managed full-stack Agile scrum team designing/developing an as-a-service solution for modeling omnichannel client user journeys.</li>
                        <li>Interfaced with stakeholders for product requirements, scope, vision, and release plans.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Senior Art Director - CIO Office</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2004 - 2011</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Defined tone and visual direction of ibm.com desktop and mobile UX work products, high-fidelity concepts, design specifications, and interaction design documentation.</li>
                        <li>Interfaced with engineering teams to validate fit-and-finish of elements, patterns, and templates.</li>
                    </ul>
                </div>

                <!-- Other Experience Sections -->
                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <h5 class="text-xl font-bold text-gray-800 mb-3">Kforce</h5>
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Contractor - IBM Sales & Distribution</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2003 - 2004</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Designed and delivered high-fidelity design concepts for worldwide ibm.com user testing.</li>
                        <li>Generated design specifications and web standards documentation.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <h5 class="text-xl font-bold text-gray-800 mb-3">i3 Information & Imagination Inc.</h5>
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Creative Director</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">2000 - 2003</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Managed day-to-day operations of agency Design and Project Management teams.</li>
                        <li>Provided high-level design oversight on client projects (web sites, rich-media presentations, CBT, product UX).</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <h5 class="text-xl font-bold text-gray-800 mb-3">Fairfield University</h5>
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Adjunct Professor</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">1997 - 2003</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Authored and conducted courses on fundamentals of web design, intermediate web development, and rich-media design/development.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <h5 class="text-xl font-bold text-gray-800 mb-3">Buyroad.com Inc.</h5>
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Creative Director</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">1999 - 2000</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Managed Creative Services Department for design/delivery of product user experiences and printed marketing collateral.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <h5 class="text-xl font-bold text-gray-800 mb-3">EC Cubed, Inc.</h5>
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Marketing Program Manager</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">1997 - 1998</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Coordinated and implemented marketing plans focused on lead generation and client relationship management.</li>
                    </ul>
                </div>

                <div class="mb-12 pb-10 border-b border-gray-200 last:border-b-0">
                    <p class="text-lg font-semibold text-purple-700 flex flex-col md:flex-row justify-between items-start md:items-baseline mb-3">
                        <span>Multimedia Designer</span>
                        <span class="text-gray-600 font-normal text-base md:text-lg">1996 - 1997</span>
                    </p>
                    <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                        <li>Designed and developed client web sites, computer-based training modules, rich-media presentations, and printed corporate collateral.</li>
                    </ul>
                </div>

                <h4 class="text-2xl font-semibold text-gray-800 mb-5">Additional Related Experience:</h4>
                <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 mb-10 leading-loose text-lg">
                    <li>Imagine Video Services - Product Technician</li>
                    <li>Fox News Channel - Graphic Designer</li>
                </ul>

                <h4 class="text-2xl font-semibold text-gray-800 mb-5">Education:</h4>
                <p class="text-gray-700 mb-10 leading-loose text-lg">Bachelor of Science, Mass Communications - Summa Cum Laude, Eastern Connecticut State University</p>

                <h4 class="text-2xl font-semibold text-gray-800 mb-5">Certifications:</h4>
                <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 mb-10 leading-loose text-lg">
                    <li>Senior Technical Staff Member (STSM), IBM</li>
                    <li>Certified Scrum Product Owner (CSPO), Scrum Alliance</li>
                </ul>

                <h4 class="text-2xl font-semibold text-gray-800 mb-5">Technical Skills:</h4>
                <ul class="list-disc list-inside text-gray-700 ml-4 space-y-3 leading-loose text-lg">
                    <li><strong>Applications:</strong> Adobe Creative Cloud, Axure, Figma, Sketch, InVision, UxPin, HotJar, Medallia, Verint, Tealeaf, Coda, Jira, ZenHub, GitHub, Trello, Rational Team Concert, Slack, Microsoft Office</li>
                    <li><strong>Languages/Frameworks:</strong> HTML, CSS, JavaScript, Drupal, WordPress</li>
                    <li><strong>Operating Systems:</strong> MacOS, Windows</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12 px-6 text-center">
        <div class="w-full max-w-screen-2xl mx-auto">
            <p class="text-lg">&copy; 2024 Marc Wisniewski. All rights reserved.</p>
            <p class="text-sm mt-3 text-gray-400">Built with passion and leadership.</p>
        </div>
    </footer>

    <script>
        // Function to display messages in a modal-like box
        function showMessageBox(message) {
            const overlay = document.getElementById('message-box-overlay');
            const messageText = document.getElementById('message-box-text');
            messageText.textContent = message;
            overlay.classList.add('show');
        }

        // Function to close the message box
        function closeMessageBox() {
            const overlay = document.getElementById('message-box-overlay');
            overlay.classList.remove('show');
        }

        // Function to check the password for project access
        function checkPassword() {
            const passwordInput = document.getElementById('project-password').value;
            const projectContent = document.getElementById('project-content');
            const passwordForm = document.getElementById('password-form');
            const correctPassword = 'portfolio'; // The password is 'portfolio'

            if (passwordInput === correctPassword) {
                projectContent.style.display = 'block'; // Show projects
                passwordForm.style.display = 'none'; // Hide password form
                showMessageBox('Projects unlocked successfully!');
            } else {
                showMessageBox('Incorrect password. Please try again.');
            }
            // Clear the password input field after attempt
            document.getElementById('project-password').value = '';
        }
    </script>
</body>
</html>
