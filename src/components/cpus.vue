<template>
    <div>
        <p>
            <button class="component_label" v-on:click="toggleVisible()">CPUS go here</button>
            <span v-if="show">
                <ul>
                    <li v-for="cpu in theCPUS" :key="cpu.name">
                        {{cpu.name}}: ${{cpu.price}}
                    </li>
                </ul>
            </span>
        </p>
    </div>
</template>

<script>
export default {
    name: "CPUs",
    data() {
        return {
            theCPUS: [{
                name: "cpu 1",
                price: 100
            },
            {
                name: "cpu 2",
                price: 150
            }
            ],
            show: false
        }
    },
    methods: {
        toggleVisible() {
            if (this.show == true) {
                this.show = false
            }
            else {
                this.show = true
            }
        }
    }
}
</script>