.windows8 {
    position: relative;
    width: 50px;
    height: 50px;
}

.windows8 .ball {
    position: absolute;
    width: 48px;
    height: 48px;
    opacity: 0;
    transform: rotate(225deg);
    animation: windows8-spin 5.5s infinite;
}

.windows8 .ball::after {
    content: '';
    position: absolute;
    width: 6px;
    height: 6px;
    background: #000000;
    border-radius: 50%;
    left: 0;
    top: 0;
}

.windows8 .ball:nth-child(1) { animation-delay: 0.24s; }
.windows8 .ball:nth-child(2) { animation-delay: 0.48s; }
.windows8 .ball:nth-child(3) { animation-delay: 0.72s; }
.windows8 .ball:nth-child(4) { animation-delay: 0.96s; }
.windows8 .ball:nth-child(5) { animation-delay: 1.2s; }

@keyframes windows8-spin {
    0% {
        opacity: 1;
        transform: rotate(180deg);
        animation-timing-function: ease-out;
    }

    7% {
        opacity: 1;
        transform: rotate(300deg);
        animation-timing-function: linear;
    }

    30% {
        opacity: 1;
        transform: rotate(410deg);
        animation-timing-function: ease-in-out;
    }

    39% {
        opacity: 1;
        transform: rotate(645deg);
        animation-timing-function: linear;
    }

    70% {
        opacity: 1;
        transform: rotate(770deg);
        animation-timing-function: ease-out;
    }

    75% {
        opacity: 1;
        transform: rotate(900deg);
        animation-timing-function: ease-out;
    }

    76%, 100% {
        opacity: 0;
        transform: rotate(900deg);
    }
}
