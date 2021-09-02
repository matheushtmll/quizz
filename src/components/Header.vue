<template>
    <div>
         <b-nav tabs>
            <b-nav-item disabled><b>Damdam Quizz App</b></b-nav-item>
            <b-nav-item disabled>Respostas: {{numCorrect}}/{{numTotal}}</b-nav-item>
            <b-nav-item disabled>Dropdown</b-nav-item>
            <b-nav-item-dropdown>
                <b-nav-item>Click to Smille :D</b-nav-item>
                <b-nav-item>Love u</b-nav-item>
            </b-nav-item-dropdown>
            
        </b-nav>
    </div>
</template>

<script>

export default ({
    props: [
        'numCorrect',
        'numTotal'
    ]
})
</script>
