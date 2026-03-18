<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SFS Realistic Simulator - AP CSP Project</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Courier New', monospace;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 100%);
            color: #00ff00;
            padding: 20px;
            min-height: 100vh;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        h1 {
            text-align: center;
            color: #00ff00;
            text-shadow: 0 0 10px #00ff00;
            margin-bottom: 10px;
            font-size: 2em;
        }

        .subtitle {
            text-align: center;
            color: #888;
            margin-bottom: 30px;
            font-size: 0.9em;
        }

        .config-panel {
            background: rgba(0, 255, 0, 0.05);
            border: 2px solid #00ff00;
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 20px;
        }

        .destination-select {
            margin-bottom: 20px;
        }

        .destination-buttons {
            display: flex;
            gap: 10px;
            margin-top: 10px;
        }

        .dest-btn {
            flex: 1;
            padding: 15px;
            background: rgba(0, 255, 0, 0.1);
            border: 2px solid #00ff00;
            color: #00ff00;
            cursor: pointer;
            font-family: 'Courier New', monospace;
            font-size: 1em;
            transition: all 0.3s;
        }

        .dest-btn:hover {
            background: rgba(0, 255, 0, 0.2);
            box-shadow: 0 0 20px rgba(0, 255, 0, 0.3);
        }

        .dest-btn.active {
            background: rgba(0, 255, 0, 0.3);
            box-shadow: 0 0 20px rgba(0, 255, 0, 0.5);
        }

        .input-group {
            margin-bottom: 15px;
        }

        label {
            display: block;
            margin-bottom: 5px;
            color: #00ff00;
        }

        input[type="number"] {
            width: 100%;
            padding: 8px;
            background: rgba(0, 0, 0, 0.5);
            border: 1px solid #00ff00;
            color: #00ff00;
            font-family: 'Courier New', monospace;
            font-size: 1em;
        }

        input[type="number"]:focus {
            outline: none;
            box-shadow: 0 0 10px rgba(0, 255, 0, 0.5);
        }

        .stage-config {
            background: rgba(0, 255, 0, 0.03);
            border: 1px solid #00ff00;
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 5px;
        }

        .stage-header {
            color: #00ff00;
            font-weight: bold;
            margin-bottom: 10px;
            text-transform: uppercase;
        }

        .stage-inputs {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 10px;
        }

        button {
            padding: 12px 30px;
            background: rgba(0, 255, 0, 0.2);
            border: 2px solid #00ff00;
            color: #00ff00;
            cursor: pointer;
            font-family: 'Courier New', monospace;
            font-size: 1em;
            margin: 5px;
            transition: all 0.3s;
        }

        button:hover {
            background: rgba(0, 255, 0, 0.3);
            box-shadow: 0 0 15px rgba(0, 255, 0, 0.5);
        }

        button:disabled {
            opacity: 0.5;
            cursor: not-allowed;
        }

        .output-panel {
            background: rgba(0, 0, 0, 0.8);
            border: 2px solid #00ff00;
            border-radius: 10px;
            padding: 20px;
            margin-top: 20px;
            max-height: 600px;
            overflow-y: auto;
        }

        .log-entry {
            white-space: pre;
            font-size: 0.85em;
            line-height: 1.4;
        }

        .event {
            color: #ffff00;
            font-weight: bold;
        }

        .success {
            color: #00ff00;
            font-weight: bold;
        }

        .failure {
            color: #ff0000;
            font-weight: bold;
        }

        .controls {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }

        .status-bar {
            background: rgba(0, 255, 0, 0.1);
            border: 1px solid #00ff00;
            padding: 10px;
            margin-top: 10px;
            border-radius: 5px;
            display: none;
        }

        .progress {
            color: #ffff00;
        }

        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0.3; }
        }

        .running {
            animation: blink 1s infinite;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🚀 SPACEFLIGHT SIMULATOR - REALISTIC MISSION CALCULATOR</h1>
        <p class="subtitle">AP Computer Science Principles - Creative Performance Task</p>
        
        <div class="config-panel">
            <div class="destination-select">
                <label>Select Destination:</label>
                <div class="destination-buttons">
                    <button class="dest-btn active" onclick="selectDestination('Venus')">
                        🌋 VENUS<br>
                        <small>Dense Atmosphere - Extreme Heating</small>
                    </button>
                    <button class="dest-btn" onclick="selectDestination('Mars')">
                        🔴 MARS<br>
                        <small>Thin Atmosphere - Lower Heating</small>
                    </button>
                </div>
            </div>

            <div class="input-group">
                <label>Number of Stages:</label>
                <input type="number" id="numStages" value="1" min="1" max="5" onchange="generateStageInputs()">
            </div>

            <div id="stageInputs"></div>

            <div class="input-group">
                <label>Number of Parachutes:</label>
                <input type="number" id="numChutes" value="20" min="0" max="100">
            </div>

            <div class="controls">
                <button onclick="startSimulation()" id="startBtn">▶ START SIMULATION</button>
                <button onclick="stopSimulation()" id="stopBtn" disabled>⏹ STOP</button>
                <button onclick="clearOutput()">🗑 CLEAR LOG</button>
            </div>

            <div class="status-bar" id="statusBar">
                <span class="progress" id="statusText">Initializing...</span>
            </div>
        </div>

        <div class="output-panel" id="output"></div>
    </div>

    <script>
        let selectedDestination = 'Venus';
        let simulationRunning = false;
        let simulationInterval = null;

        const PLANETS = {
            "Venus": {
                radius: 6051800,
                mass: 4.867e24,
                atmo: 150000,
                H: 15900,
                rho0: 67.0
            },
            "Mars": {
                radius: 3389500,
                mass: 6.39e23,
                atmo: 125000,
                H: 11100,
                rho0: 0.020
            }
        };

        const G = 6.67430e-11;
        const M_EARTH = 5.972e24;
        const G0_EARTH = 9.80665;
        const TIME_STEP = 0.1;
        const EARTH_SCALE_HEIGHT = 3200;
        const EARTH_RHO0 = 1.225;
        const HEAT_SHIELD_LIMIT = 6180.0;

        function selectDestination(dest) {
            selectedDestination = dest;
            document.querySelectorAll('.dest-btn').forEach(btn => btn.classList.remove('active'));
            event.target.closest('.dest-btn').classList.add('active');
        }

        function generateStageInputs() {
            const numStages = parseInt(document.getElementById('numStages').value);
            const container = document.getElementById('stageInputs');
            container.innerHTML = '';

            for (let i = 1; i <= numStages; i++) {
                const stageDiv = document.createElement('div');
                stageDiv.className = 'stage-config';
                stageDiv.innerHTML = `
                    <div class="stage-header">Stage ${i}</div>
                    <div class="stage-inputs">
                        <div class="input-group">
                            <label>Wet Mass (t):</label>
                            <input type="number" id="s${i}_wet" value="10000" step="0.1">
                        </div>
                        <div class="input-group">
                            <label>Dry Mass (t):</label>
                            <input type="number" id="s${i}_dry" value="1" step="0.1">
                        </div>
                        <div class="input-group">
                            <label>Thrust (tf):</label>
                            <input type="number" id="s${i}_thrust" value="30000" step="1">
                        </div>
                        <div class="input-group">
                            <label>ISP (s):</label>
                            <input type="number" id="s${i}_isp" value="1145143" step="1">
                        </div>
                        <div class="input-group">
                            <label>CD:</label>
                            <input type="number" id="s${i}_cd" value="0.6" step="0.01">
                        </div>
                        <div class="input-group">
                            <label>Area (m²):</label>
                            <input type="number" id="s${i}_area" value="20" step="0.1">
                        </div>
                    </div>
                `;
                container.appendChild(stageDiv);
            }
        }

        function log(message, className = '') {
            const output = document.getElementById('output');
            const entry = document.createElement('div');
            entry.className = `log-entry ${className}`;
            entry.textContent = message;
            output.appendChild(entry);
            output.scrollTop = output.scrollHeight;
        }

        function clearOutput() {
            document.getElementById('output').innerHTML = '';
        }

        function stopSimulation() {
            simulationRunning = false;
            document.getElementById('startBtn').disabled = false;
            document.getElementById('stopBtn').disabled = true;
            document.getElementById('statusBar').style.display = 'none';
        }

        async function startSimulation() {
            clearOutput();
            document.getElementById('startBtn').disabled = true;
            document.getElementById('stopBtn').disabled = false;
            document.getElementById('statusBar').style.display = 'block';
            
            simulationRunning = true;

            // Get configuration
            const numStages = parseInt(document.getElementById('numStages').value);
            const numChutes = parseInt(document.getElementById('numChutes').value);
            const dest = PLANETS[selectedDestination];

            // Build stages
            const stages = [];
            for (let i = 1; i <= numStages; i++) {
                const wet = parseFloat(document.getElementById(`s${i}_wet`).value);
                const dry = parseFloat(document.getElementById(`s${i}_dry`).value);
                const thrust = parseFloat(document.getElementById(`s${i}_thrust`).value);
                const isp = parseFloat(document.getElementById(`s${i}_isp`).value);
                const cd = parseFloat(document.getElementById(`s${i}_cd`).value);
                const area = parseFloat(document.getElementById(`s${i}_area`).value);

                stages.push({
                    num: i,
                    total_mass_at_start: wet * 1000,
                    total_mass_at_end: dry * 1000,
                    fuel_mass: (wet - dry) * 1000,
                    fuel_curr: (wet - dry) * 1000,
                    thrust: thrust * 1000 * G0_EARTH,
                    isp: isp,
                    cd: cd,
                    area: area,
                    flow_rate: (thrust * 1000) / (isp > 0 ? isp : 1)
                });
            }

            log(`🚀 SFS REALISTIC SIM: EARTH -> ${selectedDestination.toUpperCase()}`);
            log('─'.repeat(190));
            log(`${'Time'.padEnd(10)}${'Alt(km)'.padEnd(10)}${'Fuel%'.padEnd(9)}${'Acc(g)'.padEnd(9)}${'Vel(m/s)'.padEnd(10)}${'V-Horiz'.padEnd(10)}${'V-Vert'.padEnd(10)}${'Drag(kN)'.padEnd(11)}${'Grav(kN)'.padEnd(11)}${'Temp(C)'.padEnd(10)}${'Pitch'.padEnd(9)}Phase`);
            log('─'.repeat(190));

            // Initialize state
            let time = 0.0, alt = 0.0, vel_v = 0.0, vel_h = 0.0, curr_idx = 0;
            let shield_temp = 20.0, chute_state = "STOWED";
            let mission_success = false, failure_reason = "Unknown";
            let mission_phase = "VERTICAL_ASCENT";
            
            const v_final_target = selectedDestination === "Mars" ? 9500 : 11500;
            const entry_altitude = selectedDestination === "Mars" ? 130000 : 155000;
            
            let transfer_complete_vel_h = 0.0, transfer_time = 0.0;
            let logCounter = 0;

            // Run simulation in chunks to prevent freezing
            const runChunk = () => {
                if (!simulationRunning) return;

                const chunkSize = 100; // Process 100 timesteps at once
                for (let i = 0; i < chunkSize && time < 600000 && simulationRunning; i++) {
                    const s = stages[curr_idx];
                    const current_total_mass = s.total_mass_at_end + s.fuel_curr;

                    if (current_total_mass <= 0) {
                        failure_reason = "Structural Failure (Zero Mass)";
                        break;
                    }

                    // Environment
                    const r_p = mission_phase !== "RE_ENTRY" ? 6371000 : dest.radius;
                    const m_p = mission_phase !== "RE_ENTRY" ? M_EARTH : dest.mass;
                    const r = r_p + alt;
                    const g_accel = (G * m_p) / (r * r);

                    const h_s = mission_phase !== "RE_ENTRY" ? EARTH_SCALE_HEIGHT : dest.H;
                    const rho0 = mission_phase !== "RE_ENTRY" ? EARTH_RHO0 : dest.rho0;
                    const atmo_limit = mission_phase !== "RE_ENTRY" ? 100000 : dest.atmo;
                    const rho = alt < atmo_limit ? rho0 * Math.exp(-alt / h_s) : 0;

                    const v_tot = Math.sqrt(vel_v * vel_v + vel_h * vel_h);

                    // Guidance
                    let pitch_deg = 0;
                    if (mission_phase === "VERTICAL_ASCENT") {
                        if ((alt + (vel_v * vel_v) / (2 * g_accel)) >= 125000) {
                            mission_phase = "ORBITAL_INSERTION";
                        }
                        pitch_deg = 0;
                    } else if (mission_phase === "ORBITAL_INSERTION") {
                        if (vel_h >= 7800) mission_phase = "TRANSFER_BURN";
                        pitch_deg = alt < 100000 ? 85 : (alt < 120000 ? 88 : 90);
                    } else if (mission_phase === "TRANSFER_BURN") {
                        pitch_deg = 90;
                    } else if (mission_phase === "RE_ENTRY") {
                        pitch_deg = Math.atan2(vel_v, vel_h) * 180 / Math.PI;
                    }

                    const pitch_rad = pitch_deg * Math.PI / 180;

                    // Physics
                    const thrust_active = (mission_phase !== "RE_ENTRY" && s.fuel_curr > 0) ? s.thrust : 0;
                    
                    let area_eff = s.area;
                    if (chute_state === "HALF") area_eff += numChutes * 20;
                    if (chute_state === "FULL") area_eff += numChutes * 100;

                    const f_drag_mag = 0.5 * rho * (v_tot * v_tot) * s.cd * area_eff;
                    const f_drag_x = v_tot > 0 ? -f_drag_mag * (vel_h / v_tot) : 0;
                    const f_drag_y = v_tot > 0 ? -f_drag_mag * (vel_v / v_tot) : 0;

                    const acc_x = (thrust_active * Math.sin(pitch_rad) + f_drag_x) / current_total_mass;
                    const acc_y = (thrust_active * Math.cos(pitch_rad) - (current_total_mass * g_accel) + f_drag_y) / current_total_mass;

                    vel_h += acc_x * TIME_STEP;
                    vel_v += acc_y * TIME_STEP;
                    alt += vel_v * TIME_STEP;

                    // Heat shield
                    if (mission_phase === "RE_ENTRY") {
                        const heating_rate = 0.00001 * rho * (v_tot ** 3) / 1000;
                        const cooling_rate = shield_temp > 20 ? 0.000000005 * (shield_temp ** 4) : 0;
                        shield_temp = Math.max(20, shield_temp + (heating_rate - cooling_rate) * TIME_STEP);

                        if (shield_temp > HEAT_SHIELD_LIMIT) {
                            failure_reason = `Heat Shield Failure (${shield_temp.toFixed(1)}°C)`;
                            simulationRunning = false;
                            break;
                        }
                    }

                    // Parachutes
                    if (mission_phase === "RE_ENTRY" && chute_state === "STOWED") {
                        if (alt < 2500 && vel_v < 0) {
                            if (v_tot < 250) {
                                chute_state = "HALF";
                                log(`[${time.toFixed(1)}s] EVENT: PARACHUTES HALF-DEPLOYED`, 'event');
                            } else if (chute_state !== "FAILED") {
                                chute_state = "FAILED";
                                log(`[${time.toFixed(1)}s] ALERT: CHUTES SNAPPED (VEL > 250m/s)`, 'event');
                            }
                        }
                    }
                    if (mission_phase === "RE_ENTRY" && chute_state === "HALF" && alt < 500) {
                        chute_state = "FULL";
                        log(`[${time.toFixed(1)}s] EVENT: PARACHUTES FULL-DEPLOYED`, 'event');
                    }

                    // Transfer burn completion
                    if (mission_phase === "TRANSFER_BURN" && vel_h >= v_final_target) {
                        transfer_complete_vel_h = vel_h;
                        transfer_time = time;
                        mission_phase = "RE_ENTRY";
                        time = 250000.0;
                        alt = entry_altitude;

                        const entry_vel = selectedDestination === "Mars" ? 
                            Math.min(transfer_complete_vel_h * 0.75, 6500) : 
                            Math.min(transfer_complete_vel_h * 0.62, 7200);
                        const entry_angle = selectedDestination === "Mars" ? -3 * Math.PI / 180 : -5 * Math.PI / 180;

                        vel_h = entry_vel * Math.cos(entry_angle);
                        vel_v = entry_vel * Math.sin(entry_angle);
                        shield_temp = 20.0;

                        log(`\n[${transfer_time.toFixed(1)}s] TRANSFER COMPLETE (Vh=${transfer_complete_vel_h.toFixed(1)} m/s)`, 'event');
                        log(`[${time.toFixed(1)}s] ENTERING ${selectedDestination.toUpperCase()} ATMOSPHERE`, 'event');
                        log('─'.repeat(190));
                        continue;
                    }

                    // Landing check
                    if (mission_phase === "RE_ENTRY" && alt <= 0) {
                        if (Math.abs(vel_v) < 50.0) {
                            mission_success = true;
                            failure_reason = "Soft Landing";
                        } else {
                            failure_reason = `High Velocity Impact (${Math.abs(vel_v).toFixed(1)} m/s)`;
                        }
                        simulationRunning = false;
                        break;
                    }

                    // Crash during ascent
                    if (mission_phase !== "RE_ENTRY" && alt < 0) {
                        failure_reason = "Crashed During Ascent";
                        simulationRunning = false;
                        break;
                    }

                    // Fuel consumption & stage separation
                    if (thrust_active > 0) {
                        s.fuel_curr = Math.max(0, s.fuel_curr - s.flow_rate * TIME_STEP);
                    }

                    if (s.fuel_curr <= 0 && curr_idx < stages.length - 1) {
                        log(`[${time.toFixed(1)}s] EVENT: STAGE ${s.num} SEPARATION`, 'event');
                        curr_idx++;
                    }

                    // Logging
                    const log_interval = mission_phase === "RE_ENTRY" ? 5 : 
                                       mission_phase === "TRANSFER_BURN" ? 40 : 10;
                    
                    if (Math.floor(time / TIME_STEP) % (log_interval / TIME_STEP) === 0) {
                        const fuel_p = s.fuel_mass > 0 ? (s.fuel_curr / s.fuel_mass) * 100 : 0;
                        const total_acc_g = Math.sqrt(acc_x * acc_x + acc_y * acc_y) / 9.81;
                        const drag_kn = f_drag_mag / 1000;
                        const grav_kn = (current_total_mass * g_accel) / 1000;
                        const temp_disp = mission_phase === "RE_ENTRY" ? shield_temp.toFixed(1) : "-";

                        log(`${time.toFixed(1).padEnd(10)}${(alt/1000).toFixed(2).padEnd(10)}${fuel_p.toFixed(1).padEnd(9)}${total_acc_g.toFixed(2).padEnd(9)}${v_tot.toFixed(1).padEnd(10)}${vel_h.toFixed(1).padEnd(10)}${vel_v.toFixed(1).padEnd(10)}${drag_kn.toFixed(1).padEnd(11)}${grav_kn.toFixed(1).padEnd(11)}${temp_disp.padEnd(10)}${pitch_deg.toFixed(1).padEnd(9)}${mission_phase}`);
                    }

                    time += TIME_STEP;
                    
                    // Update status
                    if (logCounter++ % 50 === 0) {
                        document.getElementById('statusText').textContent = 
                            `Phase: ${mission_phase} | Time: ${time.toFixed(1)}s | Alt: ${(alt/1000).toFixed(1)}km | Vel: ${v_tot.toFixed(0)} m/s`;
                    }
                }

                if (simulationRunning && time < 600000) {
                    setTimeout(runChunk, 0);
                } else {
                    // Mission complete
                    log('\n' + '='.repeat(60));
                    log(`MISSION STATUS: ${mission_success ? '✅ SUCCESS' : '❌ FAILED'}`, mission_success ? 'success' : 'failure');
                    log(`REASON: ${failure_reason}`);
                    log(`Impact Velocity: ${Math.abs(vel_v).toFixed(2)} m/s`);
                    if (mission_phase === "RE_ENTRY") {
                        log(`Final Heat Shield Temp: ${shield_temp.toFixed(1)}°C`);
                    }
                    log('='.repeat(60));
                    stopSimulation();
                }
            };

            runChunk();
        }

        // Initialize on load
        generateStageInputs();
    </script>
</body>
</html>
