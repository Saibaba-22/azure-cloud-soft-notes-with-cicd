<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Cloud & DevOps Engineering | Saibaba Kola</title>

    <meta name="description"
          content="Cloud and DevOps Engineering learning content covering Azure, Terraform, Git, Docker, Kubernetes, Ansible, Prometheus, Grafana, Azure DevOps and GitHub Actions.">

    <style>

        /* ================================
           GLOBAL
        ================================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f5f7fb;
            color: #172033;
            line-height: 1.7;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .container {
            width: min(1180px, 92%);
            margin: auto;
        }


        /* ================================
           HEADER
        ================================= */

        header {
            background: #ffffff;
            border-bottom: 1px solid #e5e7eb;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .navbar {
            min-height: 72px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 25px;
        }

        .logo {
            font-size: 21px;
            font-weight: 800;
            color: #172033;
        }

        .logo span {
            color: #2563eb;
        }

        .nav-links {
            display: flex;
            gap: 22px;
            list-style: none;
            flex-wrap: wrap;
        }

        .nav-links a {
            font-size: 14px;
            font-weight: 600;
            color: #596273;
        }

        .nav-links a:hover {
            color: #2563eb;
        }


        /* ================================
           HERO
        ================================= */

        .hero {
            background: #ffffff;
            padding: 95px 0 85px;
            border-bottom: 1px solid #e5e7eb;
        }

        .hero-content {
            max-width: 900px;
            margin: auto;
            text-align: center;
        }

        .hero-badge {
            display: inline-block;
            padding: 7px 16px;
            border: 1px solid #dbe3f0;
            border-radius: 50px;
            background: #f8fafc;
            color: #2563eb;
            font-size: 13px;
            font-weight: 700;
            margin-bottom: 22px;
        }

        .hero h1 {
            font-size: clamp(38px, 6vw, 68px);
            line-height: 1.1;
            margin-bottom: 22px;
            letter-spacing: -2px;
        }

        .hero h1 span {
            color: #2563eb;
        }

        .hero p {
            max-width: 760px;
            margin: auto;
            color: #667085;
            font-size: 18px;
        }

        .hero-tags {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 30px;
        }

        .hero-tags span {
            background: #f1f5f9;
            border: 1px solid #e2e8f0;
            padding: 8px 14px;
            border-radius: 7px;
            font-size: 13px;
            font-weight: 600;
            color: #475467;
        }


        /* ================================
           SECTION
        ================================= */

        section {
            padding: 75px 0;
        }

        .section-header {
            margin-bottom: 38px;
        }

        .section-number {
            color: #2563eb;
            font-size: 13px;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 1.5px;
        }

        .section-header h2 {
            font-size: 34px;
            margin-top: 5px;
            line-height: 1.2;
        }

        .section-header p {
            color: #667085;
            max-width: 720px;
            margin-top: 10px;
        }


        /* ================================
           OVERVIEW
        ================================= */

        .overview {
            background: #ffffff;
        }

        .overview-text {
            max-width: 900px;
            color: #596273;
            font-size: 16px;
        }

        .overview-text strong {
            color: #172033;
        }


        /* ================================
           TOPIC CARDS
        ================================= */

        .topic-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 22px;
        }

        .topic-card {
            background: #ffffff;
            border: 1px solid #e4e7ec;
            border-radius: 14px;
            padding: 27px;
            transition: 0.25s ease;
        }

        .topic-card:hover {
            transform: translateY(-3px);
            border-color: #cbd5e1;
            box-shadow: 0 12px 30px rgba(15, 23, 42, 0.07);
        }

        .topic-icon {
            width: 48px;
            height: 48px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 11px;
            background: #eff6ff;
            font-size: 23px;
            margin-bottom: 18px;
        }

        .topic-card h3 {
            font-size: 20px;
            margin-bottom: 12px;
        }

        .topic-card p {
            color: #667085;
            font-size: 14px;
        }


        /* ================================
           CONTENT BOX
        ================================= */

        .content-box {
            background: #ffffff;
            border: 1px solid #e4e7ec;
            border-radius: 14px;
            padding: 30px;
            margin-bottom: 25px;
        }

        .content-box h3 {
            font-size: 21px;
            margin-bottom: 17px;
        }

        .content-box h4 {
            font-size: 16px;
            margin: 20px 0 10px;
            color: #344054;
        }

        .content-list {
            list-style: none;
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 9px 30px;
        }

        .content-list li {
            color: #596273;
            font-size: 14px;
            position: relative;
            padding-left: 20px;
        }

        .content-list li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #2563eb;
            font-weight: bold;
        }


        /* ================================
           TECHNOLOGY TABLE
        ================================= */

        .table-wrapper {
            overflow-x: auto;
            background: #ffffff;
            border: 1px solid #e4e7ec;
            border-radius: 14px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            min-width: 700px;
        }

        th {
            background: #f8fafc;
            text-align: left;
            padding: 16px 18px;
            font-size: 13px;
            color: #344054;
            border-bottom: 1px solid #e4e7ec;
        }

        td {
            padding: 15px 18px;
            border-bottom: 1px solid #edf0f4;
            color: #596273;
            font-size: 14px;
        }

        tr:last-child td {
            border-bottom: none;
        }

        td:first-child {
            font-weight: 700;
            color: #172033;
        }


        /* ================================
           SKILLS
        ================================= */

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 18px;
        }

        .skill-card {
            background: #ffffff;
            border: 1px solid #e4e7ec;
            border-radius: 12px;
            padding: 23px;
        }

        .skill-card h3 {
            font-size: 17px;
            margin-bottom: 9px;
        }

        .skill-card p {
            font-size: 14px;
            color: #667085;
        }


        /* ================================
           CAREER
        ================================= */

        .career-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 18px;
        }

        .career-card {
            background: #ffffff;
            border: 1px solid #e4e7ec;
            border-radius: 13px;
            padding: 24px;
        }

        .career-card h3 {
            font-size: 17px;
            margin-bottom: 13px;
        }

        .career-card ul {
            list-style: none;
        }

        .career-card li {
            color: #667085;
            font-size: 14px;
            padding: 5px 0;
        }

        .career-card li::before {
            content: "→ ";
            color: #2563eb;
            font-weight: bold;
        }


        /* ================================
           ROLE COMBINATION
        ================================= */

        .role-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
        }

        .role {
            background: #ffffff;
            border: 1px solid #e4e7ec;
            border-radius: 10px;
            padding: 18px;
            text-align: center;
            font-size: 14px;
            font-weight: 700;
        }


        /* ================================
           STACK
        ================================= */

        .stack {
            background: #ffffff;
        }

        .stack-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 15px;
        }

        .stack-item {
            border: 1px solid #e4e7ec;
            background: #f8fafc;
            padding: 22px 12px;
            border-radius: 11px;
            text-align: center;
        }

        .stack-item .icon {
            font-size: 28px;
            display: block;
            margin-bottom: 9px;
        }

        .stack-item strong {
            display: block;
            font-size: 14px;
        }

        .stack-item small {
            display: block;
            color: #667085;
            font-size: 11px;
            margin-top: 4px;
        }


        /* ================================
           LEARNING PATH
        ================================= */

        .learning-path {
            max-width: 850px;
            margin: auto;
        }

        .path-item {
            display: flex;
            align-items: center;
            gap: 18px;
            background: #ffffff;
            border: 1px solid #e4e7ec;
            padding: 18px 22px;
            border-radius: 10px;
            margin-bottom: 10px;
        }

        .path-number {
            min-width: 40px;
            height: 40px;
            border-radius: 50%;
            background: #eff6ff;
            color: #2563eb;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 800;
            font-size: 13px;
        }

        .path-item strong {
            font-size: 15px;
        }

        .path-item span {
            color: #667085;
            font-size: 13px;
            margin-left: auto;
        }


        /* ================================
           OBJECTIVE
        ================================= */

        .objective {
            background: #172033;
            color: #ffffff;
        }

        .objective .section-number {
            color: #93c5fd;
        }

        .objective h2 {
            font-size: 34px;
            margin: 7px 0 18px;
        }

        .objective p {
            max-width: 850px;
            color: #cbd5e1;
            font-size: 17px;
        }


        /* ================================
           CREATED BY
        ================================= */

        .creator {
            background: #ffffff;
            text-align: center;
            padding: 85px 0;
        }

        .creator-badge {
            display: inline-block;
            background: #eff6ff;
            color: #2563eb;
            border: 1px solid #dbeafe;
            padding: 7px 15px;
            border-radius: 50px;
            font-size: 12px;
            font-weight: 800;
            margin-bottom: 18px;
        }

        .creator h2 {
            font-size: 38px;
            margin-bottom: 5px;
        }

        .creator h3 {
            color: #2563eb;
            font-size: 17px;
            margin-bottom: 17px;
        }

        .creator p {
            max-width: 650px;
            margin: auto;
            color: #667085;
            font-size: 15px;
        }

        .creator-stack {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 9px;
            margin-top: 25px;
        }

        .creator-stack span {
            padding: 7px 12px;
            background: #f8fafc;
            border: 1px solid #e4e7ec;
            border-radius: 6px;
            font-size: 12px;
            font-weight: 700;
            color: #475467;
        }


        /* ================================
           FOOTER
        ================================= */

        footer {
            background: #f8fafc;
            border-top: 1px solid #e4e7ec;
            padding: 25px 0;
            text-align: center;
        }

        footer p {
            color: #667085;
            font-size: 13px;
        }

        footer strong {
            color: #172033;
        }


        /* ================================
           RESPONSIVE
        ================================= */

        @media (max-width: 900px) {

            .nav-links {
                display: none;
            }

            .topic-grid,
            .content-list {
                grid-template-columns: 1fr;
            }

            .skills-grid,
            .career-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .stack-grid {
                grid-template-columns: repeat(3, 1fr);
            }

            .role-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 600px) {

            section {
                padding: 55px 0;
            }

            .hero {
                padding: 65px 0;
            }

            .hero h1 {
                font-size: 40px;
            }

            .hero p {
                font-size: 16px;
            }

            .skills-grid,
            .career-grid,
            .stack-grid,
            .role-grid {
                grid-template-columns: 1fr;
            }

            .content-box {
                padding: 22px;
            }

            .section-header h2 {
                font-size: 29px;
            }

            .path-item {
                align-items: flex-start;
            }

            .path-item span {
                display: none;
            }
        }

    </style>
</head>

<body>

<!-- =========================================
     NAVIGATION
========================================= -->

<header>
    <div class="container navbar">

        <div class="logo">
            ☁️ Cloud<span>DevOps</span>
        </div>

        <ul class="nav-links">
            <li><a href="#cloud">Cloud</a></li>
            <li><a href="#azure">Azure</a></li>
            <li><a href="#terraform">Terraform</a></li>
            <li><a href="#git">Git</a></li>
            <li><a href="#docker">Docker</a></li>
            <li><a href="#kubernetes">Kubernetes</a></li>
            <li><a href="#monitoring">Monitoring</a></li>
            <li><a href="#careers">Careers</a></li>
        </ul>

    </div>
</header>


<!-- =========================================
     HERO
========================================= -->

<section class="hero">

    <div class="container hero-content">

        <div class="hero-badge">
            CLOUD & DEVOPS ENGINEERING
        </div>

        <h1>
            Cloud & <span>DevOps</span><br>
            Engineering
        </h1>

        <p>
            A complete learning foundation covering cloud infrastructure,
            networking, Azure, Infrastructure as Code, containers,
            orchestration, automation, monitoring and CI/CD technologies.
        </p>

        <div class="hero-tags">
            <span>☁️ Cloud</span>
            <span>🔷 Azure</span>
            <span>🏗️ Terraform</span>
            <span>🔀 Git</span>
            <span>🐳 Docker</span>
            <span>☸️ Kubernetes</span>
            <span>⚙️ Ansible</span>
            <span>📊 Prometheus</span>
            <span>📈 Grafana</span>
            <span>🚀 CI/CD</span>
        </div>

    </div>

</section>


<!-- =========================================
     ABOUT
========================================= -->

<section class="overview">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                About
            </div>

            <h2>Cloud & DevOps Learning Journey</h2>

        </div>

        <p class="overview-text">

            This learning content is designed to build practical knowledge
            across <strong>Cloud Computing, Infrastructure, Networking,
            Automation, Containers, Kubernetes, Monitoring and DevOps.</strong>

            It brings together the technologies commonly used to build,
            manage, automate, deploy and monitor modern cloud infrastructure.

        </p>

    </div>

</section>


<!-- =========================================
     CLOUD COMPUTING
========================================= -->

<section id="cloud">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                01 · Cloud Computing
            </div>

            <h2>☁️ Cloud Computing</h2>

            <p>
                Understanding the fundamentals of data centers, cloud
                infrastructure, service models and networking.
            </p>

        </div>


        <div class="topic-grid">

            <div class="topic-card">

                <div class="topic-icon">🏢</div>

                <h3>Data Center</h3>

                <p>
                    Understanding what a data center is and the major
                    components required to operate IT infrastructure.
                </p>

                <h4>Topics</h4>

                <ul class="content-list">
                    <li>What is a Data Center</li>
                    <li>Parts of a Data Center</li>
                    <li>On-Premises Data Center</li>
                    <li>Cloud Data Center</li>
                    <li>Cloud Service Models</li>
                </ul>

            </div>


            <div class="topic-card">

                <div class="topic-icon">🌐</div>

                <h3>Networking Fundamentals</h3>

                <p>
                    Building the networking foundation required for
                    cloud and infrastructure engineering.
                </p>

                <h4>Topics</h4>

                <ul class="content-list">
                    <li>IP Address</li>
                    <li>IP Address Classes</li>
                    <li>CIDR</li>
                    <li>DNS</li>
                    <li>Basic Networking</li>
                    <li>Cloud Keywords</li>
                </ul>

            </div>

        </div>

    </div>

</section>


<!-- =========================================
     AZURE
========================================= -->

<section id="azure">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                02 · Microsoft Azure
            </div>

            <h2>🔷 Microsoft Azure</h2>

            <p>
                Cloud infrastructure, networking, compute, storage,
                identity, security, monitoring and disaster recovery.
            </p>

        </div>


        <div class="content-box">

            <h3>☁️ Azure Fundamentals</h3>

            <ul class="content-list">
                <li>Resource Group</li>
                <li>Azure Account Creation</li>
                <li>Azure Portal</li>
                <li>Azure Basic Networking</li>
                <li>IP Address</li>
                <li>CIDR – Classless Inter-Domain Routing</li>
                <li>DNS – Domain Name System</li>
                <li>VNet – Virtual Network</li>
            </ul>

        </div>


        <div class="content-box">

            <h3>🌐 Azure Networking</h3>

            <ul class="content-list">
                <li>VNet Peering</li>
                <li>NSG – Network Security Group</li>
                <li>NSG at NIC Level</li>
                <li>NSG at Subnet Level</li>
                <li>ASG – Application Security Group</li>
                <li>Azure Load Balancer</li>
                <li>Azure Application Gateway</li>
                <li>Azure Traffic Manager</li>
                <li>Azure Front Door</li>
                <li>Hub & Spoke Architecture</li>
                <li>Azure VPN</li>
            </ul>

        </div>


        <div class="content-box">

            <h3>🖥️ Azure Compute & Applications</h3>

            <ul class="content-list">
                <li>Azure Virtual Machines</li>
                <li>Image Creation</li>
                <li>VMSS – Virtual Machine Scale Sets</li>
                <li>Azure App Service</li>
                <li>Azure Bastion</li>
            </ul>

        </div>


        <div class="content-box">

            <h3>💾 Azure Storage & Database</h3>

            <ul class="content-list">
                <li>Storage Account</li>
                <li>Storage Account Access</li>
                <li>Identity Management</li>
                <li>Azure SQL</li>
            </ul>

        </div>


        <div class="content-box">

            <h3>🔄 Azure Backup & Disaster Recovery</h3>

            <ul class="content-list">
                <li>Recovery Services Vault</li>
                <li>Recovery Services Vault Recovery</li>
                <li>Backup</li>
                <li>Restore</li>
                <li>Site Recovery</li>
                <li>Geo-Replication</li>
                <li>Test Failover</li>
                <li>DR Drill Activity</li>
            </ul>

        </div>


        <div class="content-box">

            <h3>🔐 Azure Identity, Monitoring & Automation</h3>

            <ul class="content-list">
                <li>Azure Active Directory</li>
                <li>Microsoft Entra ID</li>
                <li>Azure Monitor</li>
                <li>Azure Logic Apps</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     TERRAFORM
========================================= -->

<section id="terraform">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                03 · Infrastructure as Code
            </div>

            <h2>🏗️ Terraform</h2>

            <p>
                Infrastructure as Code for defining, provisioning and
                managing cloud infrastructure.
            </p>

        </div>


        <div class="content-box">

            <h3>Terraform Fundamentals</h3>

            <ul class="content-list">
                <li>Introduction to Terraform</li>
                <li>Terraform Configuration</li>
                <li>Terraform Providers</li>
                <li>Terraform Resources</li>
                <li>Azure VNet Peering</li>
                <li>Virtual Machine Creation</li>
                <li>Variables</li>
                <li>Data Types</li>
                <li>Workspaces</li>
                <li>Depends On</li>
                <li>Data Blocks</li>
                <li>Import Command</li>
                <li>Modules</li>
                <li>Provisioners</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     GIT
========================================= -->

<section id="git">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                04 · Version Control
            </div>

            <h2>🔀 Git & GitHub</h2>

            <p>
                Version control, source code management, branching,
                collaboration and repository management.
            </p>

        </div>


        <div class="content-box">

            <h3>🔀 Version Control</h3>

            <ul class="content-list">
                <li>Introduction to Version Control</li>
                <li>Centralized Version Control System</li>
                <li>Distributed Version Control System</li>
                <li>Git Installation</li>
                <li>Git Areas</li>
            </ul>

        </div>


        <div class="content-box">

            <h3>🌍 GitHub & Collaboration</h3>

            <ul class="content-list">
                <li>GitHub Introduction</li>
                <li>Personal Access Token</li>
                <li>PAT Management</li>
                <li>Add New Token</li>
                <li>Remove Old Token</li>
                <li>Git Basic Commands</li>
                <li>Git Branching Strategy</li>
                <li>Merge Conflicts</li>
                <li>Pull Requests</li>
                <li>Hotfix Requests</li>
                <li>Git Commands Reference</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     DOCKER
========================================= -->

<section id="docker">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                05 · Containerization
            </div>

            <h2>🐳 Docker</h2>

            <p>
                Containerization, image management, networking, storage
                and multi-container applications.
            </p>

        </div>


        <div class="content-box">

            <h3>🐳 Docker Fundamentals</h3>

            <ul class="content-list">
                <li>Docker Introduction</li>
                <li>Docker Architecture</li>
                <li>Docker Internal Architecture</li>
                <li>Docker Installation</li>
                <li>Image Operations</li>
                <li>Container Operations</li>
                <li>Docker Networks</li>
                <li>Docker Volumes</li>
                <li>Dockerfile</li>
                <li>Image Creation</li>
                <li>Image Optimization</li>
                <li>Multi-Stage Dockerfile</li>
                <li>Docker Compose</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     KUBERNETES
========================================= -->

<section id="kubernetes">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                06 · Container Orchestration
            </div>

            <h2>☸️ Kubernetes</h2>

            <p>
                Container orchestration, cluster architecture,
                services, ingress, namespaces and Helm.
            </p>

        </div>


        <div class="content-box">

            <h3>☸️ Kubernetes Fundamentals</h3>

            <ul class="content-list">
                <li>Docker vs Kubernetes</li>
                <li>Kubernetes Introduction</li>
                <li>Kubernetes Architecture</li>
                <li>Kubernetes Components</li>
                <li>Kubernetes Services</li>
                <li>Service LoadBalancer</li>
                <li>Service Ingress</li>
                <li>Namespaces</li>
                <li>Helm Charts</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     ANSIBLE
========================================= -->

<section>

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                07 · Configuration Management
            </div>

            <h2>⚙️ Ansible</h2>

            <p>
                Configuration management and infrastructure automation.
            </p>

        </div>


        <div class="content-box">

            <ul class="content-list">
                <li>Ansible Introduction</li>
                <li>Ansible Architecture</li>
                <li>Playbooks</li>
                <li>Roles</li>
                <li>Shell Module</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     MONITORING
========================================= -->

<section id="monitoring">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                08 · Monitoring & Observability
            </div>

            <h2>📊 Prometheus & Grafana</h2>

            <p>
                Infrastructure monitoring, metrics collection,
                alerting and visualization.
            </p>

        </div>


        <div class="topic-grid">

            <div class="topic-card">

                <div class="topic-icon">📊</div>

                <h3>Prometheus</h3>

                <ul class="content-list">
                    <li>Prometheus Introduction</li>
                    <li>Features & Components</li>
                    <li>Prometheus Architecture</li>
                    <li>Internal Architecture</li>
                    <li>Node Exporter</li>
                    <li>Alertmanager</li>
                </ul>

            </div>


            <div class="topic-card">

                <div class="topic-icon">📈</div>

                <h3>Grafana</h3>

                <ul class="content-list">
                    <li>Grafana Introduction</li>
                    <li>Grafana Architecture</li>
                    <li>Prometheus Integration</li>
                    <li>Dashboards</li>
                    <li>Visualization</li>
                    <li>Monitoring</li>
                </ul>

            </div>

        </div>

    </div>

</section>


<!-- =========================================
     AZURE DEVOPS
========================================= -->

<section>

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                09 · DevOps Platform
            </div>

            <h2>🔷 Azure DevOps</h2>

            <p>
                Azure DevOps services, agents, YAML-based infrastructure
                deployment, boards and CI/CD concepts.
            </p>

        </div>


        <div class="content-box">

            <ul class="content-list">
                <li>Azure DevOps Introduction</li>
                <li>Account Creation</li>
                <li>Azure DevOps Components</li>
                <li>Options & Components Briefing</li>
                <li>Self-Hosted Agent</li>
                <li>Terraform Deployment Using YAML</li>
                <li>End-to-End CI/CD</li>
                <li>Azure Boards</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     GITHUB ACTIONS
========================================= -->

<section>

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                10 · CI/CD Automation
            </div>

            <h2>🚀 GitHub Actions</h2>

            <p>
                Automation and CI/CD using GitHub Actions,
                YAML and Terraform.
            </p>

        </div>


        <div class="content-box">

            <ul class="content-list">
                <li>GitHub Actions Introduction</li>
                <li>Workflow</li>
                <li>GitHub Actions Architecture</li>
                <li>Internal Architecture</li>
                <li>Create an Action File</li>
                <li>YAML Configuration</li>
                <li>Sample YAML</li>
                <li>Terraform with GitHub Actions</li>
            </ul>

        </div>

    </div>

</section>


<!-- =========================================
     TECHNOLOGY STACK
========================================= -->

<section class="stack">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                Technology Stack
            </div>

            <h2>🛠️ Tools & Technologies</h2>

            <p>
                The core technology stack covered across this learning journey.
            </p>

        </div>


        <div class="stack-grid">

            <div class="stack-item">
                <span class="icon">☁️</span>
                <strong>Azure</strong>
                <small>Cloud</small>
            </div>

            <div class="stack-item">
                <span class="icon">🏗️</span>
                <strong>Terraform</strong>
                <small>IaC</small>
            </div>

            <div class="stack-item">
                <span class="icon">🔀</span>
                <strong>Git</strong>
                <small>Version Control</small>
            </div>

            <div class="stack-item">
                <span class="icon">🌍</span>
                <strong>GitHub</strong>
                <small>Repository</small>
            </div>

            <div class="stack-item">
                <span class="icon">🐳</span>
                <strong>Docker</strong>
                <small>Containers</small>
            </div>

            <div class="stack-item">
                <span class="icon">☸️</span>
                <strong>Kubernetes</strong>
                <small>Orchestration</small>
            </div>

            <div class="stack-item">
                <span class="icon">⚙️</span>
                <strong>Ansible</strong>
                <small>Automation</small>
            </div>

            <div class="stack-item">
                <span class="icon">📊</span>
                <strong>Prometheus</strong>
                <small>Monitoring</small>
            </div>

            <div class="stack-item">
                <span class="icon">📈</span>
                <strong>Grafana</strong>
                <small>Visualization</small>
            </div>

            <div class="stack-item">
                <span class="icon">🔷</span>
                <strong>Azure DevOps</strong>
                <small>DevOps Platform</small>
            </div>

            <div class="stack-item">
                <span class="icon">🚀</span>
                <strong>GitHub Actions</strong>
                <small>CI/CD</small>
            </div>

            <div class="stack-item">
                <span class="icon">📄</span>
                <strong>YAML</strong>
                <small>Configuration</small>
            </div>

        </div>

    </div>

</section>


<!-- =========================================
     TECHNOLOGY TABLE
========================================= -->

<section>

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                Technology Overview
            </div>

            <h2>🧰 Complete Technology Map</h2>

        </div>


        <div class="table-wrapper">

            <table>

                <thead>

                    <tr>
                        <th>Area</th>
                        <th>Technologies / Concepts</th>
                    </tr>

                </thead>

                <tbody>

                    <tr>
                        <td>☁️ Cloud</td>
                        <td>Microsoft Azure, Cloud Computing, Service Models</td>
                    </tr>

                    <tr>
                        <td>🌐 Networking</td>
                        <td>VNet, DNS, IP, CIDR, NSG, ASG, VPN, Peering</td>
                    </tr>

                    <tr>
                        <td>🖥️ Compute</td>
                        <td>Azure VM, VMSS, App Service, Images</td>
                    </tr>

                    <tr>
                        <td>💾 Storage</td>
                        <td>Azure Storage Account, Storage Access</td>
                    </tr>

                    <tr>
                        <td>🗄️ Database</td>
                        <td>Azure SQL</td>
                    </tr>

                    <tr>
                        <td>🔐 Identity</td>
                        <td>Microsoft Entra ID, Identity Management</td>
                    </tr>

                    <tr>
                        <td>🛡️ Security</td>
                        <td>NSG, ASG, Bastion, Identity</td>
                    </tr>

                    <tr>
                        <td>🔄 Disaster Recovery</td>
                        <td>Recovery Services Vault, Site Recovery, Failover</td>
                    </tr>

                    <tr>
                        <td>🏗️ IaC</td>
                        <td>Terraform</td>
                    </tr>

                    <tr>
                        <td>🔀 Version Control</td>
                        <td>Git & GitHub</td>
                    </tr>

                    <tr>
                        <td>🐳 Containers</td>
                        <td>Docker</td>
                    </tr>

                    <tr>
                        <td>☸️ Orchestration</td>
                        <td>Kubernetes, Helm</td>
                    </tr>

                    <tr>
                        <td>⚙️ Automation</td>
                        <td>Ansible</td>
                    </tr>

                    <tr>
                        <td>📊 Monitoring</td>
                        <td>Prometheus, Node Exporter, Alertmanager</td>
                    </tr>

                    <tr>
                        <td>📈 Visualization</td>
                        <td>Grafana</td>
                    </tr>

                    <tr>
                        <td>🚀 CI/CD</td>
                        <td>Azure DevOps, GitHub Actions</td>
                    </tr>

                </tbody>

            </table>

        </div>

    </div>

</section>


<!-- =========================================
     SKILLS
========================================= -->

<section>

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                Skills
            </div>

            <h2>🎯 Skills Covered</h2>

            <p>
                Key technical domains developed through this learning path.
            </p>

        </div>


        <div class="skills-grid">

            <div class="skill-card">
                <h3>☁️ Cloud Computing</h3>
                <p>
                    Cloud fundamentals, data centers, cloud service models
                    and infrastructure concepts.
                </p>
            </div>

            <div class="skill-card">
                <h3>🌐 Networking</h3>
                <p>
                    IP addressing, CIDR, DNS, VNets, peering, NSG,
                    ASG, VPN and load balancing.
                </p>
            </div>

            <div class="skill-card">
                <h3>🔷 Azure</h3>
                <p>
                    Azure compute, storage, networking, security,
                    identity, monitoring and disaster recovery.
                </p>
            </div>

            <div class="skill-card">
                <h3>🏗️ Infrastructure as Code</h3>
                <p>
                    Terraform variables, modules, workspaces,
                    data blocks, dependencies and infrastructure deployment.
                </p>
            </div>

            <div class="skill-card">
                <h3>🔀 Version Control</h3>
                <p>
                    Git, GitHub, branching, merging, pull requests,
                    conflicts and token management.
                </p>
            </div>

            <div class="skill-card">
                <h3>🐳 Containers</h3>
                <p>
                    Docker images, containers, networks, volumes,
                    Dockerfiles, optimization and Compose.
                </p>
            </div>

            <div class="skill-card">
                <h3>☸️ Orchestration</h3>
                <p>
                    Kubernetes architecture, services, ingress,
                    namespaces and Helm.
                </p>
            </div>

            <div class="skill-card">
                <h3>⚙️ Automation</h3>
                <p>
                    Ansible playbooks, roles, modules and
                    infrastructure configuration.
                </p>
            </div>

            <div class="skill-card">
                <h3>📊 Monitoring</h3>
                <p>
                    Prometheus, Node Exporter, Alertmanager,
                    Grafana, metrics and dashboards.
                </p>
            </div>

            <div class="skill-card">
                <h3>🚀 CI/CD</h3>
                <p>
                    Azure DevOps, GitHub Actions, YAML and
                    automated infrastructure deployment.
                </p>
            </div>

            <div class="skill-card">
                <h3>🔐 Security & Identity</h3>
                <p>
                    NSG, ASG, Bastion, identity management and
                    Microsoft Entra ID.
                </p>
            </div>

            <div class="skill-card">
                <h3>🔄 Disaster Recovery</h3>
                <p>
                    Backup, restore, site recovery, geo-replication,
                    failover and DR drills.
                </p>
            </div>

        </div>

    </div>

</section>


<!-- =========================================
     LEARNING PATH
========================================= -->

<section>

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                Learning Path
            </div>

            <h2>📈 Cloud & DevOps Skill Progression</h2>

        </div>


        <div class="learning-path">

            <div class="path-item">
                <div class="path-number">01</div>
                <strong>☁️ Cloud Computing</strong>
                <span>Fundamentals</span>
            </div>

            <div class="path-item">
                <div class="path-number">02</div>
                <strong>🌐 Networking</strong>
                <span>Infrastructure</span>
            </div>

            <div class="path-item">
                <div class="path-number">03</div>
                <strong>🔷 Microsoft Azure</strong>
                <span>Cloud Platform</span>
            </div>

            <div class="path-item">
                <div class="path-number">04</div>
                <strong>🏗️ Terraform</strong>
                <span>Infrastructure as Code</span>
            </div>

            <div class="path-item">
                <div class="path-number">05</div>
                <strong>🔀 Git & GitHub</strong>
                <span>Version Control</span>
            </div>

            <div class="path-item">
                <div class="path-number">06</div>
                <strong>🐳 Docker</strong>
                <span>Containerization</span>
            </div>

            <div class="path-item">
                <div class="path-number">07</div>
                <strong>☸️ Kubernetes</strong>
                <span>Orchestration</span>
            </div>

            <div class="path-item">
                <div class="path-number">08</div>
                <strong>⚙️ Ansible</strong>
                <span>Automation</span>
            </div>

            <div class="path-item">
                <div class="path-number">09</div>
                <strong>📊 Prometheus & Grafana</strong>
                <span>Monitoring</span>
            </div>

            <div class="path-item">
                <div class="path-number">10</div>
                <strong>🚀 Azure DevOps & GitHub Actions</strong>
                <span>CI/CD</span>
            </div>

        </div>

    </div>

</section>


<!-- =========================================
     CAREER ROLES
========================================= -->

<section id="careers">

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                Career Opportunities
            </div>

            <h2>💼 Roles You Can Target</h2>

            <p>
                This combination of skills provides a foundation for
                multiple Cloud, Infrastructure, Networking, Systems
                and DevOps career paths.
            </p>

        </div>


        <div class="career-grid">

            <div class="career-card">

                <h3>☁️ Cloud Roles</h3>

                <ul>
                    <li>Cloud Engineer</li>
                    <li>Azure Cloud Engineer</li>
                    <li>Cloud Infrastructure Engineer</li>
                    <li>Cloud Support Engineer</li>
                    <li>Cloud Administrator</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>🚀 DevOps Roles</h3>

                <ul>
                    <li>DevOps Engineer</li>
                    <li>Junior DevOps Engineer</li>
                    <li>DevOps Support Engineer</li>
                    <li>CI/CD Engineer</li>
                    <li>Build & Release Engineer</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>🏗️ Infrastructure</h3>

                <ul>
                    <li>Infrastructure Engineer</li>
                    <li>Infrastructure Automation Engineer</li>
                    <li>Terraform Engineer</li>
                    <li>IaC Engineer</li>
                    <li>Configuration Management Engineer</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>☸️ Platform & Containers</h3>

                <ul>
                    <li>Kubernetes Engineer</li>
                    <li>Container Engineer</li>
                    <li>Platform Engineer</li>
                    <li>Cloud Platform Engineer</li>
                    <li>Junior SRE</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>🌐 Networking</h3>

                <ul>
                    <li>Network Administrator</li>
                    <li>Network Support Engineer</li>
                    <li>Cloud Network Engineer</li>
                    <li>Cloud Network Administrator</li>
                    <li>Network Infrastructure Engineer</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>🖥️ System Administration</h3>

                <ul>
                    <li>System Administrator</li>
                    <li>Linux Administrator</li>
                    <li>Linux System Administrator</li>
                    <li>Windows Administrator</li>
                    <li>Windows System Administrator</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>💾 Storage & Database</h3>

                <ul>
                    <li>Storage Administrator</li>
                    <li>Cloud Storage Engineer</li>
                    <li>Database Administrator</li>
                    <li>Cloud Database Support Engineer</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>📊 Monitoring</h3>

                <ul>
                    <li>Monitoring Engineer</li>
                    <li>Cloud Monitoring Engineer</li>
                    <li>Observability Engineer</li>
                    <li>Infrastructure Monitoring Engineer</li>
                    <li>Junior SRE</li>
                </ul>

            </div>


            <div class="career-card">

                <h3>🔧 Support & Operations</h3>

                <ul>
                    <li>Cloud Support Engineer</li>
                    <li>Infrastructure Support Engineer</li>
                    <li>Technical Support Engineer</li>
                    <li>Cloud Operations Engineer</li>
                </ul>

            </div>

        </div>

    </div>

</section>


<!-- =========================================
     COMBINATION OF ROLES
========================================= -->

<section>

    <div class="container">

        <div class="section-header">

            <div class="section-number">
                Infrastructure Domains
            </div>

            <h2>👥 Combination of Roles</h2>

            <p>
                Cloud and DevOps engineering brings together knowledge
                from multiple infrastructure and operations domains.
            </p>

        </div>


        <div class="role-grid">

            <div class="role">🏢 Data Center Engineer</div>

            <div class="role">🌐 Network Administrator</div>

            <div class="role">💾 Storage Administrator</div>

            <div class="role">🖥️ System Administrator</div>

            <div class="role">🖥️ VMware Administrator</div>

            <div class="role">🪟 Windows Administrator</div>

            <div class="role">🐧 Linux Administrator</div>

            <div class="role">🗄️ Database Administrator</div>

            <div class="role">☁️ Cloud Engineer</div>

            <div class="role">🏗️ Infrastructure Engineer</div>

            <div class="role">🚀 DevOps Engineer</div>

            <div class="role">📊 Monitoring Engineer</div>

        </div>

    </div>

</section>


<!-- =========================================
     OBJECTIVE
========================================= -->

<section class="objective">

    <div class="container">

        <div class="section-number">
            Objective
        </div>

        <h2>
            🎯 Build. Automate. Monitor. Grow.
        </h2>

        <p>
            Build strong practical knowledge of Cloud, Infrastructure,
            Networking, Automation, Containers, Kubernetes, Monitoring
            and DevOps technologies while developing the technical
            foundation required for modern Cloud & DevOps engineering roles.
        </p>

    </div>

</section>


<!-- =========================================
     CREATED BY
========================================= -->

<section class="creator">

    <div class="container">

        <div class="creator-badge">
            CREATED & MAINTAINED BY
        </div>

        <h2>Saibaba Kola</h2>

        <h3>Cloud & DevOps Engineer</h3>

        <p>
            This learning content has been created, organized,
            practiced and maintained by me as part of my continuous
            learning journey in Cloud Computing, Infrastructure,
            Automation, Monitoring and DevOps.
        </p>


        <div class="creator-stack">

            <span>☁️ Azure</span>
            <span>🏗️ Terraform</span>
            <span>🔀 Git</span>
            <span>🌍 GitHub</span>
            <span>🐳 Docker</span>
            <span>☸️ Kubernetes</span>
            <span>⚙️ Ansible</span>
            <span>📊 Prometheus</span>
            <span>📈 Grafana</span>
            <span>🔷 Azure DevOps</span>
            <span>🚀 GitHub Actions</span>

        </div>

    </div>

</section>


<!-- =========================================
     FOOTER
========================================= -->

<footer>

    <div class="container">

        <p>
            <strong>☁️ Cloud & DevOps Engineering</strong>
            <br>
            Learn • Practice • Build • Automate • Monitor • Grow 🚀
        </p>

        <p style="margin-top: 8px;">
            © 2026 Saibaba Kola. All rights reserved.
        </p>

    </div>

</footer>


</body>
</html>
