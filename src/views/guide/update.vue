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
        <h1>更新日志</h1>
        <article class="doc-update">
            <Timeline pending>
                <Timeline-item color="green">
                    <Icon type="ios-trophy" size="18" slot="dot"></Icon>
                    <inAnchor title="3.0.0 Battleheart" h2></inAnchor>
                    <p>
                        <code>2018-07-28</code>
                    </p>
                    <h2>新增组件</h2>
                    <ul>
                        <li>相对时间组件 <code>Time</code>。<issue id="3645"></issue> <router-link to="/components/time">查看组件</router-link></li>
                        <li>锚点组件 <code>Anchor</code>。<issue id="3369"></issue> <router-link to="/components/anchor">查看组件</router-link></li>
                        <li>面板分割组件 <code>Split</code>。<issue id="3844"></issue> <router-link to="/components/split">查看组件</router-link></li>
                        <li>分割线组件 <code>Divider</code>。<issue id="3275"></issue> <router-link to="/components/divider">查看组件</router-link></li>
                        <li>单元格组件 <code>Cell</code>。<router-link to="/components/cell">查看组件</router-link></li>
                    </ul>
                    <h2>UI</h2>
                    <ul>
                        <li>优化 Collapse 组件样式，看起来更简洁、清新。</li>
                        <li>优化 Switch 组件样式，尺寸更协调了。</li>
                        <li>优化 Page 组件样式，风格更简洁。</li>
                        <li>优化 Poptip / Tooltip 组件样式，箭头更清晰了。</li>
                        <li>优化了 Tag 组件样式，增加多种预设的颜色。</li>
                        <li>优化 Alert 组件样式，配色和图标更直观好看了。</li>
                        <li>优化 Message / Notice 组件样式，看起来更简洁、清新。</li>
                        <li>优化 Modal、$Modal 样式，看起来更协调了。</li>
                        <li>优化 Menu 样式。</li>
                        <li>优化 Select 样式。</li>
                        <li>Circle 和 Progress 组件的默认色改为了主色，保持配色统一。</li>
                    </ul>
                    <h2>新特性</h2>
                    <br>
                    <h3>全局配置</h3>
                    <ul>
                        <li>使用 iView 时，可以进行全局配置组件的一些属性，例如：</li>
                        <i-code lang="auto" bg>{{ code.global.example }}</i-code>
                        目前只支持配置 transfer 和 size 两个属性。组件会优先使用 prop 设置的属性，如果未设置，再使用全局配置。
                    </ul>
                    <h3>Icon 图标：</h3>
                    <ul>
                        <li>升级至 <code>ionicons</code> 3.0 图标。</li>
                        <li>新增属性 <code>custom</code>，支持自定义图标。<issue id="3568"></issue> </li>
                    </ul>
                    <h3>Button 按钮：</h3>
                    <ul>
                        <li>新增属性 <code>custom-icon</code>，支持自定义图标。</li>
                        <li>新增属性 <code>to</code>、<code>replace</code>、<code>target</code>，支持点击直接跳转。</li>
                        <li>新增幽灵属性 <code>ghost</code>，可以使按钮背景透明，常用于有色背景上。</li>
                    </ul>
                    <h3>Input 输入框：</h3>
                    <ul>
                        <li>新增属性 <code>prefix</code> 和 <code>suffix</code> 以及同名 slot，支持设置前缀和后缀图标。</li>
                        <li>新增属性 <code>search</code> 和 <code>enterButton</code>，支持搜索类型的输入框。</li>
                        <li>新增事件 <code>@on-search</code>，使用搜索类型输入框时，点击搜索或按下回车键时触发。</li>
                    </ul>
                    <h3>Modal 对话框：</h3>
                    <ul>
                        <li>新增全屏属性 <code>fullscreen</code>。</li>
                        <li>新增隐藏遮罩层属性 <code>mask</code>。</li>
                        <li>新增拖拽属性 <code>draggable</code>。</li>
                    </ul>
                    <h3>Table 表格：</h3>
                    <ul>
                        <li>Column 新增属性 <code>indexMethod</code>， 可以自定义 <code>type="index"</code> 时的序号。</li>
                        <li>Column 新增属性 <code>tooltip</code>，开启后，当单元格文本超过一行，会以…显示，并在 Tooltip 中显示完整内容。</li>
                    </ul>
                    <h3>Menu 菜单：</h3>
                    <ul>
                        <li>新增属性 <code>to</code>、<code>replace</code>、<code>target</code>，支持点击直接跳转。</li>
                    </ul>
                    <h3>Breadcrumb 面包屑：</h3>
                    <ul>
                        <li>新增属性 <code>target</code>。</li>
                    </ul>
                    <h3>Badge 徽章：</h3>
                    <ul>
                        <li>新增属性 <code>show-zero</code>。<issue id="3654"></issue> </li>
                        <li>新增属性 <code>text</code>，可以自定义内容。</li>
                        <li>新增属性 <code>status</code>，可以设置徽标为状态点。</li>
                        <li>新增属性 <code>offset</code>，可以设置偏移量。</li>
                        <li>新增属性 <code>type</code>，可以设置预设的颜色。</li>
                    </ul>
                    <h3>Page 分页：</h3>
                    <ul>
                        <li>新增属性 <code>prev-text</code> 和 <code>next-text</code>，可以自定义上下页的文案。</li>
                    </ul>
                    <h3>Upload 上传：</h3>
                    <ul>
                        <li>新增属性 <code>paste</code>，开启后可以上传复制在剪贴板的文件。</li>
                    </ul>
                    <h3>Tooltip 文字提示：</h3>
                    <ul>
                        <li>新增属性 <code>theme</code>，可以设置 dark（默认）或 light 两种主题。</li>
                        <li>新增属性 <code>max-width</code>，超出最大值后，文本将自动换行，并两端对齐。</li>
                    </ul>
                    <h3>Poptip 气泡提示：</h3>
                    <ul>
                        <li>新增属性 <code>word-wrap</code>，开启后，超出指定宽度文本将自动换行，并两端对齐。</li>
                        <li>新增属性 <code>padding</code>，可以自定义间距值。</li>
                    </ul>
                    <h3>Rate 评分：</h3>
                    <ul>
                        <li>新增属性 <code>character</code>、<code>icon</code> 和 <code>custom-icon</code>，支持自定义字符或图标。</li>
                    </ul>
                    <h3>Collapse 折叠面板：</h3>
                    <ul>
                        <li>新增属性 <code>hide-arrow</code>，可以隐藏箭头。</li>
                        <li>新增属性 <code>simple</code>，可以显示为无边框的简洁模式。</li>
                    </ul>
                    <h3>Switch 开关：</h3>
                    <ul>
                        <li>新增属性 <code>loading</code>，可表示开关仍在执行中。</li>
                    </ul>
                    <h3>Tag 标签：</h3>
                    <ul>
                        <li><code>color</code> 属性新增了 13 种预设。</li>
                    </ul>
                    <h3>Dropdown 下拉菜单：</h3>
                    <ul>
                        <li>触发方式 trigger 新增 <code>contextMenu</code>，可以通过点击右键触发。</li>
                    </ul>
                    <h3>Circle 进度环：</h3>
                    <ul>
                        <li>新增仪表盘属性 <code>dashboard</code>。</li>
                    </ul>
                    <h3>Progress 进度条：</h3>
                    <ul>
                        <li>新增分段进度属性 <code>success-percent</code>。</li>
                    </ul>
                    <h3>Avatar 头像：</h3>
                    <ul>
                        <li>新增自定义图标属性 <code>custom-icon</code>。</li>
                    </ul>
                    <h2>优化</h2>
                    <br>
                    <h3>Breadcrumb 面包屑：</h3>
                    <ul>
                        <li>在链接上会显示 a 标签的 href 值。</li>
                    </ul>
                    <h3>Page 分页：</h3>
                    <ul>
                        <li>优化快进和快退的逻辑。<issue id="3965"></issue> </li>
                    </ul>
                    <h3>Table 表格：</h3>
                    <ul>
                        <li>优化 <code>type="selection"</code> 时，Checkbox 为居中。</li>
                    </ul>
                    <h2>其它</h2>
                    <ul>
                        <li>新增蒙古语。<mention id="Ariunbold13"></mention> </li>
                    </ul>
                    <h2>修复</h2>
                    <ul>
                        <li>修复 Progress 纵向时，active 动画方向不正确的 bug。</li>
                        <li>修复 Carousel 未使用 v-model 时，点击指示器，指示器不更新的 bug。</li>
                        <li>修复 Carousel 设置 loop 无效的 bug。</li>
                    </ul>
                    <h2>不兼容更新</h2>
                    <ul>
                        <li>Button 废弃 type <code>ghost</code>，原先的 default 样式有改变。</li>
                        <li>Icon 的图标升级至 <code>ionicons</code> 3.0 图标，图标名称有改变。</li>
                        <li>Breadcrumb 废弃 <code>href</code> 属性。</li>
                        <li>Badge 的 count 属性只支持 Number 类型。</li>
                        <li>Tag 的 color 属性将原先的 <code>blur</code>、<code>green</code>、<code>yellow</code>、<code>red</code> 更名为了 <code>primary</code>、<code>success</code>、<code>warning</code>、<code>error</code>。</li>
                    </ul>
                </Timeline-item>
                <Timeline-item>
                    <Button size="large" @click="handleBefore">查看 2.x 版本的日志</Button>
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
                window.open('http://v2.iviewui.com/docs/guide/update');
            }
        }
    }
</script>