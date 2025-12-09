<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>1120 서버 KvK 일정표</title>
    <style>
        /* RoK 스타일 디자인 */
        :root {
            --bg-color: #1a1a2e;
            --card-bg: #16213e;
            --text-color: #e94560;
            --highlight: #fcdab7;
        }
        body {
            font-family: 'Noto Sans KR', sans-serif;
            background-color: var(--bg-color);
            color: white;
            margin: 0;
            padding: 20px;
            text-align: center;
        }
        h1 { color: var(--highlight); margin-bottom: 10px; }
        .server-info { font-size: 0.9em; color: #888; margin-bottom: 30px; }
        
        .timeline {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .event-card {
            background-color: var(--card-bg);
            border: 1px solid #2a2a4e;
            border-radius: 10px;
            padding: 15px;
            margin-bottom: 15px;
            text-align: left;
            position: relative;
            transition: transform 0.2s;
        }
        .event-card.active { border: 2px solid var(--text-color); box-shadow: 0 0 10px rgba(233, 69, 96, 0.5); }
        .event-card.past { opacity: 0.5; }
        
        .event-title { font-size: 1.2em; font-weight: bold; color: var(--highlight); }
        .event-date { font-size: 0.9em; color: #ccc; margin-top: 5px; }
        .d-day {
            position: absolute;
            right: 15px;
            top: 50%;
            transform: translateY(-50%);
            font-weight: bold;
            font-size: 1.2em;
            color: var(--text-color);
        }
        .status-badge {
            display: inline-block;
            padding: 2px 8px;
            border-radius: 4px;
            font-size: 0.7em;
            margin-bottom: 5px;
            font-weight: bold;
        }
        .status-future { background-color: #444; color: #ddd; }
        .status-active { background-color: var(--text-color); color: white; }
        .status-done { background-color: #2e7d32; color: white; }

    </style>
</head>
<body>

    <h1>⚔️ 1120 서버 KvK 일정 ⚔️</h1>
    <div class="server-info">Time Zone: Korea Standard Time (KST)</div>

    <div class="timeline" id="timeline-container">
        </div>

    <script>
        // ==========================================
        // 👇 여기 아래 날짜들만 수정하시면 됩니다! 👇
        // ==========================================
        const kvkEvents = [
            { title: "잃어버린 왕국 오픈 (진입)", date: "2025-12-09T09:00:00" },
            { title: "4레벨 관문 오픈 (준결승)", date: "2025-12-13T12:00:00" },
            { title: "5레벨 관문 오픈", date: "2025-12-27T12:00:00" },
            { title: "킹스랜드 (7레벨 관문)", date: "2026-01-08T12:00:00" },
            { title: "KvK 시즌 종료", date: "2026-01-28T09:00:00" }
        ];
        // ==========================================

        const container = document.getElementById('timeline-container');

        function updateSchedule() {
            container.innerHTML = '';
            const now = new Date();

            kvkEvents.forEach(event => {
                const eventDate = new Date(event.date);
                const diffMS = eventDate - now;
                const diffDays = Math.ceil(diffMS / (1000 * 60 * 60 * 24));
                
                let dDayText = "";
                let statusClass = "";
                let cardClass = "event-card";
                let badgeText = "";

                if (diffMS > 0) {
                    // 미래
                    dDayText = `D-${diffDays}`;
                    statusClass = "status-future";
                    badgeText = "예정";
                } else if (diffDays === 0 || (diffMS < 0 && diffMS > -86400000)) { 
                    // 당일 (또는 24시간 내)
                    dDayText = "D-Day!";
                    statusClass = "status-active";
                    cardClass += " active";
                    badgeText = "진행중";
                } else {
                    // 과거
                    dDayText = "종료";
                    statusClass = "status-done";
                    cardClass += " past";
                    badgeText = "완료";
                }

                // 날짜 포맷팅 (월/일 시:분)
                const dateStr = eventDate.toLocaleString('ko-KR', { month: 'long', day: 'numeric', hour: '2-digit', minute: '2-digit', hour12: false });

                const html = `
                    <div class="${cardClass}">
                        <span class="status-badge ${statusClass}">${badgeText}</span>
                        <div class="event-title">${event.title}</div>
                        <div class="event-date">📅 ${dateStr}</div>
                        <div class="d-day">${dDayText}</div>
                    </div>
                `;
                container.innerHTML += html;
            });
        }

        updateSchedule();
        // 1분마다 새로고침
        setInterval(updateSchedule, 60000);
    </script>
</body>
</html>
