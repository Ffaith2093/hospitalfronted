<!--侦听器的代码分析-->
<template>
    <div id="example">
        <p>Oriainal message: "{{message}}"</p>
        <p>Computed reversed message: "{{message}}"</p>
    </div>
</template>

<script>
    var vm = new Vue({
        el: '#watch-example',
        data: {
            question: '',
            answer: 'I cannot give you an answer'
        },
        watch: {
            //如果question发生改变，则这个函数就会执行
            question: fuction (newQuestion, oldQuestion) {
                this.answer = 'waiting for you to ...'
                this.debouncedGetAnswer()
            }
        },
        created: function () {
            this.debouncedGetAnswer() = _.debounce(this.getAnswer, 500)
        },
        methods: {
            
        }
    })

        
</script>




