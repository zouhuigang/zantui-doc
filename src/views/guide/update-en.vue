<style>
    .doc-update .ivu-timeline .ivu-timeline-item-content{
        top: -14px;
    }
    .doc-update h2{
        margin: 0;
        font-weight: normal;
    }
    .doc-update code{
        margin: 8px 0 10px;
    }
    .doc-update ul{
        padding-left: 22px !important;
    }
    .doc-update-important{
        color: #3399ff;
    }
    .doc-update-loop.ivu-load-loop{
        animation-duration: 3s;
    }
</style>
<template>
    <i-article>
        <h1>Change Log</h1>
        <article class="doc-update">
            <Timeline pending>
                <Timeline-item color="green">
                    <Icon type="ios-trophy" size="18" slot="dot"></Icon>
                    <inAnchor title="3.0.0 Battleheart" h2></inAnchor>
                    <p>
                        <code>2018-07-28</code>
                    </p>
                    <h2>New Components</h2>
                    <ul>
                        <li>Add new component <code>Time</code>。<issue id="3645"></issue> <router-link to="/components/time-en">View</router-link></li>
                        <li>Add new component <code>Anchor</code>。<issue id="3369"></issue> <router-link to="/components/anchor-en">View</router-link></li>
                        <li>Add new component <code>Split</code>。<issue id="3844"></issue> <router-link to="/components/split-en">View</router-link></li>
                        <li>Add new component <code>Divider</code>。<issue id="3275"></issue> <router-link to="/components/divider-en">View</router-link></li>
                        <li>Add new component <code>Cell</code>。<router-link to="/components/cell-en">View</router-link></li>
                    </ul>
                    <h2>UI</h2>
                    <ul>
                        <li>Optimize the Collapse component style to look cleaner and fresher.</li>
                        <li>Optimize the Switch component style and make the dimensions more coordinated.</li>
                        <li>Optimize the Page component for a more concise style.</li>
                        <li>Optimize the Poptip / Tooltip components styles and the arrows are clearer.</li>
                        <li>Optimized the Tag component style and added a variety of preset colors.</li>
                        <li>Optimize the Alert component style, color and icons are more intuitive.</li>
                        <li>Optimize the Message / Notice components style to look cleaner and fresher.</li>
                        <li>Optimize the Modal and $Modal components style to look more coordinated.</li>
                        <li>Optimize the Menu style.</li>
                        <li>Optimize the Select style.</li>
                        <li>The default color of the Circle and Progress components is changed to the primary color, keeping the color uniform.</li>
                    </ul>
                    <h2>New Features</h2>
                    <br>
                    <h3>Global Settings</h3>
                    <ul>
                        <li>When using iView, you can make some properties of the global configuration component, for example:</li>
                        <i-code lang="auto" bg>{{ code.global.example }}</i-code>
                        Currently only supports the transfer and size properties. The component will use the properties set by prop first, and if not, then use the global configuration.
                    </ul>
                    <h3>Icon:</h3>
                    <ul>
                        <li>Upgrade to the <code>ionicons</code> 3.0 icon.</li>
                        <li>Add new property <code>custom</code>, now you can customize the icons. <issue id="3568"></issue> </li>
                    </ul>
                    <h3>Button:</h3>
                    <ul>
                        <li>Add new property <code>custom-icon</code>, now you can customize the icons of button.</li>
                        <li>Add new properties <code>to</code>, <code>replace</code>, <code>target</code>, support click to jump directly.</li>
                        <li>Add new property <code>ghost</code>, the button background can be made transparent and is often used on colored backgrounds.</li>
                    </ul>
                    <h3>Input:</h3>
                    <ul>
                        <li>Add new properties <code>prefix</code> and <code>suffix</code> , and the same named slot, support for setting the prefix and suffix icon.</li>
                        <li>Add new properties <code>search</code> and <code>enterButton</code>, support for input types of search boxes.</li>
                        <li>Add new event <code>@on-search</code>, when using the search type, trigger when you click search button or press the Enter key.</li>
                    </ul>
                    <h3>Modal:</h3>
                    <ul>
                        <li>Add new property <code>fullscreen</code>.</li>
                        <li>Add hidden mask layer property <code>mask</code>.</li>
                        <li>Add new property <code>draggable</code>.</li>
                    </ul>
                    <h3>Table:</h3>
                    <ul>
                        <li>Column add new property <code>indexMethod</code>, you can customize the index when use <code>type="index"</code> .</li>
                        <li>Column add new property <code>tooltip</code>, if open it, when the cell text exceeds one line, it will be displayed in ... and the full content will be displayed in the Tooltip.</li>
                    </ul>
                    <h3>Menu:</h3>
                    <ul>
                        <li>Add new properties <code>to</code>, <code>replace</code>, and <code>target</code>, support click to jump directly.</li>
                    </ul>
                    <h3>Breadcrumb:</h3>
                    <ul>
                        <li>Add new property <code>target</code>。</li>
                    </ul>
                    <h3>Badge:</h3>
                    <ul>
                        <li>Add new property <code>show-zero</code>. <issue id="3654"></issue> </li>
                        <li>Add new property <code>text</code>, now you can customize the content of Badge.</li>
                        <li>Add new property <code>status</code>, the Badge can be set to a status point.</li>
                        <li>Add new property <code>offset</code>, you can set the position.</li>
                        <li>Add new property <code>type</code>, the preset color can be set.</li>
                    </ul>
                    <h3>Page:</h3>
                    <ul>
                        <li>Add new property <code>prev-text</code> and <code>next-text</code>, you can customize the copy of the upper and lower pages.</li>
                    </ul>
                    <h3>Upload:</h3>
                    <ul>
                        <li>Add new property <code>paste</code>, after opening, you can upload files copied to the clipboard.</li>
                    </ul>
                    <h3>Tooltip:</h3>
                    <ul>
                        <li>Add new property <code>theme</code>, you can set either dark (default) or light.</li>
                        <li>Add new property <code>max-width</code>, when the maximum value is exceeded, the text will automatically wrap and be aligned.</li>
                    </ul>
                    <h3>Poptip:</h3>
                    <ul>
                        <li>Add new property <code>word-wrap</code>, when turned on, text that exceeds the specified width will automatically wrap and be aligned.</li>
                        <li>Add new property <code>padding</code>, you can customize the spacing value.</li>
                    </ul>
                    <h3>Rate:</h3>
                    <ul>
                        <li>Add new property <code>character</code>, <code>icon</code> and <code>custom-icon</code>, support for custom characters or icons.</li>
                    </ul>
                    <h3>Collapse:</h3>
                    <ul>
                        <li>Add new property <code>hide-arrow</code>, you can hide the arrows.</li>
                        <li>Add new property <code>simple</code>, can be displayed as a clean mode without borders.</li>
                    </ul>
                    <h3>Switch:</h3>
                    <ul>
                        <li>Add new property <code>loading</code>, it can be said that the switch is still being executed.</li>
                    </ul>
                    <h3>Tag:</h3>
                    <ul>
                        <li>There are 13 new presets added to the <code>color</code> property.</li>
                    </ul>
                    <h3>Dropdown:</h3>
                    <ul>
                        <li>Trigger mode <code>trigger</code> add <code>contextMenu</code>, which can be triggered by right clicking.</li>
                    </ul>
                    <h3>Circle:</h3>
                    <ul>
                        <li>Add new property <code>dashboard</code>.</li>
                    </ul>
                    <h3>Progress:</h3>
                    <ul>
                        <li>Added the segmentation progress property <code>success-percent</code>.</li>
                    </ul>
                    <h3>Avatar:</h3>
                    <ul>
                        <li>Add custom icon property <code>custom-icon</code>.</li>
                    </ul>
                    <h2>Optimizations</h2>
                    <br>
                    <h3>Breadcrumb:</h3>
                    <ul>
                        <li>The href value of the `a` is displayed.</li>
                    </ul>
                    <h3>Page:</h3>
                    <ul>
                        <li>Optimize the logic for fast forward and fast backwards. <issue id="3965"></issue> </li>
                    </ul>
                    <h3>Table:</h3>
                    <ul>
                        <li>Checkbox is centered when <code>type="selection"</code>.</li>
                    </ul>
                    <h2>Others</h2>
                    <ul>
                        <li>Add Mongolian. <mention id="Ariunbold13"></mention> </li>
                    </ul>
                    <h2>Bug Fix</h2>
                    <ul>
                        <li>Fixed a bug where the active animation was not oriented correctly when Progress was vertical.</li>
                        <li>Fixed a bug where Carousel does not use v-model when clicking on the indicator and the indicator is not updated.</li>
                        <li>Fixed a bug that Carouse loop is invalid.</li>
                    </ul>
                    <h2>Breaking Changes</h2>
                    <ul>
                        <li>Button discards type <code>ghost</code>, the original default style has changed.</li>
                        <li>The Icon is upgraded to the <code>ionicons</code> 3.0, icon and the icon's name has changed.</li>
                        <li>Breadcrumb discards the <code>href</code> property.</li>
                        <li>Badge's count property only supports the Number type.</li>
                        <li>The color property of Tag renames the original <code>blur</code>, <code>green</code>, <code>yellow</code>, <code>red</code> to <code>primary</code>, <code>success</code>, <code>warning</code>, <code>error</code>.</li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Button size="large" @click="handleBefore">View 2.x Change Log</Button>
                </Timeline-item>
            </Timeline>
        </article>
    </i-article>
</template>
<script>
    import iArticle from '../../components/article.vue';
    import iCode from 'iCode';
    import Code from '../../code/guide';
    import inAnchor from '../../components/anchor.vue';
    import issue from '../../components/issue.vue';
    import mention from '../../components/mention.vue';

    import version from '../../config/config';

    export default {
        components: {
            iArticle,
            iCode,
            inAnchor,
            issue,
            mention
        },
        data () {
            return {
                code: Code
            }
        },
        mounted () {
            window.localStorage.setItem('version', version.version);
        },
        methods: {
            handleBefore () {
                window.open('http://v2.iviewui.com/docs/guide/update-en');
            }
        }
    }
</script>