<template>
  <header>
    <h1>vue-reading-time</h1>
    <section>
      <img alt="npm" src="https://img.shields.io/npm/v/vue-reading-time"> <img alt="npm" src="https://img.shields.io/npm/dt/vue-reading-time">

    <p>vue-reading-time provides an estimate of how long an article or blog will take for the average adult to read.</p>
    </section>
    
  </header>
  <section>
    <h2>install</h2>
    <code>npm i vue-reading-time</code>
  </section>
  <section>
    <h2>Style</h2>
    <code>
      You can style component with the <span>.vue-reading-time</span> class
    </code>
    <small>or by adding some class</small>
    <code>
      &lt;vue-reading-time element=&quot;article-ref&quot; <span>class=&quot;my-class&quot;</span> /&gt;
    </code>
    <small>or using inline styles</small>
    <code>
      &lt;vue-reading-time element=&quot;article-ref&quot; <span>style=&quot;border:1px solid red</span> /&gt;
    </code>
  </section>
  <section>
    <h2>Demo</h2>
    <h3>Try some style:</h3>
    <pre class="edit-area">.vue-reading-time {</pre>
    <textarea ref="code" @input="updateHeight" v-model="myClass"></textarea>
    <pre>}</pre>
    <svg class="point-draw" id="Layer_1" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 51.76 169.82">
      <g>
        <path class="acls-1" d="m36.1.5s-.34.38-.97,1.14"/>
        <path class="acls-3" d="m33.27,4.02C25.83,13.94,5.95,44.76,1.1,96.5c-5.64,60.18,30.2,63.77,40.99,63.5"/>
        <path class="acls-1" d="m43.61,159.94c.95-.06,1.49-.14,1.49-.14"/>
      </g>
      <g>
        <path class="acls-1" d="m40.67,150.74c.04.15.23.66.6,1.37"/>
        <path class="acls-2" d="m42.91,154.7c1.7,2.26,4.39,4.79,8.19,5.58.22.05.21.39-.01.43-3.92.77-7.73,2.13-10.35,5.95"/>
        <path class="acls-1" d="m39.93,167.97c-.23.43-.45.88-.65,1.35"/>
      </g>
    </svg>
  </section>  
  <article ref="articleID">
    <h3>Preview - 
     Paragraphs: <select name="count" v-model="pCount">
        <option value="1">1</option>
        <option value="2">2</option>
        <option value="3">3</option>
        <option value="4">4</option>
        <option value="5">5</option>
        <option value="6">6</option>
        <option value="7">7</option>
        <option value="8">8</option>
        <option value="9">9</option>
        <option value="10">10</option>
      </select>
    </h3>
    
    <h1>Lorem ipsum dolor sit amet</h1>
    <vue-reading-time v-if="renderComponent" element="articleID" :style="myClass"/>
    <h2>Consectetur adipisicing elit. Maxime laudantium consequuntur modi accusantium repudiandae similique illo ipsa id
      voluptatem.</h2>
    <p v-for="p in paragraphs.slice(0,pCount)">
      {{ p }}
    </p>
  </article>

  <section>
    <p>Give a star on Github ★</p>
    <a href="https://github.com/BoraKucukkara/vue-reading-time" target="_blank">https://github.com/BoraKucukkara/vue-reading-time</a>
  </section>

  <section>
    <p>Report Bug/Issue</p>
    <a href="https://github.com/BoraKucukkara/vue-reading-time/issues" target="_blank">https://github.com/BoraKucukkara/vue-reading-time/issues</a>
  </section>

  <a href="https://www.npmjs.com/package/vue-reading-time">
    <svg class="npm-logo" id="Layer_1" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 332.29 332.29">
      <polygon class="cls-1" points="135.76 0 0 0 332.29 332.29 332.29 196.53 135.76 0"/>
      <g>
        <polygon class="cls-2" points="117.18 79.7 134.09 96.61 159.45 71.25 167.91 79.7 142.54 105.06 151 113.52 184.81 79.7 151 45.89 117.18 79.7"/>
        <polygon class="cls-2" points="252.45 214.97 286.26 181.15 235.54 130.43 201.72 164.24 218.63 181.15 243.99 155.79 252.45 164.24 227.08 189.6 235.54 198.06 260.9 172.7 269.35 181.15 243.99 206.51 252.45 214.97"/>
        <path class="cls-2" d="m193.27,155.79l33.82-33.82-33.82-33.82-41.95,41.95,16.91,16.91,8.13-8.13,16.91,16.91Zm8.45-42.27l8.45,8.45-16.91,16.91-8.45-8.45,16.91-16.91Z"/>
      </g>
    </svg>
  </a>

  <div class="copyright">
    <a href="https://github.com/BoraKucukkara/vue-reading-time" title="Bora Kucukkara / vue-article-reading-time on Github">
      <svg height="24" style="fill:rgb(128, 128, 129)" aria-hidden="true" viewBox="0 0 16 16" version="1.1" width="24" data-view-component="true" class="octicon octicon-mark-github v-align-middle">
        <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path>
      </svg>
    </a>
    <a href="https://www.borakucukkara.com/" title="Bora Kucukkara personal web site">
      <img src="https://www.borakucukkara.com/borakucukkara.png" width="24">
    </a>
  </div>
</template>

<script>
import { VueReadingTime } from 'vue-reading-time'
export default {
  data() {
    return {
      myClass: `color:coral;
border:1px solid coral;
font-size: .8rem;
padding: .2rem .5rem;
display:inline;
border-radius:.5rem;`,
      paragraphs: [
        "Aenean non aliquam ligula, vel tristique lectus. Sed eu risus ipsum. Sed a suscipit eros. Sed rhoncus ac velit non molestie. Duis consequat odio id finibus dictum. Vivamus posuere ex vel nisi facilisis, id fringilla turpis finibus. Maecenas in quam volutpat erat varius ultricies ut et quam. Ut eu ligula malesuada, pretium lorem eu, fermentum purus.",
        "Curabitur ultrices fringilla dignissim. Pellentesque feugiat tincidunt orci, pretium condimentum leo convallis in. Sed finibus, sapien a ultricies venenatis, lacus diam tincidunt elit, nec venenatis dolor nunc a orci. Aliquam sed ornare eros, vel egestas orci. Vivamus erat tellus, fringilla ut justo non, maximus bibendum mi. Mauris malesuada, leo ut sodales pretium, ipsum elit hendrerit diam, vel pellentesque orci nisl vel libero. Sed cursus in ligula a ullamcorper. Quisque vitae dapibus odio. Donec eget dictum purus. Praesent fringilla, leo in vulputate interdum, diam dolor aliquet ex, vel placerat neque erat et risus. Proin ut dui vel lacus condimentum porttitor et in tortor.",
        "Proin at risus sit amet lorem interdum mollis. Curabitur eget magna ultricies nibh vehicula faucibus et vel turpis. Nullam vel imperdiet ante. Suspendisse potenti. Mauris sit amet tincidunt dolor. Nunc quis lorem in lectus luctus elementum. Integer sit amet eros in massa viverra consequat. Suspendisse ut est nec metus auctor commodo. Ut convallis massa in quam congue ultricies. Phasellus ante tortor, feugiat et sagittis id, eleifend id lacus. Praesent elementum est id tortor porta laoreet.",
        "Vivamus maximus tellus iaculis lectus pretium imperdiet. Nam nec blandit mi. Mauris et pulvinar neque. Maecenas ut augue eu urna sollicitudin eleifend. Sed vestibulum venenatis risus, vel suscipit nisi ullamcorper in. Vestibulum sodales scelerisque laoreet. Morbi semper ac neque sit amet accumsan. Quisque vulputate odio et rhoncus ornare. Aliquam erat volutpat. Fusce convallis magna vel ultrices tempus. Suspendisse bibendum, ante in faucibus bibendum, neque nisl commodo urna, ut efficitur lectus mauris eu purus. Integer porttitor tincidunt euismod. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Quisque nec varius velit. Sed est erat, tristique eu egestas vitae, pretium vitae tellus. Aliquam ultrices ultrices velit, ut commodo quam accumsan id.",
        "Donec varius, enim non consectetur pulvinar, libero enim rhoncus enim, quis egestas felis nisi vel quam. Morbi posuere accumsan orci, ut placerat orci congue vitae. Proin ornare nunc ex, in luctus quam consectetur vitae. Fusce ut tincidunt orci. Cras dictum mattis massa vitae egestas. Morbi tristique euismod magna. Vestibulum interdum tellus metus, eu dapibus odio fringilla ut. Mauris volutpat massa massa, auctor faucibus nisi sodales vel. Morbi mauris ex, pellentesque sed augue et, pretium fermentum massa. Aliquam dapibus suscipit tortor, vel rutrum ipsum faucibus eget. Aliquam erat volutpat.",
        "Proin nec risus consequat, consequat quam sed, interdum velit. Vivamus et felis commodo, dignissim magna quis, venenatis felis. Praesent sed egestas mauris. Aenean sed diam aliquet, feugiat justo et, consequat nulla. Donec ac laoreet nisi, nec luctus ipsum. Maecenas sed purus molestie ligula sollicitudin sollicitudin et nec lorem. Mauris vel diam eu nibh lacinia euismod. Morbi id rhoncus metus. Praesent arcu lorem, molestie at ipsum at, semper euismod sem. Suspendisse fermentum, libero ac blandit convallis, tortor leo porta mauris, ultricies varius tellus elit eu leo. Nunc pretium ex non purus lacinia, id bibendum augue congue. Morbi nec velit vitae eros sodales fringilla vel at nulla. Curabitur vitae pharetra dui. In ultricies sollicitudin mauris. In mi augue, pulvinar vel magna quis, semper laoreet magna.",
        "Ut a odio eu velit tempus dapibus. Aliquam vitae tortor ut eros pretium efficitur id sed lorem. Mauris posuere auctor sem, sed hendrerit urna rhoncus vitae. Praesent varius eros sapien, ac convallis enim blandit ac. Donec semper pharetra lectus. Sed ultricies magna vitae mollis porta. Cras a sodales orci, id scelerisque elit. Quisque commodo felis ac consectetur tristique. Vivamus convallis nisi a lacus dictum dignissim at a turpis.",
        "Aenean ullamcorper purus nec metus rutrum placerat. Suspendisse aliquam mattis maximus. Donec cursus aliquam blandit. Vestibulum et gravida quam. Aliquam erat volutpat. Integer leo ligula, blandit vel bibendum et, consectetur at velit. Ut justo justo, interdum eu tempor ac, dignissim id magna. Aliquam erat volutpat. Pellentesque suscipit, nisi sed aliquam egestas, leo velit porttitor mi, a tincidunt libero felis sed metus.",
        "Vestibulum fermentum volutpat tempus. Praesent molestie ac nibh sed facilisis. Phasellus sed aliquet nisi. Vivamus ullamcorper neque sit amet purus dictum, molestie facilisis lectus tempus. Nam aliquet nibh ac mauris bibendum tempor. Integer gravida sed mi porta suscipit. Proin nec diam vitae odio semper sodales vel a mauris. Integer scelerisque enim nibh, vitae imperdiet quam pulvinar vitae.",
        "Maecenas viverra nisl purus, a porttitor nibh varius vitae. Suspendisse non placerat magna, nec tincidunt augue. Curabitur arcu nisi, semper nec fermentum blandit, tincidunt a purus. Proin ipsum nisi, laoreet eget velit ut, maximus varius sem. Donec vel lorem finibus, cursus lorem eget, placerat turpis. Vestibulum mattis varius euismod. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Morbi sapien tortor, aliquam sit amet augue vitae, imperdiet rutrum elit. Nullam commodo mollis nisl, eget finibus est interdum at. Fusce faucibus dolor eros, ac faucibus sapien tincidunt quis. Donec fringilla et nunc a posuere. Quisque facilisis massa libero, egestas ornare nunc molestie nec. In interdum ex eu purus dictum, vel euismod ex varius. Proin vestibulum leo sit amet mattis auctor. Vivamus dapibus ut elit a tincidunt.",
      ],
      pCount: 3,
      renderComponent: true
    }
  },
  components:{
    VueReadingTime
  },
  methods: {
    focusTextArea() {
      this.$refs.code.focus()
    },
    updateHeight() {
      let codeArea = this.$refs.code
      codeArea.style.height = ""
      codeArea.style.height = Math.min(codeArea.scrollHeight) + "px";
    },
    async forceRender() {
      this.renderComponent = false;
      await this.$nextTick();
      this.renderComponent = true;
    }
  },
  watch:{
    pCount(newVal, oldVal) {
      if(newVal != oldVal) {
        this.forceRender()
      }
    }
  },
  mounted(){
    this.focusTextArea()
  }
}
</script>

<style>
.copyright { position: fixed; bottom:1rem; right:1rem;}
.copyright a {padding: .3rem; opacity: .7; transition: all .3s;}
.copyright a:hover {opacity: 1}
textarea {
  padding: 0;
  margin:0 0 0 1rem;
  width: 100%;
  outline: none;
  border: none;
  resize: none;
  line-height: 1.5;
  background: none;
  height: 120px;
  color:rgb(255, 227, 202);
}
textarea:focus {
  color: #fff;
}
.edit-area {position: relative;}
.edit-area:after {
  content:"Edit Css Here_";
  margin:0 0 0 .5rem;
  padding: .2rem .5rem;
  font-size: .7rem;
  color:#a7a7a7;
  border-radius: .4rem;
  border: 1px solid #606060;
  z-index: 10;
}
section {
  padding: 1rem;
  margin:0;
  border-bottom: 1px dashed #555;
}
article {
  padding: 1rem 2rem;
  border:1px solid #ffffff22;
  border-radius: 1rem;
  max-width: 700px;
  margin:1rem 1rem;
}
span {color:coral}
code {
  border:.14rem solid #363636;
  border-radius: .5rem;
  padding: .5rem 1rem;
  display: block;
  background: #292929;
  color:#eee;
  margin:.4rem 0
}
pre {
  margin:0;
  padding: 0;
  color:coral;
  font-weight: bold;
  font-size: 1rem;
  outline: none;
}
select, select:focus, select:focus-visible, select:focus-within {
  padding: .3rem .5rem;
  background-color: #292929;
  color:#eee;
  border-radius: .3rem;
  outline: none;
  
}
.point-draw {
  position: absolute;
  width: 10rem;
  height: 20rem;
  margin: -4.5rem 0 0 -9rem;
}
.cls-1 {
  fill: #dd222e;
}
.cls-1, .cls-2 {
  stroke-width: 0px;
}
.cls-2 {
  fill: #fff;
}
.npm-logo {
  position: absolute;
  top:0;
  right: 0;
  width: 5rem;
  height: 5rem;
  position: fixed;

}
.acls-1, .acls-2, .acls-3 {
        fill: none;
        stroke: #666;
        stroke-linecap: round;
        stroke-linejoin: round;
      }

      .acls-2 {
        stroke-dasharray: 0 0 3.06 3.06;
      }

      .acls-3 {
        stroke-dasharray: 0 0 3.03 3.03;
      }
</style>
