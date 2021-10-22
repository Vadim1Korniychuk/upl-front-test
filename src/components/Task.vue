<template>
    <div class="task-page">
        <h1 class="title">Task list</h1>
        <div class="tasks">
            <div class="task priority-high">
                <h2>{{task.title}}</h2>
                <p>{{task.description}}</p>
                <div class="tags">
                    <span>Тестове</span>
                </div>
            </div>
            <div class="task priority-high">
                <h2>{{task.title}}</h2>
                <p>{{task.description}}</p>
                <div class="tags">
                    <span>Тестове</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data () {
            return {
                task: {
                    "id": 1,
                    "title": "List/detail for Tags",
                    "description": "List/detail for Tags",
                    "priority": "HIGH",
                    "status": "IN_PROGRESS",
                    "tags": [
                        {
                            "id": 1,
                            "name": "Тестове",
                            "created": "2021-10-22T12:26:49.984620Z",
                            "updated": "2021-10-22T12:26:49.984753Z"
                        }
                    ],
                    "created": "2021-10-22T12:26:49.987504Z",
                    "updated": "2021-10-22T12:26:49.987602Z"
                },
            }
        },
        methods : {}
    };
</script>

<style scoped lang="scss">
.tasks {
    display: flex;
    flex-wrap: wrap;
}
.task {
    display: flex;
    flex-direction: column;
    background: #fff;
    border-radius: 4px;
    height: 300px;
    margin: 1rem;
    padding: 1rem;
    position: relative;
    width: 300px;
    box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23);
}
.tags {
    margin-top: auto;
}
.tags span{
    background: #e3c9c9;
    border-radius: 12px;
    display: inline-block;
    padding: .4rem;
    box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23);
}
</style>
