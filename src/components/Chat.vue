<template>
    <section>
        <div class="container">
            <div class="left-content">
                <div class="search-box">
                    <input type="search" class="search-field">
                    <i class='bx bx-search search-icon'></i>
                </div>
                <div class="chat-lists">
                    <div class="single-list" v-for="(item, index) in 20" :key="index">
                        <img src="../assets/women.jpg" alt="" class="chat-img">
                        <div class="text">
                            <h5 class="chat-name">Sahiner Bou {{ index+1 }}</h5>
                            <p class="chat-message">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ullam, excepturi.</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="right-content">
                <div class="top-contents">
                    <div class="chat-info">
                        <img src="../assets/women.jpg" alt="" class="chat-img">
                        <h5 class="chat-name">Sahiner Bou</h5>
                    </div>
                    <div class="icon-lists">
                        <i class='bx bx-phone'></i>
                        <i class='bx bx-video' ></i>
                        <i class='bx bx-dots-vertical-rounded' ></i>
                    </div>
                </div>
                <div class="chat-body">
                    <div class="chat-message">
                        <img src="../assets/women.jpg" alt="">
                        <span class="message-line">I am Jarina, better half of Sahin. Who are you talking with me?</span>
                    </div>
                    <div class="chat-message myself">
                        <span class="message-line">Sahin Notir pula koi? okeee doree felo na kheno?</span>
                    </div>
                </div>
                <div class="chat-typing">
                    <div class="search-box">
                        <input type="search" class="" placeholder="Aa">
                    </div>
                    <div class="icon-lists">
                        <i class='bx bxs-send icon'></i>
                        <i class='bx bx-upload icon'></i>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    section{
        display: flex;
        align-items: center;
        justify-content: center;
        height: 98vh;
    }
        /* width */
    ::-webkit-scrollbar {
    width: 5px;
    }

    /* Track */
    ::-webkit-scrollbar-track {
    background: #b7b1ff;
    }

    /* Handle */
    ::-webkit-scrollbar-thumb {
    background: #d3cfff;
    }

    /* Handle on hover */
    ::-webkit-scrollbar-thumb:hover {
    background: #555;
    }
    .container{
        background: #a29bfe;
        width: 1000px;
        display: flex;
        border-radius: 5px;
    }
    .left-content{
        min-width: 300px;
        width: 300px;
        padding: 15px;
        overflow: hidden;
    }
    .search-box{
        position: relative;
    }
    .search-box .search-field{
        width: 100%;
        height: 35px;
        border-radius: 5px;
        color: #222;
        font-size: 14px;
        border: none;
        outline: none;
        padding: 0 15px 0 40px;
    }
    .search-box .search-icon{
        position: absolute;
        top: 7px;
        left: 10px;
        font-size: 20px;
        color: #888;
    }
    .chat-lists {
        margin-top: 15px;
        min-height: 400px;
        height: 400px;
        overflow-y: auto;
        border-top: 1px solid #b7b1ff;
        overflow-x: hidden;
    }
    .chat-lists .single-list{
        display: flex;
        align-items: center;
        gap: 10px;
        width: 100%;
        border-bottom: 1px solid #b7b1ff;
        padding: 7px 0;
        cursor: pointer;
    }
    .chat-lists .single-list .chat-img{
        min-width: 60px;
        width: 60px;
        height: 60px;
        object-fit: cover;
        border-radius: 50%;
    }
    .chat-lists .single-list .text{
        width: 100%;
    }
    .chat-lists .single-list .chat-name{
        color: #222;
        margin: 0;
        font-size: 16px;
        margin-bottom: 8px;
        font-weight: normal;
    }
    .chat-lists .single-list .chat-message{
        white-space: nowrap;
        text-overflow: ellipsis;
        overflow: hidden;
        width: 70%;
        font-size: 14px;
        margin: 0;
        color: #666;
    }








    .right-content{
        border-left: 1px solid #b7b1ff;
        width: 100%;
        overflow: hidden;
    }
    .top-contents{
        display: flex;
        align-items: center;
        justify-content: space-between;
        border-bottom: 1px solid #b7b1ff;
        width: 95%;
        padding: 10px 15px;
    }
    .top-contents .chat-info{
        display: flex;
        align-items: center;
        gap: 10px;
    }
    .top-contents .chat-img{
        min-width: 45px;
        width: 45px;
        height: 45px;
        border-radius: 50%;
        object-fit: cover;
    }
    .top-contents .chat-name{
        font-size: 16px;
        color: #222;
        margin: 0;
    }
    .top-contents .icon-lists{
        display: flex;
        align-items: center;
        gap: 20px;
    }
    .top-contents .icon-lists i{
        color: #6c5ce7;
        font-size: 24px;
        cursor: pointer;
    }





    .search-box{
        width: 100%;
        margin-right: 5px;
    }
    .search-box input{
        height: 40px;
        padding: 0 15px;
        color: #222;
        outline: none;
        width: 100%;
        border: none;
        border-radius: 5px;
    }
    .icon-lists{
        width: 20%;
    }
    .icon-lists .icon{
        font-size: 16px;
        width: 40px;
        height: 40px;
        background: #6c5ce7;
        border-radius: 50%;
        line-height: 40px;
        text-align: center;
        color: #fff;
        margin: 0 5px;
        cursor: pointer;
    }
    .chat-typing {
        display: flex;
        align-items: center;
        padding: 10px 15px 0;
        border-top: 1px solid #b7b1ff;
    }











    .chat-body {
        height: 350px;
        overflow-y: auto;
        overflow-x: hidden;
        padding: 0 10px;
    }
    .chat-body .chat-message.myself{
        justify-content: flex-end;
    }
    .chat-body .chat-message{
        display: flex;
        gap: 10px;
        justify-content: flex-start;
        align-items: flex-end;
        margin: 10px 0;
    }
    .chat-body .chat-message img{
        width: 30px;
        height: 30px;
        object-fit: cover;
        border-radius: 50%;
    }
    .chat-body .chat-message .message-line{
        font-size: 14px;
        color: #222;
        background: #b9b3ff;
        padding: 5px 10px;
        border-radius: 5px;
        max-width: 80%;
        line-height: 20px;
    }
</style>