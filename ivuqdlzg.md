代发 wailian999

[U63] PHP：文件读写
来源：http://ayj.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gmo.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://dvz.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://pcf.yanxiufei.cn

[U65] PHP：会话
来源：http://vru.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tqt.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://aep.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mre.jianghu66.top

[U67] PHP：处理文件上传
来源：http://wqg.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jeh.smart0.xyz

[U68] PHP：PDO 连接
来源：http://stz.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fft.shanyushiyangkeji.top

[U69] PHP：PDO 预处理
来源：http://gel.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hbk.bjfxy.top

[U70] PHP：PDO 事务
来源：http://wxd.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gea.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://wjv.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://dtg.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://brz.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://dmk.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://nld.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://aih.snrcjt.cn

[U74] PHP：读取环境变量
来源：http://vrk.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://tdw.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://wqk.zhaomingkeji.xyz

composer require psr/container
来源：http://nsi.jiagoushi.top

[U76] PHP：简单路由
来源：http://dmm.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zaz.cashguo.top

[U77] PHP：模板渲染
来源：http://syh.yuanzhike.top

composer require twig/twig
来源：http://vba.dianchejie.cn

[U78] PHP：单元测试
来源：http://qhj.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://hhq.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://gdq.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://bsp.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://lni.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://tcj.epnwcf.com

[U81] JS：初始化项目
来源：http://gba.0kj1m.cn

npm init -y;  npm i express
来源：http://oax.shangyingyoupin.top

[U82] JS：package.json 脚本
来源：http://juv.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hlr.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://ztj.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://epb.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://nom.bjfxy.top

module.exports = { a };  const { a } = require("./m");
来源：http://gfr.cheryme.top

[U85] JS：可选链
来源：http://qfw.yj202588.top

a?.b?.c
来源：http://tvw.pengpengdd.cyou

[U86] JS：空值合并
来源：http://vxe.hywenlv.cn

a ?? b
来源：http://cqz.tianlin.xyz

[U87] JS：解构默认值
来源：http://jll.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://yyo.daria6918.cn

[U88] JS：对象展开合并
来源：http://blt.ydzc1.top

{ ...a, ...b }
来源：http://jxw.ybcxt.top

[U89] JS：数组去重
来源：http://neu.ybcxt.top

[...new Set(arr)]
来源：http://mzc.yfazqb.com

[U90] JS：数字数组排序
来源：http://wqn.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://eyj.hammf.cn

[U91] JS：对象键值遍历
来源：http://wca.hongshengwenyu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rnr.vqdsnc.cn

[U92] JS：深拷贝
来源：http://ypz.yueranfly.top

structuredClone(obj)
来源：http://jrg.guowangkeji.top

[U93] JS：模板字符串
来源：http://iep.xziqi.cn

`共 ${n} 条`
来源：http://laz.yj202588.top

[U94] JS：箭头函数
来源：http://lmu.cqqwz.cn

const double = x => x * 2;
来源：http://npr.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://gvc.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://cvy.epnwcf.com

[U96] JS：async/await 与异常
来源：http://rsk.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://piq.dashuyun.cn

[U97] JS：并发请求
来源：http://jlt.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://moy.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://kvu.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xkn.daxiang520.top

[U99] JS：事件监听
来源：http://ulz.daria6918.cn

el.addEventListener("click", e => {})
来源：http://cpg.gzhubu.top

[U100] JS：DOM 查询
来源：http://nbb.yongpay.top

document.querySelector(".item")
来源：http://sig.jinqigufen.top

[U101] JS：classList 操作
来源：http://qmh.dashuyun.cn

el.classList.toggle("active")
来源：http://doa.cqqwz.cn

[U102] JS：本地存储
来源：http://hro.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hrw.daxiang520.top

[U103] JS：定时器
来源：http://mxh.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gio.yuxming.cn

[U104] JS：防抖
来源：http://eaj.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzh.cashguo.top

[U105] JS：节流
来源：http://mze.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mlz.snrcjt.cn

[U106] JS：日期格式化
来源：http://yul.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wgv.xylfe.cn

[U107] JS：数字千分位
来源：http://jvu.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yim.guannengcc.top

[U108] JS：随机整数
来源：http://sse.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jpf.gzhubu.top

[U109] JS：数组分组
来源：http://pks.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://rbi.aibaodan.cn

[U110] JS：数组分块
来源：http://mdh.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjn.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://syf.dashuyun.cn

new Map(Object.entries(obj))
来源：http://cyv.sweek.top

[U112] JS：字符串补位
来源：http://hfj.hfpthk.cn

"7".padStart(3, "0")
来源：http://rrs.cheryme.top

[U113] JS：正则替换全部
来源：http://vrf.uphjek.com

s.replaceAll("a", "b")
来源：http://bcg.shuidangran.top

[U114] JS：JSON 深比较
来源：http://asi.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mne.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://jck.yuanzhike.top

crypto.randomUUID()
来源：http://cvg.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://zvr.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://ert.uphjek.com

[U117] JS：单元测试
来源：http://ofo.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://afh.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://wrf.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://gfh.zdqjudy.top

[U119] JS：生产构建
来源：http://tbm.redwolf501.top

npx vite build
来源：http://mif.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://hqs.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://yjf.jianghu66.top

================================================================================
来源：http://cmp.snrcjt.cn

统计汇总
来源：http://cvx.aibaodan.cn

================================================================================
来源：http://tfd.daria6918.cn

按语言统计（条）：
来源：http://cnx.epnwcf.com

Python ......... 252
来源：http://ojb.gaohongyu789.top

PHP ............ 252
来源：http://yny.uphjek.com

JavaScript ..... 252
来源：http://qwz.zhoulong.xyz

TypeScript ..... 212
来源：http://srl.dianchejie.cn

Java ........... 212
来源：http://oow.xuanzx.com

Go ............. 212
来源：http://sfs.zhongyouzk.top

Ruby ........... 212
来源：http://hfu.ydzc1.top

C# ............. 212
来源：http://pju.bjfxy.top

C .............. 30
来源：http://vij.dianchejie.cn

C++ ............ 30
来源：http://ojl.shanyushiyangkeji.top

SQL ............ 90
来源：http://olr.vqdsnc.cn

Bash ........... 80
来源：http://cds.nanxinkj.top

Kotlin ......... 15
来源：http://fcb.c1oappe.top

Swift .......... 15
来源：http://nog.bbcook.cn

Lua ............ 10
来源：http://fum.cheryme.top

Perl ........... 10
来源：http://yhx.ybcxt.top

Scala .......... 10
来源：http://ckx.guannengcc.top

------------------------------------
来源：http://aph.ehwqpu.com

合计 ........... 2106 条
来源：http://gkr.jlsjyb.cn

按章节统计：
来源：http://mtn.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fja.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kvk.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ibz.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jnw.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vxa.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zxs.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ntt.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hxs.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fxr.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://get.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yzw.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lqe.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dmf.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bft.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ifw.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ypy.yvedp.cn

Q SQL 专题                              90
来源：http://xcw.daxiang520.top

R Bash 专题                             80
来源：http://wkf.shzxlz.cn

S C / C++ 专题                          60
来源：http://far.feifeiyinyue.top

T 其他语言补充                          60
来源：http://hwa.yuxming.cn

U 高频实用片段                         120
来源：http://wek.havefunace.top

------------------------------------
来源：http://rxl.hysaishi.cn

合计                                  2106 条
来源：http://gyz.yj202588.top

--------------------------------------------------------------------------------
来源：http://qqb.shanyushiyangkeji.top

使用提醒
来源：http://igw.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://xbb.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cqk.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gjr.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dnm.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pbt.daria6918.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uvn.gogol.net.cn

—— 文件结束 ——
来源：http://qcx.zycfv.cn

================================================================================
来源：http://jxu.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://jsj.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://ggs.gotoacloud.top

================================================================================
来源：http://hga.xuetiantiany.cn

【收录内容】
来源：http://xuu.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://olq.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iqq.yj20258888.top

SQL · Bash · C · C++
来源：http://bvn.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yvh.ivvv.top

【使用说明】
来源：http://kas.dashuyun.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lbu.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://avd.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bjo.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cyq.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ufk.epnwcf.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nvq.yonumen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cpt.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zpd.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ewr.zhongyouzk.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mjk.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ndy.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mnb.cucudq.cn

【文件统计】
来源：http://ryq.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pdj.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://iiy.fengsongda.top

目  录
来源：http://fbc.yj20258888.top

--------------------------------------------------------------------------------
来源：http://bnv.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pfl.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qdm.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nrk.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wxl.xuanzx.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wpr.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fsm.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oya.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vyg.fanxiaobao.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wfy.tanke756.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gug.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ajf.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qyz.yongpay.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qvg.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ooa.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nll.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://upi.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://eep.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://eiu.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bef.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hfv.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ipb.vehdjk.com

================================================================================
来源：http://awf.dianchejie.cn

A. 基础语法与类型
来源：http://tkz.yfazqb.com

================================================================================
来源：http://mjn.xuanzx.com

[A01] Hello World
来源：http://xhi.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://xsi.zhongyouzk.top

PHP:  echo "Hello, World!";
来源：http://paj.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://ycf.ybcxt.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rzr.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://qiz.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://gft.sjlbkw.cn

Ruby: puts "Hello, World!"
来源：http://ptn.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xjy.andypj.xyz

[A02] 变量声明与赋值
来源：http://qvb.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zhh.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://fvm.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://xnd.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wbo.cashguo.top

Java: String name = "Alex"; int age = 20;
来源：http://ytk.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://btj.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://vta.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://uux.jqgufenzy.top

[A03] 常量定义
来源：http://ejf.xinyue.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gut.yonumen.top

PHP:  const PI = 3.14159;
来源：http://miu.yongpay.top

JS:   const PI = 3.14159;
来源：http://uks.vqdsnc.cn

TS:   const PI: number = 3.14159;
来源：http://tly.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://uya.guannengcc.top

Go:   const PI = 3.14159
来源：http://nuh.cashguo.top

Ruby: PI = 3.14159
来源：http://vbb.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://geh.jinghuilouyu.cn

[A04] 判断变量类型
来源：http://ouo.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bxm.fengsongda.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jpv.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gup.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://zts.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iih.xylfe.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vux.quarkkingdee.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ute.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://elx.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://hhh.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qmj.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gic.ydjk.org.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hyr.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://klm.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://bsx.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://anz.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://lhq.uphjek.com

C#:   7 / 2; 7 % 2
来源：http://vaq.yueranfly.top

[A06] 字符串转数字
来源：http://toe.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://rrh.yj20258.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ebx.c1oappe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://umd.wangdashe.top

TS:   parseInt("42", 10); Number("42")
来源：http://wnh.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gqp.hammf.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kfa.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iug.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://slq.nwbrower.top

[A07] 数字转字符串
来源：http://tsj.0kj1m.cn

Py:   str(42)
来源：http://zua.wangdashe.top

PHP:  (string) 42; strval(42)
来源：http://gue.yonumen.top

JS:   String(42); (42).toString()
来源：http://vrp.chenlongwang.top

TS:   String(42)
来源：http://uea.jinqigufen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xtx.meibo888.top

Go:   strconv.Itoa(42)
来源：http://mla.tarul.cn

Ruby: 42.to_s
来源：http://qzr.9152youxi.cn

C#:   42.ToString()
来源：http://phc.tarul.cn

[A08] 取整与四舍五入
来源：http://rtl.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hhc.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zai.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bot.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://glb.jinqigufen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mfk.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ekj.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jrw.xziqi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://swf.316326.xyz

[A09] 绝对值与最大最小值
来源：http://pgk.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fyz.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jpx.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hee.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://prc.yj202588.top


<!-- 参考信息 -->