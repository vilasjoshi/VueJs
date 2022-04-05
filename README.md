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

:: VueJs Directive :: 

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
 * v-else-if  :- 
            v-else-if="varible"
 
 * v-else : do not take any variable.



 * v-show  :- is also used to show/hide element on the screen/html. 
              Difference between v-if and v-show is that v-if does not render on html. but v-show get render on the html DOM but can be hidden on page, but style display set to none.(can be seen inspect element tool).
              This can be use where we need to toggle something.
  

:: Events and Methods :: 

 * Events : browser captured events - clicks, double click, mouse motion, hover, keypress etc
    * v-on :- help to listem DOM events and run Javascript.

    ```
    <div id="app" >
       
        <div v-if = "isVisible"> This is conditional rendering</div>
        <button v-on:click ="isVisible = !isVisible">Show Box</button>

    </div>

      <script src="https://unpkg.com/vue@3"></script>

    <script>
        let app = Vue.createApp({
            data: function(){
                return {
                    greeting : "Hello Vue3 JS !",
                    isVisible : true,
                    isShow : false
                }
            }
        })
        app.mount('#app')
    </script>


    ```