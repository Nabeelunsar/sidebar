
<template>
    <div class="section">
        <div class="column">
            <h2>Content</h2>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odio itaque cumque facere adipisci dolorem repudiandae velit eos minus esse deleniti vitae tenetur reiciendis beatae tempora hic sunt, praesentium iure eaque.</p>
        </div>
        <div class="column">
            <h2>Instruction</h2>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Hic error eaque, maxime id, deleniti, consequuntur necessitatibus et commodi nihil aliquid doloribus sapiente optio eius fugit iusto vel pariatur veritatis repellat.</p>
        </div>
        <div class="column">
            <h2> Code</h2>
            <div class="input-section">
                <textarea v-model="codeInput" placeholder="Enter code..">
                        </textarea>
                <button @click="submitCode">Submit</button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'BODYMAIN',
    data() {
        return {
            codeInput: "",
        };
    },
    methods: {
        submitCode() {
            console.log("submitted code:", this.codeinput);
        },
    },
};
</script>

<style scoped>
.section {
    display: flex;
    flex-wrap: wrap;
    /* margin: auto auto; */
    padding-top: 65px;
}


.column {
    background-color: white;
    padding: 20px;
    margin: 10px;
    box-sizing: border-box;
    text-align: center;
    height: 600px;
    width: 300px;
    border-radius: 12px;
    width: calc(33.3% - 20px);
    border: 2px solid grey;
}

.column p {
    margin-top: 20px;
}

.columnn h2 {
    color: orange
}

@media screen and (max-width:768px) {
    .column {
        width: 200px;
        height: 250px;
    }

    .input-section {
        margin-top: 20px;
        height: 50px;
        width: 200px;
        flex-direction: column;
    }
}

.input-section {
    margin-top: 20px;
}

textarea {
    width: 100%;
    padding: 8px 0 0 8px;
    height: 450px;
    resize: none;
    border-radius: 4px;
    border-color: grey;
}

button {

    display: block;
    margin-top: 10px;
    padding: 8px 16px;
    background-color: gray;
    color: azure;
    border: none;
    cursor: pointer;
    border-radius: 4px;
}
</style>