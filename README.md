<style>
    /* SVG容器样式保持不变 */
    #container {
        width: 100%;
        margin: 50px auto;
    }

    #hello-svg {
        width: 100%;
        height: auto;
    }
    
    /* 定义渐变色 */
    #hello-svg {
        --gradient-1: #FF6B6B, #4ECDC4, #45B7D1;
        --gradient-2: #96E6A1, #D4FC79;
        --gradient-3: #FFD93D, #FF6B6B;
    }
    
    /* 路径基础样式 */
    .path {
        fill: none;
        stroke-width: 5;
        stroke-linecap: round;
        stroke-linejoin: round;
    }
    
    /* 路径1动画和渐变 */
    .path-1 {
        stroke: url(#gradient1);
        stroke-dasharray: 1800;
        stroke-dashoffset: 1800;
        animation: drawPath1 3s ease forwards;
    }
    
    /* 路径2动画和渐变 */
    .path-2 {
        stroke: url(#gradient2);
        stroke-dasharray: 600;
        stroke-dashoffset: 600;
        animation: drawPath2 2s ease forwards 3s;
    }
    
    /* 路径3动画和渐变 */
    .path-3 {
        stroke: url(#gradient3);
        stroke-dasharray: 300;
        stroke-dashoffset: 300;
        animation: drawPath3 1.5s ease forwards 5s;
    }
    
    /* 动画关键帧保持不变 */
    @keyframes drawPath1 {
        to {
            stroke-dashoffset: 0;
        }
    }
    
    @keyframes drawPath2 {
        to {
            stroke-dashoffset: 0;
        }
    }
    
    @keyframes drawPath3 {
        to {
            stroke-dashoffset: 0;
        }
    }
</style>

<div id="container">
    <svg id="hello-svg" data-name="hello" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 582 197">
        <defs>
            <linearGradient id="gradient1" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" style="stop-color:#FF6B6B"/>
                <stop offset="50%" style="stop-color:#4ECDC4"/>
                <stop offset="100%" style="stop-color:#45B7D1"/>
            </linearGradient>
            <linearGradient id="gradient2" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" style="stop-color:#96E6A1"/>
                <stop offset="100%" style="stop-color:#D4FC79"/>
            </linearGradient>
            <linearGradient id="gradient3" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" style="stop-color:#FFD93D"/>
                <stop offset="100%" style="stop-color:#FF6B6B"/>
            </linearGradient>
        </defs>
        <path class="path path-1" d="M208,338c38-16.67,73.74-45.72,97.33-66,21.33-18.33,32.67-35.67,37.33-52.67C347.12,203.12,344,192,332,192c-11,0-21,10.33-24.94,27.68-4.52,19.89-22.06,107.82-29.39,149,15.67-72.33,36.33-81.33,53.67-81.33,22.33,0,24.67,18.67,19.42,39-5.43,21.07-7.42,44.32,17.91,44.32,18,0,35.53-8.17,52.67-20,14-9.67,23-24,23-40,0-13.42-8-23.33-20.67-23.33s-24.33,12-24.33,33.33c0,27,16.33,48,44,48,25.67,0,47.67-19.67,62-44.67,13.61-23.74,30.67-64.67,33.33-92.67s-5.33-36-18.67-36-24.67,17.33-28.67,43.33S486,302,491.33,330s28,37.67,46,37.67,38.17-15.67,52-37c16.54-25.51,35.87-67.45,38.67-102,2-24.67-8.67-33.33-20-33.33-14.67,0-23.33,13.33-28,38-4.5,23.81-8,64-2,94,4.64,23.21,25.33,40.33,44.67,40.33s32.67-19,36.67-42.33" transform="translate(-199 -183)"/>
        <path class="path path-2" d="M697.33,287.33C672,287.33,661.33,305,659,327c-2.81,26.54,10.33,41.67,29.67,41.67,22,0,34.54-20.78,36.67-40.67,2-18.67-7.39-39.13-28-40.67" transform="translate(-199 -183)"/>
        <path class="path path-3" d="M714.8,295.12c12.11,12.26,43.53,9.55,56.53-5.79" transform="translate(-199 -183)"/>
        <line class="path path-4" x1="561" y1="181.67" x2="561" y2="181.67"/>
    </svg>
</div>
