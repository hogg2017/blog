<p>
`<addr>`
        <template v-for="(fragment, i) in text.toString().split(new RegExp(`(?<=${searchText})|(?=${searchText})`, 'i'))">
          <mark v-if="fragment.toLowerCase() === searchText.toLowerCase()" :key="i" class="highlight">{{fragment}}</mark>
          <template v-else>{{fragment}}</template>
        </template>
`</addr>`
</p>        
<p>
`<addr>`
?<=${searchText})|(?=${searchText})
?<= 表示匹配以 （）开头的字符串，并且捕获到分组中；
?=表示匹配以（）结尾的字符串，并且捕获到分组中；
`</addr>`
</p>
        