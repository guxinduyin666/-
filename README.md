# -
孤心独饮的存储库
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>个人简历</title>
    <link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css">
    <style>
        body {
            padding-top: 70px;
        }

        address {
            font-size: 17px;
        }

        #divCarousel {
            background: #000;
        }
        .carousel-indicators{
            bottom:0;
            background: #eee;
        }
    </style>
</head>
<body class="container">
<header>
    <!--头部导航栏-->
    <nav class="navbar navbar-inverse navbar-fixed-top">
        <!--导航栏容器-->
        <div class="container">
            <div class="navbar-header">
                <div class="navbar-brand">
                    个人简历
                </div>
                <!--当浏览器宽度小于一定宽度时显示的按钮，点击按钮显示/隐藏一个可折叠区域-->
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#divNav">
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
            </div>
            <!--点击按钮显示/折叠的区域-->
            <div id="divNav" class="collapse navbar-collapse">
                <ul class="nav navbar-nav navbar-right">
                    <li>
                        <!--点击按钮可出现一个模态框-->
                        <button type="button" class="btn btn-success navbar-btn" data-toggle="modal"
                                data-target="#divModal" title="打印">打印
                        </button>
                        <!--模态框-->
                        <div class="modal fade" id="divModal">
                            <div class="modal-dialog">
                                <div class="modal-content">
                                    <div class="modal-header">
                                        <button type="button" class="close"
                                                data-dismiss="modal"><span>&times;</span></button>
                                        <h4>打印简历</h4>
                                    </div>
                                    <div class="modal-body">打印预览或者打印配置</div>
                                    <div class="modal-footer">
                                        <button type="button" class="btn btn-default" data-dismiss="modal">关闭</button>
                                        <button type="button" class="btn btn-primary">打印</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <!--带提示工具的按钮-->
                        <button type="button" class="btn btn-info navbar-btn" data-toggle="tooltip"
                                data-placement="bottom" title="下载">下载
                        </button>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</header>
<!--内容区域-->
<div>
    <div class="row">
        <!--左侧-->
        <div class="col-sm-4">
            <!--个人信息-->
            <div class="panel panel-default">
                <div class="panel-heading">个人信息</div>
                <div class="panel-body">
                    <img class="img-responsive img-rounded img-thumbnail" src="images/me.jpg" alt="me">
                    <p class="text-center text-primary">王朝传</p>
                    <!--address标签显示联系方式-->
                    <address>
                        <span class="glyphicon glyphicon-home" title="地址"> 江西省吉安市</span><br>
                        <span class="glyphicon glyphicon-phone" title="电话"> 15770675728</span><br>
                        <span class="glyphicon glyphicon-envelope" title="邮箱"> 1980901451@qq.com</span>
                    </address>
                </div>
            </div>
            <!--技能-->
            <div class="panel panel-info">
                <div class="panel-heading">掌握技能</div>
                <div class="panel-body">
                    <div class="row">
                        <div class="col-sm-4">
                            <span class="text-muted">HTML</span>
                        </div>
                        <div class="col-sm-8">
                            <div class="progress">
                                <div class="progress-bar progress-bar-success progress-bar-striped active"
                                     style="width:85%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-sm-4">
                            <span class="text-muted"> CSS3</span>
                        </div>
                        <div class="col-sm-8">
                            <div class="progress">
                                <div class="progress-bar progress-bar-success progress-bar-striped active"
                                     style="width:80%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-sm-4">
                            <span class="text-muted">JS</span>
                        </div>
                        <div class="col-sm-8">
                            <div class="progress">
                                <div class="progress-bar progress-bar-info progress-bar-striped active"
                                     style="width:70%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-sm-4">
                            <span class="text-muted">JQuery</span>
                        </div>
                        <div class="col-sm-8">
                            <div class="progress">
                                <div class="progress-bar progress-bar-info progress-bar-striped active"
                                     style="width:70%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-sm-4" style="font-size: 12px">
                            <span class="text-muted">Bootstrap</span>
                        </div>
                        <div class="col-sm-8">
                            <div class="progress">
                                <div class="progress-bar progress-bar-warning progress-bar-striped active"
                                     style="width:60%"></div>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col-sm-4">
                            <span class="text-muted">JAVA</span>
                        </div>
                        <div class="col-sm-8">
                            <div class="progress">
                                <div class="progress-bar progress-bar-warning progress-bar-striped active"
                                     style="width:50%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!--联系我-->
            <div class="panel panel-primary">
                <div class="panel-heading">联系我</div>
                <div class="panel-body">
                    <form class="form-horizontal">
                        <div class="form-group">
                            <label for="email" class="col-sm-4 control-label">邮箱</label>
                            <div class="col-sm-8">
                                <input type="email" id="email" class="form-control" placeholder="请输入邮箱">
                            </div>
                        </div>
                        <div class="form-group">
                            <label for="name" class="col-sm-4 control-label">姓名</label>
                            <div class="col-sm-8">
                                <input type="text" id="name" class="form-control" placeholder="请输入姓名">
                            </div>
                        </div>
                        <div class="form-group">
                            <div class="col-sm-offset-4 col-sm-8">
                                <button type="submit" class="btn btn-primary pull-right">发送</button>
                                <div class="clearfix"></div>
                            </div>
                        </div>
                    </form>
                </div>
            </div>
        </div>
        <!--右侧-->
        <div class="col-sm-8">
            <!--个人简介-->
            <div class="jumbotron">
                <h2>自我评价</h2>
                <ol class="list-group">
                    <li class="list-group-item">具有良好的沟通能力、业务逻辑分析能力、解决问题能力强</li>
                    <li class="list-group-item">具有较丰富的前端设计和开发经验</li>
                    <li class="list-group-item">学习能力强，有了面向对象的编程思想后，能融会贯通其它的编程语言</li>
                    <li class="list-group-item">具有优良的职业操守、有优秀的团队合作精神</li>
                    <li class="list-group-item">对工作具有高度的责任心，热爱前端工作</li>
                </ol>
            </div>
            <!--折叠面板-->
            <div class="panel-group" id="accordion">
                <!--工作经验-->
                <div class="panel panel-default">
                    <div class="panel-heading">
                        <div class="panel-title">
                            <a href="#collapseOne" data-toggle="collapse" data-parent="#accordion">工作经验</a>
                        </div>
                        <div id="collapseOne" class="panel-collapse collapse">
                            <div class="panel-body">
                                <ul class="list-group">
                                    <li class="list-group-item list-group-item-success">
                                        <div class="row">
                                            <div class="col-sm-4">2015/2--2016/01</div>
                                            <div class="col-sm-4">江西联微软件技术有限公司</div>
                                            <div class="col-sm-4">Web前端工程师</div>
                                        </div>
                                    </li>
                                    <li class="list-group-item list-group-item-warning">
                                        <div class="row">
                                            <div class="col-sm-4">2014/3--2014/09</div>
                                            <div class="col-sm-4">东莞市永信药业有限公司</div>
                                            <div class="col-sm-4">验收组长</div>
                                        </div>
                                    </li>
                                    <li class="list-group-item list-group-item-info">
                                        <div class="row">
                                            <div class="col-sm-4">2013/7--2014/02</div>
                                            <div class="col-sm-4">东莞市永信药业有限公司</div>
                                            <div class="col-sm-4">验收员</div>
                                        </div>
                                    </li>
                                </ul>

                            </div>
                        </div>
                    </div>
                </div>
                <!--教育经历-->
                <div class="panel panel-default">
                    <div class="panel-heading">
                        <div class="panel-title">
                            <a href="#collapseTwo" data-toggle="collapse" data-parent="#accordion">教育经历</a>
                        </div>
                        <div id="collapseTwo" class="panel-collapse collapse">
                            <div class="panel-body">
                                <ul class="list-group">
                                    <li class="list-group-item list-group-item-success">
                                        <div class="row">
                                            <div class="col-sm-4">2009/9--2013/07</div>
                                            <div class="col-sm-4">皖南医学院</div>
                                            <div class="col-sm-4">大学本科</div>
                                        </div>
                                    </li>
                                    <li class="list-group-item list-group-item-warning">
                                        <div class="row">
                                            <div class="col-sm-4">2006/9--2009/06</div>
                                            <div class="col-sm-4">江西省永丰二中</div>
                                            <div class="col-sm-4">高中</div>
                                        </div>
                                    </li>
                                    <li class="list-group-item list-group-item-info">
                                        <div class="row">
                                            <div class="col-sm-4">2003/9--2006/06</div>
                                            <div class="col-sm-4">江西省永丰县藤田中学</div>
                                            <div class="col-sm-4">初中</div>
                                        </div>
                                    </li>
                                </ul>

                            </div>
                        </div>
                    </div>
                </div>
                <!--项目展示-->
                <div class="panel panel-default">
                    <div class="panel-heading">
                        <div class="panel-title">
                            <a href="#collapseThree" data-toggle="collapse" data-parent="#accordion">项目展示</a>
                        </div>
                        <div id="collapseThree" class="panel-collapse collapse in">
                            <div class="panel-body">
                                <div id="divCarousel" class="carousel slide" data-ride="carousel">
                                    <ol class="carousel-indicators">
                                        <li data-target="#divCarousel" data-slide-to="0" class="active"></li>
                                        <li data-target="#divCarousel" data-slide-to="1"></li>
                                        <li data-target="#divCarousel" data-slide-to="2"></li>
                                    </ol>
                                    <div class="carousel-inner">
                                        <div class="item active">
                                            <div class="panel panel-success">
                                                <div class="panel-body">
                                                    <h4>赣货网</h4>
                                                    <p>
                                                        开发环境：Chrome+webStorm <br>
                                                        开发技术：HTML + CSS/CSS3 +Bootstrap+ jQuery+JavaScript + Ajax <br>
                                                        赣货网是一个江西本土电商平台。服务于整个江西地区，大力扶持江西特色产品、农副产品等实体企业融入电商行业，推动江西特色产品、农副产品的输出.<br>
                                                        项目技术：<br>
                                                        1、登录注册页面主要使用到的是正则表达式判断数据格式及Ajax的异步请求数据。<br>
                                                        2、运用HTML/CSS进行简单布局，运用CSS3和jQuery进行渲染。<br>
                                                        3、使用CSS3多列属性实现瀑布流布局。<br>
                                                        4、运用Ajax+json把需要加载的dom元素进行组织，动态加载网页元素。<br>
                                                        5、运用Bootstrap在移动设备上自适应，使用HTML5和CSS3等的新属性方法做布局及页面特效。<br>
                                                        6、运用谷歌浏览器调试工具进行调试、抓包。
                                                    </p>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="item">
                                            <div class="panel panel-info">
                                                <div class="panel-body">
                                                    <h4>一元店商城</h4>
                                                    <p>
                                                        开发环境：Chrome+webStorm <br>
                                                        开发技术：HTML + CSS/CSS3 +Bootstrap+ jQuery+JavaScript + Ajax <br>
                                                        1元店商城是一个pc端和移动端的购物商城网站,只需1元就有机会获得一件奖品。主要负责实现注册页面、登录页面、官网页面、页面切换以及详情页的渲染等业务的要求。
                                                        <br>
                                                        项目技术：<br><br>
                                                        1、登录注册页面主要使用到的是正则表达式判断数据格式及Ajax的异步请求数据。<br>
                                                        2、运用HTML/CSS进行简单布局，运用CSS3和jQuery进行渲染。<br>
                                                        3、运用Ajax+json+jsp把需要加载的dom元素进行组织，动态加载网页元素。<br>
                                                        4、运用Bootstrap在移动设备上自适应，使用HTML5和CSS3等的新属性方法做布局及页面特效。<br>
                                                        5、运用谷歌浏览器调试工具进行调试、抓包。
                                                    </p>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="item">
                                            <div class="panel panel-primary">
                                                <div class="panel-body">
                                                    <h4>订餐小秘书网上点餐系统</h4>
                                                    <p>
                                                        开发环境： Webstorm <br>
                                                        开发技术: HTML+ CSS/CSS3+Bootstrap+JQuery+Javascript <br>
                                                        网上点餐管理系统, 主要功能: 商品列表 商品详情，商品管理，订单管理
                                                        用户管理，用户购物车管理等几个主页面。管理员可以在后台添加，删除，编辑产品信息，用户信息和订单信息，用户只有登陆，注册，查看商品详情，购买商品等权限。<br><br>
                                                        项目技术：<br>
                                                        1、使用HTML5的语义化标签进行布局，便于SEO。<br>
                                                        2、使用CSS3的新属性transition实现过度效果，transform实现2D/3D转换效果，animation实现动画效果。<br>
                                                        3、使用JavaScript和jQuery实现页面交互事件逻辑代码。<br>
                                                        4、运用Ajax+json+jsp把需要加载的dom元素进行组织，动态加载网页元素。<br>
                                                        5、运用Bootstrap在移动设备上自适应，使用HTML5和CSS3等的新属性方法做布局及页面特效。<br>
                                                    </p>
                                                </div>
                                            </div>
                                        </div>

                                    </div>
                                    <a class="left carousel-control" href="#divCarousel" data-slide="prev">
                                        <span class="glyphicon glyphicon-chevron-left"></span>
                                    </a>
                                    <a class="right carousel-control" href="#divCarousel" data-slide="next">
                                        <span class="glyphicon glyphicon-chevron-right"></span>
                                    </a>

                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
<footer>
    <!--底部导航栏-->
    <nav class="navbar-default navbar-fixed-bottom text-center">
        版权所有&nbsp;All images and content &copy;王朝传
    </nav>
</footer>
</body>
<script src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
<script src="https://cdn.bootcss.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<script>
    $(function () {
        $('[data-toggle="tooltip"]').tooltip();
    })
</script>
</html>
