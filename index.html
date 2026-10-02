<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>오늘의 밥 - 언주중학교 급식 정보</title>
    <style>
        :root {
            --bg-color: #f2f4f6;
            --card-bg: #ffffff;
            --text-primary: #191f28;
            --text-secondary: #8b95a1;
            --accent-color: #3182f6;
            --accent-light: #e8f3ff;
            --border-radius: 20px;
            --shadow: 0 8px 16px rgba(0, 0, 0, 0.04);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-primary);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            width: 100%;
            max-width: 420px;
            background-color: var(--card-bg);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 32px 24px;
            position: relative;
            overflow: hidden;
        }

        /* Step Management */
        .step {
            display: none;
            animation: fadeIn 0.3s ease-in-out forwards;
        }

        .step.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .header {
            margin-bottom: 24px;
        }

        .header .subtitle {
            font-size: 14px;
            color: var(--accent-color);
            font-weight: 600;
            margin-bottom: 4px;
        }

        .header h1 {
            font-size: 24px;
            font-weight: 700;
            line-height: 1.3;
        }

        /* Form elements */
        .input-group {
            margin-bottom: 24px;
        }

        label {
            display: block;
            font-size: 14px;
            color: var(--text-secondary);
            margin-bottom: 8px;
        }

        input[type="date"] {
            width: 100%;
            padding: 16px;
            border: 1px solid #e5e8eb;
            border-radius: 12px;
            font-size: 16px;
            outline: none;
            background-color: #f9fafb;
            color: var(--text-primary);
            transition: border-color 0.2s;
        }

        input[type="date"]:focus {
            border-color: var(--accent-color);
            background-color: #fff;
        }

        /* Allergy Grid */
        .allergy-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            max-height: 280px;
            overflow-y: auto;
            padding-right: 4px;
            margin-bottom: 20px;
        }

        .allergy-item {
            display: flex;
            align-items: center;
            padding: 12px 14px;
            border: 1px solid #e5e8eb;
            border-radius: 12px;
            cursor: pointer;
            transition: all 0.2s;
            font-size: 14px;
            user-select: none;
        }

        .allergy-item input {
            display: none;
        }

        .allergy-item.selected {
            background-color: var(--accent-light);
            border-color: var(--accent-color);
            color: var(--accent-color);
            font-weight: 600;
        }

        /* Buttons */
        .btn {
            width: 100%;
            padding: 16px;
            background-color: var(--accent-color);
            color: white;
            border: none;
            border-radius: 12px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: opacity 0.2s;
        }

        .btn:hover {
            opacity: 0.9;
        }

        .btn-secondary {
            background-color: #f2f4f6;
            color: var(--text-primary);
            margin-top: 8px;
        }

        /* Result Display */
        .result-card {
            background-color: #f9fafb;
            border-radius: 16px;
            padding: 20px;
            margin-bottom: 20px;
        }

        .menu-list {
            list-style: none;
            margin-top: 12px;
        }

        .menu-item {
            padding: 8px 0;
            border-bottom: 1px border-bottom: 1px solid #f2f4f6;
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 15px;
        }

        .menu-item:last-child {
            border-bottom: none;
        }

        .star-badge {
            color: #ffb300;
            margin-left: 6px;
        }

        .allergy-warning {
            color: #f04438;
            font-size: 12px;
            font-weight: 600;
        }

        .info-box {
            font-size: 12px;
            color: var(--text-secondary);
            margin-top: 16px;
            padding-top: 12px;
            border-top: 1px dashed #e5e8eb;
            line-height: 1.5;
        }

        .no-meal {
            text-align: center;
            padding: 30px 0;
            color: var(--text-secondary);
            font-size: 16px;
        }

        .no-meal-icon {
            font-size: 40px;
            margin-bottom: 12px;
        }
    </style>
</head>
<body>

<div class="container">
    <!-- STEP 1: 날짜 선택 -->
    <div id="step1" class="step active">
        <div class="header">
            <div class="subtitle">언주중학교 급식안내 🍱</div>
            <h1>확인하고 싶은<br>날짜를 선택해주세요</h1>
        </div>
        <div class="input-group">
            <label for="meal-date">날짜 선택</label>
            <input type="date" id="meal-date" value="2026-10-01" min="2026-10-01" max="2026-10-31">
        </div>
        <button class="btn" onclick="goToStep(2)">다음</button>
    </div>

    <!-- STEP 2: 알레르기 선택 -->
    <div id="step2" class="step">
        <div class="header">
            <div class="subtitle">맞춤 영양 정보 ⚠️</div>
            <h1>피해야 하는<br>알레르기 항원을 선택하세요</h1>
        </div>
        <div class="allergy-grid" id="allergyContainer">
            <!-- 자바스크립트로 동적 생성 -->
        </div>
        <button class="btn" onclick="showMealResult()">급식 확인하기</button>
        <button class="btn btn-secondary" onclick="goToStep(1)">이전</button>
    </div>

    <!-- STEP 3: 급식 결과 표시 -->
    <div id="step3" class="step">
        <div class="header">
            <div class="subtitle" id="result-date-title">2026년 10월 1일</div>
            <h1 id="result-main-title">오늘의 급식 🍽️</h1>
        </div>

        <div id="result-content">
            <!-- 급식 내용이 동적으로 삽입됩니다 -->
        </div>

        <button class="btn btn-secondary" onclick="goToStep(1)">다른 날짜 확인하기</button>
    </div>
</div>

<script>
    // 2026년 10월 언주중학교 급식 데이터베이스
    // 별표(isFavorite: true)는 학생 선호 인기 메뉴 표시
    const mealData = {
        "2026-10-01": {
            type: "meal",
            title: "10월 생일상",
            menu: [
                { name: "칼슘찹쌀밥", allergy: [] },
                { name: "황태미역국", allergy: [5, 6] },
                { name: "버섯소불고기", allergy: [5, 6, 13, 16, 18], isFavorite: true },
                { name: "계란말이", allergy: [1, 9] },
                { name: "배추겉절이", allergy: [9] },
                { name: "쇼콜라크레이프케이크", allergy: [1, 2, 5, 6, 10, 13], isFavorite: true }
            ],
            nutrition: "열량 571.7kcal / 단백질 36.3g / 칼슘 223.2mg / 철분 4.9mg"
        },
        "2026-10-02": {
            type: "meal",
            menu: [
                { name: "백미밥", allergy: [] },
                { name: "한우사골순대국", allergy: [5, 6, 10, 16] },
                { name: "숯불데리야끼파닭꼬치", allergy: [5, 6, 12, 15, 16], isFavorite: true },
                { name: "애호박양념무침", allergy: [5, 6] },
                { name: "석박지", allergy: [9] },
                { name: "달콤촉촉반건시", allergy: [] }
            ],
            nutrition: "열량 694.8kcal / 단백질 24.3g / 칼슘 87.2mg / 철분 13.7mg"
        },
        "2026-10-03": { type: "holiday", name: "주말 (개천절)" },
        "2026-10-04": { type: "holiday", name: "주말" },
        "2026-10-05": { type: "holiday", name: "대체공휴일" },
        "2026-10-06": {
            type: "meal",
            menu: [
                { name: "차조밥", allergy: [] },
                { name: "호박고추장찌개", allergy: [5, 6] },
                { name: "등갈비찜", allergy: [5, 6, 10, 13, 18], isFavorite: true },
                { name: "청포묵김가루무침", allergy: [5, 6] },
                { name: "배추겉절이", allergy: [9] },
                { name: "군고구마", allergy: [] }
            ],
            nutrition: "열량 541.4kcal / 단백질 16.0g / 칼슘 125.6mg / 철분 2.2mg"
        },
        "2026-10-07": {
            type: "meal",
            menu: [
                { name: "훈제오리볶음밥", allergy: [1, 2, 5, 6, 13, 16, 18] },
                { name: "트위스트꼬치어묵국", allergy: [1, 5, 6] },
                { name: "빠삭킹싸이치킨/치폴레마요소스", allergy: [1, 2, 5, 6, 12, 13, 15, 16], isFavorite: true },
                { name: "레인보우큐브치즈샐러드(오리엔탈D)", allergy: [2, 5, 6, 12, 13] },
                { name: "깍두기", allergy: [9] },
                { name: "앤티앤스프레즐", allergy: [2, 6], isFavorite: true }
            ],
            nutrition: "열량 955.0kcal / 단백질 38.8g / 칼슘 259.3mg / 철분 4.4mg"
        },
        "2026-10-08": {
            type: "meal",
            menu: [
                { name: "서리태밥", allergy: [5] },
                { name: "대구지리탕", allergy: [5, 9] },
                { name: "순살닭볶음", allergy: [5, 6, 13, 15] },
                { name: "연근조림", allergy: [5, 6, 13] },
                { name: "총각김치", allergy: [9] },
                { name: "칠보리팬케이크", allergy: [1, 2] }
            ],
            nutrition: "열량 767.9kcal / 단백질 41.6g / 칼슘 161.9mg / 철분 4.9mg"
        },
        "2026-10-09": { type: "holiday", name: "한글날" },
        "2026-10-10": { type: "holiday", name: "주말" },
        "2026-10-11": { type: "holiday", name: "주말" },
        "2026-10-12": {
            type: "meal",
            menu: [
                { name: "기장밥", allergy: [] },
                { name: "참치김치찌개", allergy: [5, 9] },
                { name: "수육보쌈", allergy: [5, 6, 10, 13], isFavorite: true },
                { name: "들기름막국수", allergy: [3, 5, 6, 13, 16] },
                { name: "양배추쌈/쌈장", allergy: [5, 6, 13] },
                { name: "보쌈김치", allergy: [9] },
                { name: "조각배", allergy: [] }
            ],
            nutrition: "열량 823.3kcal / 단백질 39.7g / 칼슘 140.0mg / 철분 3.5mg"
        },
        "2026-10-13": {
            type: "meal",
            menu: [
                { name: "현미찹쌀밥", allergy: [] },
                { name: "소고기육개장", allergy: [5, 6, 16] },
                { name: "직화석쇠불고기", allergy: [5, 6, 10, 18], isFavorite: true },
                { name: "애느타리버섯볶음", allergy: [] },
                { name: "간장깻잎지", allergy: [5, 6] },
                { name: "총각김치", allergy: [9] },
                { name: "샤인머스캣", allergy: [], isFavorite: true }
            ],
            nutrition: "열량 531.2kcal / 단백질 26.8g / 칼슘 219.1mg / 철분 2.4mg"
        },
        "2026-10-14": {
            type: "meal",
            menu: [
                { name: "지코바st치밥", allergy: [1, 5, 6, 15, 16, 18], isFavorite: true },
                { name: "들깨무채국", allergy: [5, 6] },
                { name: "킹새우튀김/칠리소스", allergy: [5, 6, 9, 12, 16] },
                { name: "감말랭이샐러드", allergy: [5, 6, 12, 13] },
                { name: "깍두기", allergy: [9] },
                { name: "소금우유아이스크림", allergy: [2], isFavorite: true }
            ],
            nutrition: "열량 882.0kcal / 단백질 52.2g / 칼슘 250.7mg / 철분 4.0mg"
        },
        "2026-10-15": {
            type: "meal",
            title: "동아리의 날",
            menu: [
                { name: "귀리밥", allergy: [] },
                { name: "낙지수제비국", allergy: [5, 6] },
                { name: "닭다리살바베큐구이", allergy: [5, 6, 12, 13, 15, 16, 18], isFavorite: true },
                { name: "시금치두부무침", allergy: [5, 6, 13] },
                { name: "배추김치", allergy: [9] },
                { name: "바나나", allergy: [] }
            ],
            nutrition: "열량 628.0kcal / 단백질 33.4g / 칼슘 126.2mg / 철분 2.8mg"
        },
        "2026-10-16": {
            type: "meal",
            menu: [
                { name: "율무밥", allergy: [] },
                { name: "부대찌개/라면사리", allergy: [1, 2, 5, 6, 9, 10, 12, 15, 16], isFavorite: true },
                { name: "데리야끼고등어구이", allergy: [5, 6, 7, 13] },
                { name: "매콤어묵볶음", allergy: [1, 5, 6, 13] },
                { name: "백김치", allergy: [9] },
                { name: "행운의황치즈타르트", allergy: [1, 2, 5, 6, 16] }
            ],
            nutrition: "열량 806.4kcal / 단백질 30.3g / 칼슘 180.8mg / 철분 3.9mg"
        },
        "2026-10-17": { type: "holiday", name: "주말" },
        "2026-10-18": { type: "holiday", name: "주말" },
        "2026-10-19": {
            type: "meal",
            menu: [
                { name: "현미찹쌀밥", allergy: [] },
                { name: "소고기무국", allergy: [5, 6, 16] },
                { name: "간장오리불고기", allergy: [5, 6, 12, 13, 16, 18] },
                { name: "마늘쫑고추장무침", allergy: [5, 6, 13] },
                { name: "무쌈", allergy: [] },
                { name: "배추김치", allergy: [9] },
                { name: "조각멜론", allergy: [] }
            ],
            nutrition: "열량 450.3kcal / 단백질 14.4g / 칼슘 153.7mg / 철분 1.7mg"
        },
        "2026-10-20": {
            type: "meal",
            menu: [
                { name: "늘보리밥", allergy: [] },
                { name: "우거지감자탕", allergy: [5, 6, 9, 10] },
                { name: "오삼불고기", allergy: [5, 6, 10, 13, 17], isFavorite: true },
                { name: "무생채", allergy: [13] },
                { name: "오이김치", allergy: [9] },
                { name: "페스츄리호두과자", allergy: [1, 2, 6, 14] }
            ],
            nutrition: "열량 840.6kcal / 단백질 38.8g / 칼슘 167.4mg / 철분 2.9mg"
        },
        "2026-10-21": {
            type: "meal",
            menu: [
                { name: "계란마늘새우볶음밥", allergy: [1, 5, 6, 9, 13, 18] },
                { name: "팽이미소국", allergy: [5, 6] },
                { name: "60계st간지치킨", allergy: [5, 6, 15, 18], isFavorite: true },
                { name: "알감자버터구이", allergy: [2, 13] },
                { name: "깍두기", allergy: [9] },
                { name: "마시는요구르트", allergy: [2] }
            ],
            nutrition: "열량 721.8kcal / 단백질 35.5g / 칼슘 237.2mg / 철분 3.3mg"
        },
        "2026-10-22": {
            type: "meal",
            menu: [
                { name: "기장밥", allergy: [] },
                { name: "꽃게탕", allergy: [5, 6, 8, 9, 17] },
                { name: "삼겹살마늘구이", allergy: [10], isFavorite: true },
                { name: "숙주미나리무침", allergy: [5, 6] },
                { name: "상추쌈/쌈장", allergy: [5, 6, 13] },
                { name: "배추김치", allergy: [9] },
                { name: "허니버터하루견과", allergy: [2, 4, 5, 14] }
            ],
            nutrition: "열량 660.1kcal / 단백질 29.7g / 칼슘 123.8mg / 철분 2.2mg"
        },
        "2026-10-23": {
            type: "meal",
            title: "사과데이",
            menu: [
                { name: "산채비빔밥/고추장", allergy: [5, 6] },
                { name: "우삼겹된장찌개", allergy: [2, 5, 6, 16] },
                { name: "갈비만두", allergy: [1, 5, 6, 10, 16, 18] },
                { name: "계란장조림", allergy: [1, 5, 6, 13] },
                { name: "열무김치", allergy: [9] },
                { name: "한입사과", allergy: [] }
            ],
            nutrition: "열량 551.1kcal / 단백질 23.4g / 칼슘 203.6mg / 철분 4.3mg"
        },
        "2026-10-24": { type: "holiday", name: "주말" },
        "2026-10-25": { type: "holiday", name: "주말" },
        "2026-10-26": {
            type: "meal",
            menu: [
                { name: "쌀밥", allergy: [] },
                { name: "버섯샤브전골", allergy: [5, 6, 16] },
                { name: "언양식바싹불고기", allergy: [2, 5, 6, 15] },
                { name: "꽃맛살샐러드", allergy: [1, 2, 5, 6, 13] },
                { name: "배추김치", allergy: [9] },
                { name: "아이스망고&치즈큐브", allergy: [1, 2, 5, 6] }
            ],
            nutrition: "열량 495.5kcal / 단백질 23.8g / 칼슘 96.02mg / 철분 1.8mg"
        },
        "2026-10-27": {
            type: "meal",
            title: "시험응원",
            menu: [
                { name: "반마리옛날통닭", allergy: [2, 5, 6, 15, 16, 18], isFavorite: true },
                { name: "전복죽", allergy: [18] },
                { name: "모짜렐라치즈스틱", allergy: [1, 2, 5, 6] },
                { name: "게맛살오이냉채", allergy: [1, 5, 6, 8, 13] },
                { name: "배추겉절이", allergy: [9] },
                { name: "수제퐁당미숫가루", allergy: [2, 5, 6] }
            ],
            nutrition: "열량 885.6kcal / 단백질 61.6g / 칼슘 369.7mg / 철분 5.7mg"
        },
        "2026-10-28": {
            type: "meal",
            title: "2학년만 급식",
            menu: [
                { name: "강황밥", allergy: [] },
                { name: "하이라이스/할라피뇨소시지", allergy: [1, 2, 5, 6, 10, 12, 15, 16] },
                { name: "유부장국", allergy: [5, 6] },
                { name: "가츠산도", allergy: [1, 2, 4, 5, 6, 8, 9, 10, 11, 12, 13, 15, 16, 17, 18], isFavorite: true },
                { name: "진미채조림", allergy: [1, 5, 6, 13, 17, 18] },
                { name: "깍두기", allergy: [9] },
                { name: "감귤", allergy: [] }
            ],
            nutrition: "열량 1004.0kcal / 단백질 29.0g / 칼슘 214.4mg / 철분 3.6mg"
        },
        "2026-10-29": {
            type: "meal",
            title: "2학년만 급식",
            menu: [
                { name: "참치김치밥버거", allergy: [1, 5, 9, 13, 16, 18], isFavorite: true },
                { name: "감자양파국", allergy: [5, 6] },
                { name: "후라이드닭다리튀김", allergy: [1, 2, 5, 6, 15, 16] },
                { name: "치킨무", allergy: [] },
                { name: "딸기라떼", allergy: [2, 13] }
            ],
            nutrition: "열량 1146.6kcal / 단백질 43.1g / 칼슘 348.6mg / 철분 4.5mg"
        },
        "2026-10-30": {
            type: "holiday",
            name: "급식 미제공 (1,2학년 진로체험 / 3학년 지필평가)"
        },
        "2026-10-31": { type: "holiday", name: "주말" }
    };

    // 알레르기 원인 식품 목록 (1~19번)
    const allergyList = [
        { id: 0, name: "없음 (해당사항 없음)" },
        { id: 1, name: "1. 난류" },
        { id: 2, name: "2. 우유" },
        { id: 3, name: "3. 메밀" },
        { id: 4, name: "4. 땅콩" },
        { id: 5, name: "5. 대두" },
        { id: 6, name: "6. 밀" },
        { id: 7, name: "7. 고등어" },
        { id: 8, name: "8. 게" },
        { id: 9, name: "9. 새우" },
        { id: 10, name: "10. 돼지고기" },
        { id: 11, name: "11. 복숭아" },
        { id: 12, name: "12. 토마토" },
        { id: 13, name: "13. 아황산류" },
        { id: 14, name: "14. 호두" },
        { id: 15, name: "15. 닭고기" },
        { id: 16, name: "16. 쇠고기" },
        { id: 17, name: "17. 오징어" },
        { id: 18, name: "18. 조개류" },
        { id: 19, name: "19. 잣" }
    ];

    let selectedAllergies = new Set();

    // 초기화 및 알레르기 목록 그리드 생성
    window.onload = function() {
        const container = document.getElementById("allergyContainer");
        allergyList.forEach(item => {
            const div = document.createElement("div");
            div.className = `allergy-item ${item.id === 0 ? 'selected' : ''}`;
            div.onclick = () => toggleAllergy(item.id, div);
            div.innerHTML = `<input type="checkbox" id="alg-${item.id}"> ${item.name}`;
            container.appendChild(div);
        });
        if (selectedAllergies.size === 0) selectedAllergies.add(0);
    };

    // 알레르기 선택 토글 기능
    function toggleAllergy(id, element) {
        if (id === 0) {
            selectedAllergies.clear();
            selectedAllergies.add(0);
            document.querySelectorAll('.allergy-item').forEach(el => el.classList.remove('selected'));
            element.classList.add('selected');
        } else {
            if (selectedAllergies.has(0)) {
                selectedAllergies.delete(0);
                document.querySelectorAll('.allergy-item')[0].classList.remove('selected');
            }
            if (selectedAllergies.has(id)) {
                selectedAllergies.delete(id);
                element.classList.remove('selected');
            } else {
                selectedAllergies.add(id);
                element.classList.add('selected');
            }
            if (selectedAllergies.size === 0) {
                selectedAllergies.add(0);
                document.querySelectorAll('.allergy-item')[0].classList.add('selected');
            }
        }
    }

    // Step 이동
    function goToStep(stepNumber) {
        document.querySelectorAll('.step').forEach(step => step.classList.remove('active'));
        document.getElementById(`step${stepNumber}`).classList.add('active');
    }

    // 결과 출력
    function showMealResult() {
        const dateInput = document.getElementById('meal-date').value;
        const data = mealData[dateInput];
        
        const dateObj = new Date(dateInput);
        const formattedDate = `${dateObj.getFullYear()}년 ${dateObj.getMonth() + 1}월 ${dateObj.getDate()}일`;
        
        document.getElementById('result-date-title').innerText = formattedDate;
        const resultContent = document.getElementById('result-content');

        if (!data || data.type === 'holiday') {
            const holidayName = data ? data.name : "주말 및 공휴일";
            document.getElementById('result-main-title').innerText = "급식 없음 😴";
            resultContent.innerHTML = `
                <div class="result-card">
                    <div class="no-meal">
                        <div class="no-meal-icon">🏖️</div>
                        <strong>${holidayName}</strong>
                        <p style="margin-top:8px; font-size:14px; color:#8b95a1;">오늘은 급식이 제공되지 않습니다.</p>
                    </div>
                </div>
            `;
        } else {
            document.getElementById('result-main-title').innerText = data.title ? `오늘의 급식 (${data.title})` : "오늘의 급식 🍽️";
            
            let menuHtml = '<ul class="menu-list">';
            data.menu.forEach(item => {
                // 알레르기 매칭 검사
                const matchedAllergies = item.allergy.filter(a => selectedAllergies.has(a));
                const hasWarning = !selectedAllergies.has(0) && matchedAllergies.length > 0;
                
                menuHtml += `
                    <li class="menu-item">
                        <div>
                            <span>${item.name}</span>
                            ${item.isFavorite ? '<span class="star-badge" title="인기메뉴">⭐</span>' : ''}
                        </div>
                        ${hasWarning ? `<span class="allergy-warning">⚠️ 알레르기 (${matchedAllergies.join(', ')})</span>` : ''}
                    </li>
                `;
            });
            menuHtml += '</ul>';

            resultContent.innerHTML = `
                <div class="result-card">
                    ${menuHtml}
                    <div class="info-box">
                        <strong>📊 영양 정보</strong><br>
                        ${data.nutrition}
                    </div>
                </div>
            `;
        }

        goToStep(3);
    }
</script>

</body>
</html>
