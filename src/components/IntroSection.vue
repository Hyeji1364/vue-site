<template>
    <section id="intro">
        <div class="intro__inner">
            <h2 class="intro__title">developer</h2>
            <div class="intro__lines" aria-hidden="true">
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
            </div>
            <div class="intro__text">
                <div class="text">
                    <div>Hello</div>
                    <div>found at the end of the</div>
                    <div>effort</div>
                </div>
                <div class="img">
                    <img src="https://images.unsplash.com/photo-1581403341630-a6e0b9d2d257?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NjJ8fHBvcnRyYWl0fGVufDB8fDB8fHww" alt="">
                </div>
            </div>
            <div class="bottom" aria-hidden="true">
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    #intro {
        height: 100vh;

        .intro__inner{
            width: 100%;
            height: 100%;
            display: flex;
            align-items: flex-start;
            justify-content: center;
            flex-direction: column;
            padding: 16px;
            margin-top: 6rem;

            .intro__title {
            font-size: 10vw;
            line-height: 1;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: -0.3vw;
            text-align: center;
            white-space: normal; /* 필요 시 추가 */
            margin: 0 auto; /* 중앙 정렬을 더 잘 맞추기 위해 추가 */
            color: #6470C8;
            
            }

            .intro__lines {
                width: 100%;
                
                .line {
                    display: block;
                    width: 100%;
                    height: 1px;
                    background-color: var(--black);
                    margin-bottom: 0.5vw;

                    &:nth-child(1){
                        height: 1px;
                    }
                    &:nth-child(2){
                        height: 2px;
                    }
                    &:nth-child(3){
                        height: 5px;
                    }
                    &:nth-child(4){
                        height: 9px;
                    }
                    &:nth-child(5){
                        height: 13px;
                    }
                    &:nth-child(6){
                        height: 16px;
                    }
                    &:nth-child(7){
                        height: 20px;
                    }
                }

                &.bottom {
                    display: none;
                }
            }

            .intro__text {
                width: 100%;
                height: 40vh;
                background-color: var(--black);
                color: var(--white);
                align-items: center;
                justify-content: center;
                flex-direction: column;
                position: relative;

                .text {
                    font-size: 3vw;
                    line-height: 1;
                    font-weight: 900;
                    text-transform: uppercase;
                    text-decoration: underline;
                    text-align: center;
                    position: relative;
                    z-index: 100;
                    transition: all 0.3s;
                    cursor: all-scroll;
                }

                .img {
                    position: absolute;
                    left: 50%;
                    top: 50%;
                    transform: translate(-50%, -50%);
                    width: 30vh;
                    height: 30vh;
                    border-radius: 50%;
                    overflow: hidden;
                    filter: grayscale(100%);
                    transition: all 0.3s;

                }
            }
        }
    }
</style>