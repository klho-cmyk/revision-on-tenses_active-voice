<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tense Master: Speed Quiz</title>
    <style>
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --neon-blue: #38bdf8;
            --neon-pink: #f472b6;
            --neon-green: #4ade80;
            --text-main: #f8fafc;
            --text-dim: #94a3b8;
            --feedback-bg: #334155;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden;
        }

        #game-container {
            width: 95%;
            max-width: 700px;
            background: var(--card-bg);
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 0 20px rgba(56, 189, 248, 0.2);
            border: 1px solid rgba(56, 189, 248, 0.3);
            text-align: center;
            position: relative;
            max-height: 95vh;
            overflow-y: auto;
        }

        h1 {
            color: var(--neon-blue);
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 1rem;
            text-shadow: 0 0 10px var(--neon-blue);
        }

        .stats-bar {
            display: flex;
            justify-content: space-between;
            margin-bottom: 1rem;
            font-weight: bold;
        }

        #timer-container {
            width: 100%;
            height: 10px;
            background: #334155;
            border-radius: 5px;
            margin-bottom: 1.5rem;
            overflow: hidden;
        }

        #timer-bar {
            height: 100%;
            width: 100%;
            background: linear-gradient(to right, var(--neon-green), var(--neon-pink));
            transition: width 0.1s linear;
        }

        .question-box {
            font-size: 1.2rem;
            margin-bottom: 1.5rem;
            min-height: 80px;
            line-height: 1.6;
            padding: 0 10px;
        }

        .options-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 12px;
        }

        .option-btn {
            background: transparent;
            border: 2px solid var(--neon-blue);
            color: var(--text-main);
            padding: 12px;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.2s;
            font-size: 1rem;
            outline: none;
        }

        .option-btn:hover:not(:disabled) {
            background: rgba(56, 189, 248, 0.1);
            box-shadow: 0 0 15px var(--neon-blue);
        }

        .option-btn.correct {
            background: var(--neon-green) !important;
            border-color: var(--neon-green);
            color: #000;
        }

        .option-btn.wrong {
            background: var(--neon-pink) !important;
            border-color: var(--neon-pink);
            color: #000;
        }

        #feedback-panel {
            background: var(--feedback-bg);
            border-radius: 15px;
            padding: 15px;
            margin-top: 20px;
            text-align: left;
            border-left: 5px solid var(--neon-blue);
        }

        .explanation-en { font-style: italic; margin-bottom: 8px; font-size: 0.95rem; }
        .explanation-zh { color: var(--neon-blue); font-size: 0.95rem; }

        #start-screen, #end-screen {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background: var(--bg-color);
            z-index: 20;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border-radius: 20px;
            padding: 20px;
        }

        .revision-container {
            width: 100%;
            margin-top: 15px;
            text-align: left;
            background: rgba(15, 23, 42, 0.6);
            padding: 15px;
            border-radius: 10px;
            font-size: 0.85rem;
            max-height: 220px;
            overflow-y: auto;
        }

        .revision-title {
            color: var(--neon-green);
            font-weight: bold;
            margin-bottom: 10px;
            text-align: center;
            text-transform: uppercase;
        }

        .revision-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
            border-top: 1px solid #334155;
            padding-top: 10px;
        }

        .tense-cat {
            color: var(--neon-blue);
            font-weight: bold;
            margin-bottom: 5px;
        }

        .indicator-list {
            color: var(--text-dim);
            line-height: 1.4;
        }

        .hidden { display: none !important; }

        .btn-primary {
            background: var(--neon-blue);
            color: var(--bg-color);
            border: none;
            padding: 12px 30px;
            font-size: 1.1rem;
            font-weight: bold;
            border-radius: 30px;
            cursor: pointer;
            margin-top: 15px;
            box-shadow: 0 0 15px var(--neon-blue);
        }

        .btn-next {
            background: var(--neon-green);
            box-shadow: 0 0 15px var(--neon-green);
        }

        .highlight { color: var(--neon-pink); }
    </style>
</head>
<body>

<div id="game-container">
    <div id="start-screen">
        <h1>Tense Master</h1>
        <p style="color: var(--text-dim); margin-bottom: 10px;">Secondary 4 Revision: Advanced Sentences</p>
        <p style="color: var(--text-dim); font-size: 0.9rem; margin-bottom: 20px;">Complete 30 questions to master time indicators.</p>
        <button class="btn-primary" onclick="startGame()">START GAME</button>
    </div>

    <div id="end-screen" class="hidden">
        <h1>Results</h1>
        <p id="final-score" style="font-size: 1.5rem; margin: 10px 0;"></p>
        <div id="final-feedback"></div>
        
        <div class="revision-container">
            <div class="revision-title">Time Indicator Revision List</div>
            <div class="revision-grid">
                <div>
                    <div class="tense-cat">Present Simple / Cont.</div>
                    <div class="indicator-list">
                        • always/usually (總是/通常)<br>
                        • every morning (每天早晨)<br>
                        • currently (目前)<br>
                        • at this moment (此刻)
                    </div>
                </div>
                <div>
                    <div class="tense-cat">Past Simple</div>
                    <div class="indicator-list">
                        • ago (之前)<br>
                        • yesterday (昨天)<br>
                        • in the past (在過去)<br>
                        • last decade (上一個十年)
                    </div>
                </div>
                <div style="grid-column: span 2; border-top: 1px solid #334155; padding-top: 5px;">
                    <div class="tense-cat">Future Tense</div>
                    <div class="indicator-list">
                        • tomorrow morning (明天早上) | • next semester (下學期) | • eventually (最終) | • in the coming years (在未來幾年)
                    </div>
                </div>
            </div>
        </div>

        <button class="btn-primary" onclick="location.reload()">REPLAY</button>
    </div>

    <div class="stats-bar">
        <span>Score: <span id="score" class="highlight">0</span></span>
        <span>Question: <span id="q-count">1</span>/30</span>
    </div>

    <div id="timer-container">
        <div id="timer-bar"></div>
    </div>

    <div class="question-box" id="question">Loading...</div>
    <div class="options-grid" id="options"></div>

    <div id="feedback-panel" class="hidden">
        <div id="result-status" style="font-weight: bold; margin-bottom: 10px;"></div>
        <div class="explanation-en" id="exp-en"></div>
        <div class="explanation-zh" id="exp-zh"></div>
        <button class="btn-primary btn-next" id="next-btn" onclick="goToNext()">PROCEED</button>
    </div>
</div>

<script>
    const questionPool = [
        // PRESENT TENSES (LONGER)
        { q: "Our chemistry teacher usually _______ the weekly lab sessions every Monday morning to ensure we follow safety protocols.", a: "prepares", o: ["prepares", "is preparing", "prepared", "will prepare"], en: "'Usually' and 'every Monday' indicate a habitual present action.", zh: "'Usually' 和 'every Monday' 表示現在的習慣性動作。" },
        { q: "Look! The students in the courtyard _______ for the annual talent show right now, so please try to be quiet.", a: "are practicing", o: ["practice", "practiced", "are practicing", "will practice"], en: "'Right now' and 'Look!' signal an action currently in progress.", zh: "'Right now' 和 'Look!' 提示動作此時正在進行中。" },
        { q: "Despite the bad weather, the ferry _______ across the harbor every thirty minutes to transport commuters to the city center.", a: "operates", o: ["operates", "is operating", "operated", "will operate"], en: "'Every thirty minutes' refers to a regular, scheduled routine in the present.", zh: "'Every thirty minutes' 指的是現在常規的、有規律的日程。" },
        { q: "At this very moment, the marketing director _______ the final details of the advertisement with her creative team.", a: "is discussing", o: ["discusses", "discussed", "is discussing", "will discuss"], en: "'At this very moment' indicates a continuous action happening now.", zh: "'At this very moment' 表示現在正在進行的持續動作。" },
        { q: "The library _______ its digital archive every weekend to make sure that all online resources are accessible to students.", a: "updates", o: ["update", "updates", "updated", "will update"], en: "'Every weekend' suggests a repetitive task using the Present Simple.", zh: "'Every weekend' 提示這是一個重複性的任務，應使用一般現在時。" },
        { q: "Listen carefully! The principal _______ the winners of the inter-school debate competition over the public address system.", a: "is announcing", o: ["announces", "announced", "is announcing", "will announce"], en: "'Listen carefully!' indicates the announcement is happening at this second.", zh: "'Listen carefully!' 提示廣播此時此刻正在進行。" },
        { q: "The sun _______ the primary source of energy for almost all life forms on our planet, as scientists have proven.", a: "remains", o: ["remain", "remains", "remained", "will remain"], en: "Scientific facts and general truths are always stated in the Present Simple.", zh: "科學事實和普遍真理總是用一般現在時表述。" },
        { q: "Currently, many global organizations _______ tirelessly to reduce plastic pollution in the world's oceans through innovative recycling.", a: "are working", o: ["work", "worked", "are working", "will work"], en: "'Currently' focuses on a contemporary situation or ongoing effort.", zh: "'Currently' 側重於當前的狀況或正在進行的努力。" },
        { q: "My grandmother often _______ her childhood stories about living in the countryside whenever we visit her for dinner.", a: "tells", o: ["tell", "tells", "told", "will tell"], en: "'Often' and 'whenever' indicate a frequent present habit.", zh: "'Often' 和 'whenever' 表示頻繁的現在習慣。" },
        { q: "The local museum _______ a wide variety of historical artifacts that date back to the early Ming Dynasty.", a: "houses", o: ["house", "houses", "housed", "will house"], en: "Descriptions of existing states or permanent facts use Present Simple.", zh: "描述現有狀態或永久事實使用一般現在時。" },

        // PAST TENSES (LONGER)
        { q: "The construction company _______ the new residential complex in the northern district exactly three years ago today.", a: "completed", o: ["completes", "completed", "will complete", "is completing"], en: "'Three years ago today' points to a specific, finished point in the past.", zh: "'Three years ago today' 指向過去一個特定的、已結束的時間點。" },
        { q: "Last winter, the temperatures in the mountain region _______ to record lows, causing many pipes to freeze and burst.", a: "dropped", o: ["drop", "drops", "dropped", "will drop"], en: "'Last winter' refers to a completed time period in the past.", zh: "'Last winter' 指的是過去一個已結束的時間段。" },
        { q: "I _______ my best friend for lunch at that small Italian restaurant near the park yesterday afternoon.", a: "met", o: ["meet", "meets", "met", "will meet"], en: "'Yesterday afternoon' is a specific past time marker.", zh: "'Yesterday afternoon' 是特定的過去時間標記。" },
        { q: "The great explorer _______ the previously unknown islands during his long voyage across the Pacific in the 18th century.", a: "discovered", o: ["discovers", "discovered", "will discover", "is discovering"], en: "Historical events in the past (18th century) require the Past Simple.", zh: "過去的歷史事件（18世紀）需要使用一般過去時。" },
        { q: "When the lights suddenly went out during the storm last night, we _______ for some candles in the dark kitchen.", a: "searched", o: ["search", "searches", "searched", "will search"], en: "Refers to a specific action that happened during a past event (last night).", zh: "指在過去事件（昨晚）期間發生的特定動作。" },
        { q: "The ancient civilizations _______ impressive irrigation systems to support their large populations thousands of years ago.", a: "developed", o: ["develop", "develops", "developed", "will develop"], en: "'Thousands of years ago' is a clear indicator of the distant past.", zh: "'Thousands of years ago' 是遙遠過去的明確標記。" },
        { q: "The famous author _______ her first novel while she was working as a part-time librarian in her hometown.", a: "wrote", o: ["writes", "wrote", "will write", "is writing"], en: "Refers to a completed action (writing the novel) in the past.", zh: "指過去已完成的動作（寫小說）。" },
        { q: "Before the invention of the internet, people _______ letters to each other to share news across long distances.", a: "sent", o: ["send", "sends", "sent", "will send"], en: "'Before the invention of the internet' refers to an era in the past.", zh: "'Before the invention of the internet' 指的是過去的一個時代。" },
        { q: "He _______ his driving test on the first attempt last Tuesday, much to his parents' delight and surprise.", a: "passed", o: ["pass", "passes", "passed", "will pass"], en: "'Last Tuesday' indicates a specific completed event in the past.", zh: "'Last Tuesday' 表示過去一個特定的已完成事件。" },
        { q: "The scientist _______ the results of her experiment to the committee during the conference held two weeks ago.", a: "presented", o: ["presents", "presented", "will present", "is presenting"], en: "'Two weeks ago' requires the Past Simple tense for the main action.", zh: "'Two weeks ago' 要求主要動作使用一般過去時。" },

        // FUTURE TENSES (LONGER)
        { q: "Our environmental club _______ a large-scale beach cleanup operation next Saturday morning to celebrate Earth Day.", a: "will organize", o: ["organizes", "organized", "will organize", "is organizing"], en: "'Next Saturday morning' indicates a planned future event.", zh: "'Next Saturday morning' 表示計劃中的未來事件。" },
        { q: "In the coming decades, artificial intelligence _______ the way we work and interact with our surroundings in ways we cannot yet imagine.", a: "will transform", o: ["transforms", "transformed", "will transform", "is transforming"], en: "'In the coming decades' points to a future period for a prediction.", zh: "'In the coming decades' 指向未來的一段時期進行預測。" },
        { q: "If you study hard for the mock exams, I am sure that you _______ excellent grades in your final results next semester.", a: "will achieve", o: ["achieve", "achieved", "will achieve", "are achieving"], en: "'Next semester' and the prediction 'I am sure' signal the Future Tense.", zh: "'Next semester' 和預測語氣 'I am sure' 提示使用將來時。" },
        { q: "The space agency _______ a new satellite into orbit next month to monitor the effects of global climate change.", a: "will launch", o: ["launch", "launched", "will launch", "is launching"], en: "'Next month' is a definite future time marker.", zh: "'Next month' 是確定的未來時間標記。" },
        { q: "Maybe the government _______ stricter laws to protect endangered species in the tropical rainforests eventually.", a: "will introduce", o: ["introduces", "introduced", "will introduce", "is introducing"], en: "'Maybe' and 'eventually' suggest a future possibility or prediction.", zh: "'Maybe' 和 'eventually' 暗示未來的可能性或預測。" },
        { q: "I promise that I _______ you with your difficult mathematics assignment as soon as I finish my own project tonight.", a: "will help", o: ["help", "helped", "will help", "am helping"], en: "Promises and future plans (tonight) typically use 'will'.", zh: "承諾和未來的計劃（今晚）通常使用 'will'。" },
        { q: "According to the weather forecast, a powerful typhoon _______ the coast of Japan tomorrow afternoon, so stay indoors.", a: "will hit", o: ["hits", "hit", "will hit", "is hitting"], en: "'Tomorrow afternoon' is a future time reference for a prediction.", zh: "'Tomorrow afternoon' 是預測未來的時間參考。" },
        { q: "In the future, electric vehicles _______ the majority of cars on the road to help reduce carbon emissions.", a: "will become", o: ["become", "became", "will become", "are becoming"], en: "'In the future' is a general indicator of the Future Tense.", zh: "'In the future' 是將來時的一般標記。" },
        { q: "Our school football team _______ against their long-term rivals in the regional finals next Friday evening.", a: "will compete", o: ["competes", "competed", "will compete", "is competing"], en: "'Next Friday evening' points to a future event.", zh: "'Next Friday evening' 指向未來的事件。" },
        { q: "I hope that more people _______ the importance of mental health awareness in our society in the years to come.", a: "will realize", o: ["realize", "realized", "will realize", "are realizing"], en: "'In the years to come' and 'I hope' indicate a future expectation.", zh: "'In the years to come' 和 'I hope' 表示對未來的期望。" }
    ];

    let currentQuestions = [];
    let currentIndex = 0;
    let score = 0;
    let timer;
    let timeLeft = 100;

    function shuffle(array) {
        return array.sort(() => Math.random() - 0.5);
    }

    function startGame() {
        document.getElementById('start-screen').classList.add('hidden');
        currentQuestions = shuffle([...questionPool]);
        currentIndex = 0;
        score = 0;
        showQuestion();
    }

    function showQuestion() {
        document.getElementById('feedback-panel').classList.add('hidden');
        if (currentIndex >= currentQuestions.length) {
            endGame();
            return;
        }

        const data = currentQuestions[currentIndex];
        document.getElementById('question').innerText = data.q;
        document.getElementById('q-count').innerText = currentIndex + 1;
        document.getElementById('score').innerText = score;
        
        const optionsDiv = document.getElementById('options');
        optionsDiv.innerHTML = '';
        
        const shuffledOptions = shuffle([...data.o]);
        shuffledOptions.forEach(opt => {
            const btn = document.createElement('button');
            btn.className = 'option-btn';
            btn.innerText = opt;
            btn.onclick = () => checkAnswer(opt, data.a, btn);
            optionsDiv.appendChild(btn);
        });

        startTimer();
    }

    function startTimer() {
        clearInterval(timer);
        timeLeft = 100;
        const bar = document.getElementById('timer-bar');
        timer = setInterval(() => {
            timeLeft -= 0.8; // Slightly slower for longer sentences
            bar.style.width = timeLeft + "%";
            if (timeLeft <= 0) {
                clearInterval(timer);
                handleTimeout();
            }
        }, 100);
    }

    function checkAnswer(selected, correct, btn) {
        clearInterval(timer);
        const buttons = document.querySelectorAll('.option-btn');
        buttons.forEach(b => b.disabled = true);

        const statusText = document.getElementById('result-status');
        if (selected === correct) {
            btn.classList.add('correct');
            score += 10;
            statusText.innerText = "✓ CORRECT! 好極了！";
            statusText.style.color = "var(--neon-green)";
        } else {
            btn.classList.add('wrong');
            statusText.innerText = "✗ INCORRECT! 不正確";
            statusText.style.color = "var(--neon-pink)";
            buttons.forEach(b => {
                if (b.innerText === correct) b.classList.add('correct');
            });
        }
        showFeedback();
    }

    function handleTimeout() {
        const buttons = document.querySelectorAll('.option-btn');
        buttons.forEach(b => b.disabled = true);
        const statusText = document.getElementById('result-status');
        statusText.innerText = "⌛ TIME'S UP! 時間到";
        statusText.style.color = "var(--neon-pink)";
        
        const correct = currentQuestions[currentIndex].a;
        buttons.forEach(b => {
            if (b.innerText === correct) b.classList.add('correct');
        });
        showFeedback();
    }

    function showFeedback() {
        const data = currentQuestions[currentIndex];
        document.getElementById('exp-en').innerText = data.en;
        document.getElementById('exp-zh').innerText = data.zh;
        document.getElementById('feedback-panel').classList.remove('hidden');
    }

    function goToNext() {
        currentIndex++;
        showQuestion();
    }

    function endGame() {
        document.getElementById('end-screen').classList.remove('hidden');
        document.getElementById('final-score').innerText = `Your Score: ${score} / 300`;
        
        let msg = "";
        if (score >= 260) msg = "Master Level! You handled those complex sentences perfectly.";
        else if (score >= 180) msg = "Great effort! Review the time markers in longer sentences.";
        else msg = "Keep practicing! Don't let the extra words distract you from the indicators.";
        
        document.getElementById('final-feedback').innerText = msg;
    }
</script>

</body>
</html>
