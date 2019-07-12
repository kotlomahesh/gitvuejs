 <template>      
 <h1> This is hari</h1>
<p :style="md">{{display}}</p>
<h2>{{vue()}}-<a :href="link">click here to know</a></h2>
FINISHED LINK  
<p v-html="fin"></p> 
<button @click="counter++">plus</button>
<p>{{counter}}</p>
<h1> hellikjdsjwakjfajdw</h1>	
<p v-on:mousemove="coordintaes"> Coordinates: {{ x }} / {{  y }}-<span v-on:mousemove.stop="">stop</span></p>
<p>{{kotlo}}</p>
<p v-html="n"></p>
name<input type="text" v-model="kotlo"><br><br>
<input type="text" v-model="hr">
<h1>{{hr}}</h1>
alert box<input type="text" v-on:keyup.space="alert">
<button v-on:click="decrease">increase</button>
<p>{{count}}</p>
<p>{{ updated code}}</p>
<p>{{result}}</p>
<h1>hie harinath</h1>
<span>hello</span>
</template>
<script>
export default{

    data(){
        return{
            display:"welcome to the tutorials point",
            title:"vue js learning",
            link:"hsr.html",
            fin:'<a href="hsr.html"> click me</a>',
            n:'<span> HI THIS IS THE HTML CODE</span><br> <h1> NAME IS DUMMY</h1>',
            counter:0,
            x:0,
            y:0,
            kotlo:"welcome", 
            hr:"HARINATH REDDY SADARA",
            count:0,
            result:"",
            md:{color:'red',background:'blue'}
                    }
    },
    created(){
    this.alert();
    },
    methods:{
    vue:function(){
     return this.title;
    }, 
increase:function(step){
   this.counter+=step;
},

coordintaes:function(item){
	this.x=item.clientX;
	this.y=item.clientY;
},
mahesh:function(event){
this.kotlo=event.target.value;
},
alert:function(){
	alert("HELLO!");
},
decrease(){
    this.count++;
    this.result=this.count > 5 ? 'greater than 5':'smaller than 5';
}
}
}
</script>