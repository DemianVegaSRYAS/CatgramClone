    <template>
        <div class="Left">
        <div class="profileName">
            Profile Name
        </div>
        <button type='button' class="Create">
            Create New Post
        </button>
        <div class="contentLeft_wrapp">
            Content
        </div>
        </div>
    </template>
    
    <script>
    export default {
        name: 'Left',
    }
    </script>
    
    <!-- Add "scoped" attribute to limit CSS to this component only -->
    <style scoped>
    .Left{
        background-color: rgb(0, 0, 0);
        height: 80vh;
        color: white;
        margin: 0;
        padding: 0.5em;
    }
    .profileName{
        height: 100px;
        background-color: rgba(103, 103, 103, 0.466);
        border-radius: 5px;
    }
    .Create{
        margin-top: 0.5em;
        color: white;
        background-color: #3B82F6;
        border-radius: 5px;
        width: 100%;
        height: 1.8em;
        font-size: 1.5em;
        font-weight: 500;
    }
    .contentLeft_wrapp{
        margin-top: 0.5em;

        background-color: rgba(103, 103, 103, 0.466);
        border-radius: 5px;
        min-height: 45vh;
    }
    </style>
    