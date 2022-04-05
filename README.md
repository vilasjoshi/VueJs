Vue JS:


Vue :
- Create Dynamic Applications
- Tools for Code Orgnization
- Speed of Development
- Developer Tools
- Helps with Scaling

:: Features & Benefits ::

- Virtula DOM (makes JS web application faster)
- LightWeight
- Progressive(means can be used at anywhere anytime in project for small part of project to fully dependent on VueJS Lib)
- Flexible(to use lib provided by Vue or other)
- Incrementally adoptable(can be added to existing project step by step without any issue)


:: VUE3 SETUP::

1.CDN : <script src="https://unpkg.com/vue@3"></script>

:: VUEJs Directive :: 

- it is way to connect elements from html to vuesjs object/data
 * v-model :- two way data binding, used to  to variable from vue to template componet
    ```
     <input type="text" v-model = "greeting">

    ```
 * v-if  :- used for conditional rendering
    ```
        <div id="app" >
            <div v-if = "isVisible"> This is conditional rendering</div>
        </div>

        <script src="https://unpkg.com/vue@3"></script>
        <script>
            let app = Vue.createApp({
                data: function(){
                    return {
                        greeting : "Hello Vue3 JS !",
                        isVisible : true
                    }
                }
            })
            app.mount('#app')
        </script>
    ```
