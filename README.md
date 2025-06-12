<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marc Wisniewski - Design Leader Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom CSS for finer control or overrides */
        html {
            scroll-behavior: smooth;
        }
        .gradient-bg {
            background: linear-gradient(to right, #6D28D9, #4C1D95); /* A vibrant purple gradient */
        }
        .project-section {
            display: none; /* Hidden by default */
        }
    </style>
</head>
<body class="font-sans text-gray-800 bg-gray-50">

    <header class="bg-white shadow-md py-4 sticky top-0 z-50">
        <nav class="container mx-auto flex justify-between items-center px-4">
            <div class="text-2xl font-bold text-gray-900">Marc Wisniewski</div>
            <ul class="flex space-x-6">
                <li><a href="#leadership" class="text-gray-600 hover:text-purple-700 transition duration-300">Leadership</a></li>
                <li><a href="#projects" class="text-gray-600 hover:text-purple-700 transition duration-300">Projects</a></li>
                <li><a href="#resume" class="text-gray-600 hover:text-purple-700 transition duration-300">Resume</a></li>
            </ul>
        </nav>
    </header>

    <section class="gradient-bg text-white py-20 px-4">
        <div class="container mx-auto flex flex-col md:flex-row items-center justify-center text-center md:text-left">
            <div class="md:w-1/3 mb-8 md:mb-0 md:mr-12">
                <img src="https://placehold.co/200x200/B8B8B8/FFFFFF/png?text=Your+Photo" alt="Marc Wisniewski" class="rounded-full w-48 h-48 object-cover mx-auto md:mx-0 shadow-lg border-4 border-white">
            </div>
            <div class="md:w-2/3">
                <h1 class="text-5xl font-extrabold leading-tight mb-4">Transformative Design Leader</h1>
                <p class="text-xl leading-relaxed">For over two decades, I have helped organizations build teams and develop digital product and web experiences that engage users, drive revenue, and future-proof digital solutions.</p>
                <p class="text-lg mt-4">My commitment to design transcends wireframes, visual designs, and prototypes. I lead teams that design transformative business solutions for clients by listening, simplifying, and preparing for disruption across all fronts.</p>
            </div>
        </div>
    </section>

    <section id="leadership" class="py-16 px-4 bg-white">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold text-center mb-12 text-gray-900">My Design Leadership Capabilities</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-gray-100 p-6 rounded-lg shadow-sm">
                    <h3 class="text-2xl font-semibold mb-4 text-purple-700">Strategic Vision & Execution</h3>
                    <p class="text-gray-700">Expert in setting and executing design strategies that align with key business objectives, leveraging AI and automation to boost productivity and innovation globally.</p>
                </div>
                <div class="bg-gray-100 p-6 rounded-lg shadow-sm">
                    <h3 class="text-2xl font-semibold mb-4 text-purple-700">Team Building & Culture</h3>
                    <p class="text-gray-700">Manages and cultivates high-performing multidisciplinary design teams (100+ professionals), fostering a fearless, positive, and experimental culture that thrives on innovation.</p>
                </div>
                <div class="bg-gray-100 p-6 rounded-lg shadow-sm">
                    <h3 class="text-2xl font-semibold mb-4 text-purple-700">Design Operations & Best Practices</h3>
                    <p class="text-gray-700">Champions agile and design best practices across diverse enterprise tool portfolios, driving efficiency and elevating design craft and quality through scalable operations models.</p>
                </div>
                <div class="bg-gray-100 p-6 rounded-lg shadow-sm">
                    <h3 class="text-2xl font-semibold mb-4 text-purple-700">Cross-Functional Collaboration</h3>
                    <p class="text-gray-700">Forges strong relationships with internal and external partners, enabling knowledge sharing and promoting seamless integration across disciplines to break down silos.</p>
                </div>
                <div class="bg-gray-100 p-6 rounded-lg shadow-sm">
                    <h3 class="text-2xl font-semibold mb-4 text-purple-700">Innovation & Future-Proofing</h3>
                    <p class="text-gray-700">Committed to designing transformative business solutions by anticipating disruption and evolving digital experiences, ensuring long-term relevance and success.</p>
                </div>
                <div class="bg-gray-100 p-6 rounded-lg shadow-sm">
                    <h3 class="text-2xl font-semibold mb-4 text-purple-700">Key Expertise Areas</h3>
                    <ul class="list-disc list-inside text-gray-700">
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

    ---

    <section id="projects" class="py-16 px-4 bg-gray-100">
        <div class="container mx-auto">
            <h2 class="text-4xl font-bold text-center mb-12 text-gray-900">Portfolio Samples</h2>

            <div id="password-form" class="text-center mb-8">
                <p class="mb-4 text-lg">Enter password to view project details:</p>
                <input type="password" id="project-password" class="p-3 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-2 focus:ring-purple-500 mr-2">
                <button onclick="checkPassword()" class="px-6 py-3 bg-purple-700 text-white font-semibold rounded-md shadow-md hover:bg-purple-800 transition duration-300">Unlock Projects</button>
                <p id="password-message" class="text-red-600 mt-2"></p>
            </div>

            <div id="project-content" class="project-section">
                <div class="bg-white p-8 rounded-lg shadow-lg mb-12">
                    <h3 class="text-3xl font-bold text-purple-700 mb-4">W3 Intranet Unification: Increasing productivity for over 280,000 IBMers</h3>
                    <img src="https://placehold.co/800x450/E0E0E0/333333/png?text=W3+Intranet+Project" alt="W3 Intranet Unification Project" class="w-full h-auto rounded-md mb-6">
                    <p class="text-gray-700 mb-4">This project streamlined IBM’s intranet experience by unifying four key platforms (w3 main intranet, BluePages, Help@IBM, and w3 Search) into a single cohesive system, enhancing productivity and usability for 280,000+ IBMers. Recognized with the Nielsen Norman Best Intranet Award.</p>
                    <p class="text-gray-800 font-semibold mb-2">Key Highlight:</p>
                    <p class="text-gray-700 mb-4">Demonstrates "Platform Thinking" – integrating distinct tools into a unified system to eliminate silos and foster collaborative product teams.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Problem: Silos and Inconsistency</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-4">
                        <li>Disjointed intranet with inconsistent experiences, disconnected features, difficult navigation, siloed functionalities, and prior failed unification attempts due to complexity and resistance.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Solution: Approach to Designing a Unified Intranet</h4>
                    <p class="text-gray-700 mb-4">Achieved through iterative prototyping (for stakeholder buy-in), leveraging the w3 Design System for consistency, streamlining navigation, maintaining essential functionality, and developing a native mobile app.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">Collaboration, Upskilling, and Support:</h4>
                    <p class="text-gray-700 mb-4">Partnered with leadership to establish a shared vision, built the necessary staffing plan, developed training workshops (for 13 designers, 30+ developers), and owned the design direction for the entire unified experience.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Impact: Measurable Success</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-4">
                        <li><strong>51.4 NPS</strong> (after one year)</li>
                        <li><strong>142M monthly active users</strong> (12.7% increase)</li>
                        <li><strong>89.7% users completing key tasks</strong></li>
                        <li><strong>5.4M monthly search queries</strong> (72% increase)</li>
                        <li>**Impact on CIO Organization:** Reduced design/developer support, improved team morale and collaboration, enhanced integration opportunities, reliable metrics for user behavior, and established a foundation for future evolution (e.g., AI integration).</li>
                    </ul>
                </div>

                <div class="bg-white p-8 rounded-lg shadow-lg mb-12">
                    <h3 class="text-3xl font-bold text-purple-700 mb-4">AskIBM: Bringing AI to a Global Workforce</h3>
                    <img src="https://placehold.co/800x450/E0E0E0/333333/png?text=AskIBM+Project" alt="AskIBM Project" class="w-full h-auto rounded-md mb-6">
                    <p class="text-gray-700 mb-4">A generative AI-powered assistant (watsonx and Granite LLM) for 280,000+ IBM employees, streamlining access to intranet and tools via a unified chat interface. Offers intelligent, context-aware solutions from document analysis to IT/HR support.</p>
                    <p class="text-gray-800 font-semibold mb-2">Key Highlight:</p>
                    <p class="text-gray-700 mb-4">Showcases expertise in AI Strategy & Implementation – leveraging AI to solve real-world challenges and create user-centric solutions that transform workflows and deliver measurable impact.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Problem: Designing an AI that Works for Everyone</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-4">
                        <li>Challenges included educating IBMers on AI usage, fragmented tools (hundreds of independent watsonx chat experiences), ensuring scalability and consistency across platforms, and lost productivity due to routine tasks and information searches.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Solution: A Collaborative Approach to Redefining Productivity</h4>
                    <p class="text-gray-700 mb-4">Iterative and user-driven process, including in-depth research, iterative prototyping to validate AI functionalities, a unified strategy integrating 13 specialized assistants, and a "Contribution First Framework" for reusable patterns.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The watsonx Challenge:</h4>
                    <p class="text-gray-700 mb-4">A company-wide initiative (3,400+ submissions) inviting employees to create custom workflows with AskIBM, leading to 43 highly productive workflows released for broader use and valuable feedback for product refinement.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Impact: Transforming Work at Every Level</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-4">
                        <li><strong>10k reported hours saved</strong> by IBMers</li>
                        <li><strong>504k average monthly prompts/queries</strong> (since July 2024)</li>
                        <li><strong>13 dedicated assistants</strong> federated</li>
                        <li><strong>3.4k+ community-built workflows</strong></li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">Concepts & Vision: Where it's going</h4>
                    <p class="text-gray-700 mb-4">Focus on seamlessly integrating AI into existing workflows (search, dashboards, news) and interfaces, leveraging an iterative approach while overcoming technical hurdles and preserving the current ecosystem.</p>
                </div>

                <div class="bg-white p-8 rounded-lg shadow-lg">
                    <h3 class="text-3xl font-bold text-purple-700 mb-4">Carbon for IBMers: A Complete Design System Migration</h3>
                    <img src="https://placehold.co/800x450/E0E0E0/333333/png?text=Design+System+Project" alt="Design System Project" class="w-full h-auto rounded-md mb-6">
                    <p class="text-gray-700 mb-4">Transformed IBM's internal CIO design system by migrating the intranet to Carbon, IBM's official design system. This initiative streamlined resources, enhanced design consistency, and created a unified framework for internal tools and applications.</p>
                    <p class="text-gray-800 font-semibold mb-2">Key Highlight:</p>
                    <p class="text-gray-700 mb-4">Emphasizes Systems Thinking, team coordination, and fostering a "contribution-first" mindset for scalable products and brand alignment. Required deep technical expertise in design systems.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Problem: The costs of maintaining an internal design system</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-4">
                        <li>Duplication of efforts (drained resources), outdated components and inconsistent patterns due to lack of investment (poor adoption), reinvention of the wheel (no shared updates), and scalability issues with growing product demands.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Solution: Inside the migration</h4>
                    <p class="text-gray-700 mb-4">Redirected the internal design system team's focus to Carbon, established documentation and guidelines, conducted workshops and training, developed tailored Pattern Asset Libraries (Figma & Storybook), optimized processes, and fostered a contribution-first mindset with Carbon.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">Carbon for IBMers Figma Library:</h4>
                    <p class="text-gray-700 mb-4">Centralized hub for design assets, components, templates, and patterns, ensuring consistency and efficiency.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">Carbon for IBMers Storybook:</h4>
                    <p class="text-gray-700 mb-4">Living repository for coded components, bridging design and development for consistent, reusable patterns.</p>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">The Impact: After the migration</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-4">
                        <li><strong>68 NPS</strong> (14pt increase) after one year</li>
                        <li><strong>50% reported time savings</strong></li>
                        <li><strong>142M monthly visitors to homepage</strong> post-migration (12.7% increase)</li>
                        <li><strong>5 new initiatives/projects</strong> pursued due to efficiency gains.</li>
                    </ul>

                    <h4 class="text-2xl font-semibold text-gray-800 mb-2">Continued Impact:</h4>
                    <ul class="list-disc list-inside text-gray-700 mb-4">
                        <li>15 new components contributed to Carbon by internal teams, improved brand alignment, unified user experience, significantly improved accessibility, and strategic influence within the broader IBM ecosystem.</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    ---

    <section id="resume" class="py-16 px-4 bg-white">
        <div class="container mx-auto max-w-4xl">
            <h2 class="text-4xl font-bold text-center mb-12 text-gray-900">My Resume</h2>

            <div class="bg-gray-100 p-8 rounded-lg shadow-lg">
                <h3 class="text-3xl font-bold text-purple-700 mb-2">Marc Wisniewski</h3>
                <p class="text-xl font-semibold text-gray-700 mb-4">Design Leader</p>
                <p class="text-gray-600 mb-6">marcwis@gmail.com | 914.471.3924 | <a href="https://linkedin.com/in/marcwis" target="_blank" class="text-purple-600 hover:underline">linkedin.com/in/marcwis</a></p>

                <h4 class="text-2xl font-bold text-gray-800 mb-3">Summary:</h4>
                <p class="text-gray-700 mb-6">Transformative Design Leader with a track record of digital growth, innovation, and success. For over two decades, I have helped organizations build teams and develop digital product and web experiences that engage users, drive revenue, and future-proof digital solutions. My commitment to design transcends wireframes, visual designs, and prototypes; I lead teams that design transformative business solutions for clients by listening, simplifying, and preparing for disruption across all fronts.</p>

                <h4 class="text-2xl font-bold text-gray-800 mb-3">Expertise:</h4>
                <div class="grid grid-cols-2 sm:grid-cols-3 gap-2 text-gray-700 mb-6">
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

                <h4 class="text-2xl font-bold text-gray-800 mb-4">Professional Experience:</h4>

                <div class="mb-8">
                    <h5 class="text-xl font-bold text-gray-800">IBM</h5>
                    <p class="text-lg font-semibold text-purple-700">Head of Design - IBM CIO AI, Automation & Data Platform <span class="float-right text-gray-600">2021 - Present</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Oversees strategic direction and daily operations of a 100+ multidisciplinary Design organization enhancing IBMer productivity through design and technology.</li>
                        <li>Partners with CIO leadership on design strategies aligning with key CIO objectives (AI, automation, productivity).</li>
                        <li>Cultivates a fearless, positive, and experimental team culture.</li>
                        <li>Champions agile and design best practices across 10+ enterprise tool portfolios.</li>
                        <li>Fosters knowledge sharing and networking with external design partners.</li>
                        <li>Maintains team awareness of enterprise design trends.</li>
                        <li>Leads design & user research tool strategy for 2,500+ designers and researchers worldwide.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <p class="text-lg font-semibold text-purple-700">Design Producer – CIO Office <span class="float-right text-gray-600">2018 - 2021</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Led Design practice within the CIO Office, delivering exceptional digital and physical experiences for IBMers.</li>
                        <li>Drove design and delivery of a robust design operations model for optimal organizational and people growth.</li>
                        <li>Championed and participated in improving the "design" function across the CIO through thought leadership, excellence, education, and mentorship.</li>
                        <li>Built a high-performing team by attracting top talent and fostering development for Managers and Designers.</li>
                        <li>Elevated design craft and quality via a centralized best practices library.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <p class="text-lg font-semibold text-purple-700">Executive, Design - Digital Business Group <span class="float-right text-gray-600">2015 - 2018</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
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

                <div class="mb-8">
                    <p class="text-lg font-semibold text-purple-700">Manager, Global Creative Director - CIO Office <span class="float-right text-gray-600">2013 - 2015</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Managed multidisciplinary UX team driving enhancements across IBM’s digital client experience.</li>
                        <li>Oversaw tone and direction of all internal/external agency design work published on ibm.com.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <p class="text-lg font-semibold text-purple-700">Product Owner, Senior Technical Staff Member – M&C Design Lab <span class="float-right text-gray-600">2011 - 2013</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Managed full-stack Agile scrum team designing/developing an as-a-service solution for modeling omnichannel client user journeys.</li>
                        <li>Interfaced with stakeholders for product requirements, scope, vision, and release plans.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <p class="text-lg font-semibold text-purple-700">Senior Art Director - CIO Office <span class="float-right text-gray-600">2004 - 2011</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Defined tone and visual direction of ibm.com desktop and mobile UX work products, high-fidelity concepts, design specifications, and interaction design documentation.</li>
                        <li>Interfaced with engineering teams to validate fit-and-finish of elements, patterns, and templates.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <h5 class="text-xl font-bold text-gray-800">Kforce</h5>
                    <p class="text-lg font-semibold text-purple-700">Contractor - IBM Sales & Distribution <span class="float-right text-gray-600">2003 - 2004</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Designed and delivered high-fidelity design concepts for worldwide ibm.com user testing.</li>
                        <li>Generated design specifications and web standards documentation.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <h5 class="text-xl font-bold text-gray-800">i3 Information & Imagination Inc.</h5>
                    <p class="text-lg font-semibold text-purple-700">Creative Director <span class="float-right text-gray-600">2000 - 2003</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Managed day-to-day operations of agency Design and Project Management teams.</li>
                        <li>Provided high-level design oversight on client projects (web sites, rich-media presentations, CBT, product UX).</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <h5 class="text-xl font-bold text-gray-800">Fairfield University</h5>
                    <p class="text-lg font-semibold text-purple-700">Adjunct Professor <span class="float-right text-gray-600">1997 - 2003</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Authored and conducted courses on fundamentals of web design, intermediate web development, and rich-media design/development.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <h5 class="text-xl font-bold text-gray-800">Buyroad.com Inc.</h5>
                    <p class="text-lg font-semibold text-purple-700">Creative Director <span class="float-right text-gray-600">1999 - 2000</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Managed Creative Services Department for design/delivery of product user experiences and printed marketing collateral.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <h5 class="text-xl font-bold text-gray-800">EC Cubed, Inc.</h5>
                    <p class="text-lg font-semibold text-purple-700">Marketing Program Manager <span class="float-right text-gray-600">1997 - 1998</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Coordinated and implemented marketing plans focused on lead generation and client relationship management.</li>
                    </ul>
                </div>

                <div class="mb-8">
                    <p class="text-lg font-semibold text-purple-700">Multimedia Designer <span class="float-right text-gray-600">1996 - 1997</span></p>
                    <ul class="list-disc list-inside text-gray-700 ml-4">
                        <li>Designed and developed client web sites, computer-based training modules, rich-media presentations, and printed corporate collateral.</li>
                    </ul>
                </div>

                <h4 class="text-2xl font-bold text-gray-800 mb-4">Additional Related Experience:</h4>
                <ul class="list-disc list-inside text-gray-700 ml-4 mb-6">
                    <li>Imagine Video Services - Product Technician</li>
                    <li>Fox News Channel - Graphic Designer</li>
                </ul>

                <h4 class="text-2xl font-bold text-gray-800 mb-4">Education:</h4>
                <p class="text-gray-700 mb-6">Bachelor of Science, Mass Communications - Summa Cum Laude, Eastern Connecticut State University</p>

                <h4 class="text-2xl font-bold text-gray-800 mb-4">Certifications:</h4>
                <ul class="list-disc list-inside text-gray-700 ml-4 mb-6">
                    <li>Senior Technical Staff Member (STSM), IBM</li>
                    <li>Certified Scrum Product Owner (CSPO), Scrum Alliance</li>
                </ul>

                <h4 class="text-2xl font-bold text-gray-800 mb-4">Technical Skills:</h4>
                <ul class="list-disc list-inside text-gray-700 ml-4">
                    <li><strong>Applications:</strong> Adobe Creative Cloud, Axure, Figma, Sketch, InVision, UxPin, HotJar, Medallia, Verint, Tealeaf, Coda, Jira, ZenHub, GitHub, Trello, Rational Team Concert, Slack, Microsoft Office</li>
                    <li><strong>Languages/Frameworks:</strong> HTML, CSS, JavaScript, Drupal, WordPress</li>
                    <li><strong>Operating Systems:</strong> MacOS, Windows</li>
                </ul>
            </div>
        </div>
    </section>

    <footer class="bg-gray-800 text-white py-8 px-4 text-center">
        <div class="container mx-auto">
            <p>&copy; 2024 Marc Wisniewski. All rights reserved.</p>
        </div>
    </footer>

    <script>
        function checkPassword() {
            const passwordInput = document.getElementById('project-password').value;
            const projectContent = document.getElementById('project-content');
            const passwordForm = document.getElementById('password-form');
            const passwordMessage = document.getElementById('password-message');
            const correctPassword = 'portfolio'; // The password is 'portfolio'

            if (passwordInput === correctPassword) {
                projectContent.style.display = 'block'; // Show projects
                passwordForm.style.display = 'none'; // Hide password form
                passwordMessage.textContent = ''; // Clear any error message
            } else {
                passwordMessage.textContent = 'Incorrect password. Please try again.';
            }
        }
    </script>
</body>
</html>
