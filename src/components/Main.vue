<template>
    <div>
        <main>
            <div class="first">
                <h2>WordPressで何が作れるんだろう？</h2>
                <p class="first-content">これからWordPressを勉強する人のために何ができるかをいくつか説明します。</p><!--/.first-content-->
            </div><!--/.first-->
            <div class="articles-wrap">
                <ul class="articles">
                    <li 
                        class="article"
                        v-for="list in lists"
                        :key=list.id
                    >
                        <div class="wrap">
                            <img :src="list.image">
                            <p>{{list.number}}</p>
                        </div><!--/.wrap-->
                        <p class="article-content">{{list.title}}</p><!--/.article-content-->
                    </li><!--/.article-->
                </ul><!--/.artilces-->
            </div><!--/.articles-wrap-->
            <p class="comment">WordPressでできることはまだまだいっぱいありますが基本的な内容を作れるようにしてからカスタムできるようにした方がいいです。<br>WordPressでできることはまだまだいっぱいありますが基本的な内容を作れるようにしてからカスタムできるようにした方がいいです。コーディングができないとWordPressを使ったサイトを作ることができないのでコーディングを継続してやるようにしましょう。</p><!--/.comment-->
        </main>
    </div>
</template>

<script>
    export default{
        data:function(){
            return{
                lists:[
                    {
                        number:'その1',
                        image:require('@/assets/images/profile.png'),
                        title:'プロフィールについて'
                    },
                    {
                        number:'その2',
                        image:require('@/assets/images/main.png'),
                        title:'メインページについて'
                    },
                    {
                        number:'その3',
                        image:require('@/assets/images/single.png'),
                        title:'投稿ページについて'
                    },
                    {
                        number:'その4',
                        image:require('@/assets/images/side-bar.png'),
                        title:'サイドバーについて'
                    },
                    {
                        number:'その5',
                        image:require('@/assets/images/page.png'),
                        title:'固定ページについて'
                    },
                    {
                        number:'その6',
                        image:require('@/assets/images/category.png'),
                        title:'カテゴリーについて'
                    },
                ]
            }
        }
    }
</script>