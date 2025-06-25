.navbar\_\_link {
@apply relative inline-block px-3 py-2 uppercase font-medium overflow-hidden transition-all duration-500 ease-in-out;
}

/_ 🔹 Home — Скользящий фон _/
.effect-slide::before {
content: '';
@apply absolute top-0 left-full w-full h-full bg-indigo-400 opacity-20 blur-md transition-all duration-500;
z-index: -1;
}
.effect-slide:hover::before {
left: 0;
}

/_ 🔸 About — Заливка (ОСТАЁТСЯ) _/
.effect-fill::before {
content: '';
@apply absolute bottom-0 left-0 w-0 h-full bg-gradient-to-r from-pink-500 to-purple-600 transition-all duration-500;
z-index: -1;
}
.effect-fill:hover::before {
width: 100%;
}
.effect-fill:hover {
@apply text-white;
}

/_ ⚡ Contact — Глитч эффект _/
.effect-glitch {
position: relative;
color: #6366f1;
}
.effect-glitch::before,
.effect-glitch::after {
content: attr(data-text);
position: absolute;
left: 0;
width: 100%;
overflow: hidden;
color: #f43f5e;
clip: rect(0, 0, 0, 0);
}
.effect-glitch:hover::before {
animation: glitchTop 0.3s infinite linear alternate-reverse;
}
.effect-glitch:hover::after {
animation: glitchBottom 0.3s infinite linear alternate-reverse;
}
@keyframes glitchTop {
0% { clip: rect(0, 9999px, 5px, 0); transform: translate(-2px, -2px); }
100% { clip: rect(0, 9999px, 5px, 0); transform: translate(2px, -2px); }
}
@keyframes glitchBottom {
0% { clip: rect(10px, 9999px, 15px, 0); transform: translate(-2px, 2px); }
100% { clip: rect(10px, 9999px, 15px, 0); transform: translate(2px, 2px); }
}

/_ 🌊 News — Ripple эффект _/
.effect-ripple::after {
content: '';
@apply absolute left-1/2 top-1/2 w-0 h-0 bg-indigo-300 opacity-50 rounded-full transform -translate-x-1/2 -translate-y-1/2 transition-all duration-500;
z-index: -1;
}
.effect-ripple:hover::after {
@apply w-48 h-48;
opacity: 0;
}

/_ 🔍 Blog — Scale on hover _/
.effect-scale {
@apply transform transition-transform;
}
.effect-scale:hover {
@apply scale-110 text-indigo-600;
}

/_ 🌀 Services — Flip effect _/
.effect-flip {
@apply transform transition duration-500;
perspective: 1000px;
}
.effect-flip:hover {
transform: rotateY(180deg);
color: #8b5cf6;
}

/_ 🧭 Pricing — Rotate in _/
.effect-rotate {
@apply transition-transform duration-500;
}
.effect-rotate:hover {
transform: rotate(3deg) scale(1.05);
color: #4f46e5;
}

/_ 🟦 Support — Появление рамки _/
.effect-border {
@apply border border-transparent transition-all duration-500;
}
.effect-border:hover {
@apply border-indigo-500 bg-indigo-50 text-indigo-700;
}

////////
.navbar\_\_link {
@apply relative inline-block px-3 py-2 uppercase font-medium overflow-hidden transition-all duration-500 ease-in-out;
}

/_ 🔹 Home — Скользящий фон _/
.effect-slide::before {
content: '';
@apply absolute top-0 left-full w-full h-full bg-indigo-400 opacity-20 blur-md transition-all duration-500;
z-index: -1;
}
.effect-slide:hover::before {
left: 0;
}

/_ 🔸 About — Заливка (ОСТАЁТСЯ) _/
.effect-fill::before {
content: '';
@apply absolute bottom-0 left-0 w-0 h-full bg-gradient-to-r from-pink-500 to-purple-600 transition-all duration-500;
z-index: -1;
}
.effect-fill:hover::before {
width: 100%;
}
.effect-fill:hover {
@apply text-white;
}

/_ ⚡ Contact — Глитч эффект _/
.effect-glitch {
position: relative;
color: #6366f1;
}
.effect-glitch::before,
.effect-glitch::after {
content: attr(data-text);
position: absolute;
left: 0;
width: 100%;
overflow: hidden;
color: #f43f5e;
clip: rect(0, 0, 0, 0);
}
.effect-glitch:hover::before {
animation: glitchTop 0.3s infinite linear alternate-reverse;
}
.effect-glitch:hover::after {
animation: glitchBottom 0.3s infinite linear alternate-reverse;
}
@keyframes glitchTop {
0% { clip: rect(0, 9999px, 5px, 0); transform: translate(-2px, -2px); }
100% { clip: rect(0, 9999px, 5px, 0); transform: translate(2px, -2px); }
}
@keyframes glitchBottom {
0% { clip: rect(10px, 9999px, 15px, 0); transform: translate(-2px, 2px); }
100% { clip: rect(10px, 9999px, 15px, 0); transform: translate(2px, 2px); }
}

/_ 🌊 News — Ripple эффект _/
.effect-ripple::after {
content: '';
@apply absolute left-1/2 top-1/2 w-0 h-0 bg-indigo-300 opacity-50 rounded-full transform -translate-x-1/2 -translate-y-1/2 transition-all duration-500;
z-index: -1;
}
.effect-ripple:hover::after {
@apply w-48 h-48;
opacity: 0;
}

/_ 🔍 Blog — Scale on hover _/
.effect-scale {
@apply transform transition-transform;
}
.effect-scale:hover {
@apply scale-110 text-indigo-600;
}

/_ 🌀 Services — Flip effect _/
.effect-flip {
@apply transform transition duration-500;
perspective: 1000px;
}
.effect-flip:hover {
transform: rotateY(180deg);
color: #8b5cf6;
}

/_ 🧭 Pricing — Rotate in _/
.effect-rotate {
@apply transition-transform duration-500;
}
.effect-rotate:hover {
transform: rotate(3deg) scale(1.05);
color: #4f46e5;
}

/_ 🟦 Support — Появление рамки _/
.effect-border {
@apply border border-transparent transition-all duration-500;
}
.effect-border:hover {
@apply border-indigo-500 bg-indigo-50 text-indigo-700;
}
