<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Drone Command Center</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- SIDEBAR -->
    <aside class="sidebar">

        <div class="logo">
            🚁 <span>DRONE</span>
        </div>

        <nav>
            <a href="#" class="active">📊 Dashboard</a>
            <a href="#">🎥 Live Camera</a>
            <a href="#">📡 Telemetry</a>
            <a href="#">🛰️ GPS</a>
            <a href="#">📁 Flight History</a>
            <a href="#">⚙️ Settings</a>
        </nav>

        <div class="connection">
            <span class="online-dot"></span>
            System Online
        </div>

    </aside>


    <!-- MAIN CONTENT -->
    <main class="main">

        <!-- TOP BAR -->
        <header class="topbar">

            <div>
                <p class="small-title">DRONE CONTROL SYSTEM</p>
                <h1>Command Center</h1>
            </div>

            <div class="top-right">
                <span class="status">
                    <span class="online-dot"></span>
                    Connected
                </span>

                <div class="profile">
                    👤
                </div>
            </div>

        </header>


        <!-- STATUS CARDS -->
        <section class="stats-grid">

            <div class="card stat-card">
                <div class="icon">🔋</div>
                <div>
                    <p>Battery</p>
                    <h2 id="battery">82%</h2>
                    <span class="good">● Healthy</span>
                </div>
            </div>

            <div class="card stat-card">
                <div class="icon">📶</div>
                <div>
                    <p>Signal</p>
                    <h2 id="signal">94%</h2>
                    <span class="good">● Excellent</span>
                </div>
            </div>

            <div class="card stat-card">
                <div class="icon">📏</div>
                <div>
                    <p>Altitude</p>
                    <h2><span id="altitude">42</span> m</h2>
                    <span>Above ground</span>
                </div>
            </div>

            <div class="card stat-card">
                <div class="icon">🚀</div>
                <div>
                    <p>Speed</p>
                    <h2><span id="speed">18</span> km/h</h2>
                    <span>Current speed</span>
                </div>
            </div>

        </section>


        <!-- CAMERA + SYSTEM -->
        <section class="main-grid">

            <!-- CAMERA -->
            <div class="card camera-card">

                <div class="card-header">
                    <div>
                        <p class="small-title">LIVE FEED</p>
                        <h2>Drone Camera</h2>
                    </div>

                    <span class="live">
                        <span></span> LIVE
                    </span>
                </div>

                <div class="camera">

                    <div class="camera-overlay">
                        <span>REC</span>
                        <span id="cameraTime">00:12:43</span>
                    </div>

                    <div class="camera-center">
                        <div class="crosshair">+</div>
                        <p>ESP32-CAM</p>
                    </div>

                    <div class="camera-info">
                        <span>1080p</span>
                        <span>30 FPS</span>
                        <span>Wi-Fi</span>
                    </div>

                </div>

            </div>


            <!-- SYSTEM STATUS -->
            <div class="card system-card">

                <div class="card-header">
                    <div>
                        <p class="small-title">HARDWARE</p>
                        <h2>System Status</h2>
                    </div>
                </div>

                <div class="hardware">

                    <div class="hardware-item">
                        <div>
                            <strong>ESP32-CAM</strong>
                            <p>Camera module</p>
                        </div>

                        <span class="badge online">ONLINE</span>
                    </div>

                    <div class="hardware-item">
                        <div>
                            <strong>ESP32-S3</strong>
                            <p>Receiver / controller</p>
                        </div>

                        <span class="badge online">ONLINE</span>
                    </div>

                    <div class="hardware-item">
                        <div>
                            <strong>MicroSD Card</strong>
                            <p>Storage system</p>
                        </div>

                        <span class="badge online">READY</span>
                    </div>

                    <div class="hardware-item">
                        <div>
                            <strong>GPS Module</strong>
                            <p>Location tracking</p>
                        </div>

                        <span class="badge online">LOCKED</span>
                    </div>

                </div>

            </div>

        </section>


        <!-- TELEMETRY -->
        <section class="bottom-grid">

            <div class="card telemetry-card">

                <div class="card-header">

                    <div>
                        <p class="small-title">REAL-TIME DATA</p>
                        <h2>Telemetry</h2>
                    </div>

                    <span class="time-label">LIVE</span>

                </div>

                <div class="chart">

                    <div class="chart-line"></div>

                    <div class="chart-labels">
                        <span>10:00</span>
                        <span>10:05</span>
                        <span>10:10</span>
                        <span>10:15</span>
                        <span>10:20</span>
                    </div>

                </div>

            </div>


            <!-- FLIGHT INFORMATION -->
            <div class="card flight-card">

                <div class="card-header">
                    <div>
                        <p class="small-title">CURRENT FLIGHT</p>
                        <h2>Flight Information</h2>
                    </div>
                </div>

                <div class="flight-data">

                    <div>
                        <span>Flight Time</span>
                        <strong id="flightTime">12:43</strong>
                    </div>

                    <div>
                        <span>Distance</span>
                        <strong id="distance">486 m</strong>
                    </div>

                    <div>
                        <span>GPS Satellites</span>
                        <strong>14</strong>
                    </div>

                    <div>
                        <span>Heading</span>
                        <strong id="heading">128°</strong>
                    </div>

                </div>

            </div>

        </section>


        <!-- FOOTER -->
        <footer>
            <span>Tanjiro Drone Command Center</span>
            <span>ESP32 • ESP32-S3 • ESP32-CAM</span>
        </footer>

    </main>


    <script src="script.js"></script>

</body>
</html>