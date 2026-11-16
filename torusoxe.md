代发 wailian999

[U57] PHP：字符串插值
来源：http://buh.xylfe.cn

"值: {$a}"
来源：http://xki.tianlin.xyz

[U58] PHP：数组三件套
来源：http://hqt.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zfr.yongpay.top

[U59] PHP：自定义排序
来源：http://syl.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lyg.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://hxf.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://opz.quarkkingdee.top

[U61] PHP：正则
来源：http://oik.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ugg.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://uiw.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wcj.daria6918.cn

[U63] PHP：文件读写
来源：http://urp.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hon.nwbrower.top

[U64] PHP：目录遍历
来源：http://fsx.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://vhk.daria6918.cn

[U65] PHP：会话
来源：http://tjv.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dzt.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://osn.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wfw.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://lhi.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oct.zhengqikj.top

[U68] PHP：PDO 连接
来源：http://iun.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qnh.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://qez.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fwq.yj20258.top

[U70] PHP：PDO 事务
来源：http://pph.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tte.xziqi.cn

[U71] PHP：抛出异常
来源：http://grq.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://uiz.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://jlb.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://wuc.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://rtv.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://qdq.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://vwe.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://otu.andypj.xyz

[U75] PHP：依赖注入
来源：http://ful.svipenyu.cn

composer require psr/container
来源：http://nko.andypj.xyz

[U76] PHP：简单路由
来源：http://rmg.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://brv.zhoulong.xyz

[U77] PHP：模板渲染
来源：http://zur.jiagoushi.top

composer require twig/twig
来源：http://gof.xziqi.cn

[U78] PHP：单元测试
来源：http://rxd.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://qke.pycfn.com

[U79] PHP：静态分析
来源：http://eyk.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://oxj.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://use.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://dzb.cashguo.top

[U81] JS：初始化项目
来源：http://bci.gotoacloud.top

npm init -y;  npm i express
来源：http://mnv.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://kqh.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://scf.yuanzhike.top

[U83] JS：ES Module 导入导出
来源：http://cll.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://csm.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://mdg.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qck.jqgufenzy.top

[U85] JS：可选链
来源：http://yac.havefunace.top

a?.b?.c
来源：http://itw.cucudq.cn

[U86] JS：空值合并
来源：http://wvf.vehdjk.com

a ?? b
来源：http://meo.smart0.xyz

[U87] JS：解构默认值
来源：http://qhx.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://xvg.chenzaomai.com

[U88] JS：对象展开合并
来源：http://pzi.yfazqb.com

{ ...a, ...b }
来源：http://wdj.kuanghao11.cn

[U89] JS：数组去重
来源：http://obh.yanxiufei.cn

[...new Set(arr)]
来源：http://eor.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://lmd.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://swy.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://oge.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xrx.svipenyu.cn

[U92] JS：深拷贝
来源：http://iyp.meibo888.top

structuredClone(obj)
来源：http://mue.xuetiantiany.cn

[U93] JS：模板字符串
来源：http://jar.hnxiangtu.top

`共 ${n} 条`
来源：http://eij.hesvh.cn

[U94] JS：箭头函数
来源：http://pcw.tian-w.cn

const double = x => x * 2;
来源：http://bzs.shzxlz.cn

[U95] JS：Promise 包装
来源：http://qep.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://rjs.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://avo.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lhs.smart0.xyz

[U97] JS：并发请求
来源：http://eqx.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zkj.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://ioi.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rkf.iojbl.cn

[U99] JS：事件监听
来源：http://byp.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://zpp.xinyue.icu

[U100] JS：DOM 查询
来源：http://ffp.xuanzx.com

document.querySelector(".item")
来源：http://ypb.shzxlz.cn

[U101] JS：classList 操作
来源：http://ikt.daria6918.cn

el.classList.toggle("active")
来源：http://ray.gotoacloud.top

[U102] JS：本地存储
来源：http://zeg.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oiz.zhixingplan.top

[U103] JS：定时器
来源：http://qxu.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uhb.shzxlz.cn

[U104] JS：防抖
来源：http://esj.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qan.guowangkeji.top

[U105] JS：节流
来源：http://fhe.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jha.fengsongda.top

[U106] JS：日期格式化
来源：http://xfg.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tqk.ybcxt.top

[U107] JS：数字千分位
来源：http://sox.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ael.yj202588.top

[U108] JS：随机整数
来源：http://sjx.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oyw.cqqwz.cn

[U109] JS：数组分组
来源：http://sce.zhongyouzk.top

Object.groupBy(arr, x => x.type)
来源：http://ybs.yj20258888.top

[U110] JS：数组分块
来源：http://dum.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lss.svipenyu.cn

[U111] JS：对象转 Map
来源：http://icu.tarul.cn

new Map(Object.entries(obj))
来源：http://kuo.ctjpmb.com

[U112] JS：字符串补位
来源：http://qhl.cqqwz.cn

"7".padStart(3, "0")
来源：http://fjz.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://mxj.cashguo.top

s.replaceAll("a", "b")
来源：http://mbx.cashguo.top

[U114] JS：JSON 深比较
来源：http://pju.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://rvy.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://ynr.shuidangran.top

crypto.randomUUID()
来源：http://kui.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://mzd.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://itl.hammf.cn

[U117] JS：单元测试
来源：http://jld.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://jlf.kuanghao11.cn

[U118] JS：开发服务器
来源：http://vej.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://ekm.yuanzhike.top

[U119] JS：生产构建
来源：http://mef.yongpay.top

npx vite build
来源：http://bnm.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://iis.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://wmh.shanyushiyangtech.top

================================================================================
来源：http://han.jyoumei.cn

统计汇总
来源：http://mgr.yvedp.cn

================================================================================
来源：http://efr.xylfe.cn

按语言统计（条）：
来源：http://dvv.ehwqpu.com

Python ......... 252
来源：http://chg.zhaomingkeji.xyz

PHP ............ 252
来源：http://dfl.gaohongyu789.top

JavaScript ..... 252
来源：http://ymv.feifeiyinyue.top

TypeScript ..... 212
来源：http://jfu.shanyushiyangkeji.top

Java ........... 212
来源：http://zue.chenlongwang.top

Go ............. 212
来源：http://jwu.haohaochexian.top

Ruby ........... 212
来源：http://exe.jinqigfzy.top

C# ............. 212
来源：http://ehm.dianchejie.cn

C .............. 30
来源：http://yby.sxryk.cn

C++ ............ 30
来源：http://own.jlsjyb.cn

SQL ............ 90
来源：http://yoc.jinghuilouyu.cn

Bash ........... 80
来源：http://kcd.fengsongda.top

Kotlin ......... 15
来源：http://wga.shzxlz.cn

Swift .......... 15
来源：http://kzi.jinghuilouyu.cn

Lua ............ 10
来源：http://zta.shanyushiyangtech.top

Perl ........... 10
来源：http://ual.gogol.net.cn

Scala .......... 10
来源：http://zqj.daria6918.cn

------------------------------------
来源：http://mlw.mhx1999.top

合计 ........... 2106 条
来源：http://xre.pengpengdd.cyou

按章节统计：
来源：http://jzz.gzhubu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://atv.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rpd.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mqf.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ffq.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dwi.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tzz.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cjq.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lxl.kuanghao11.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nmr.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rte.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://brd.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gwr.ybcxt.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cod.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zvk.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tcs.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xyz.tarul.cn

Q SQL 专题                              90
来源：http://aly.jyoumei.cn

R Bash 专题                             80
来源：http://kex.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://vua.hfpthk.cn

T 其他语言补充                          60
来源：http://xtt.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://brv.pycfn.com

------------------------------------
来源：http://mnj.gaohongyu789.top

合计                                  2106 条
来源：http://vwp.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://epm.jyoumei.cn

使用提醒
来源：http://syv.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://ifn.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cnv.jqgfzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yqb.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://viy.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fuk.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://glo.ppjwa.cn

—— 文件结束 ——
来源：http://pye.ehwqpu.com

================================================================================
来源：http://lgp.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://wcm.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://dxj.uphjek.com

================================================================================
来源：http://kss.hesvh.cn

【收录内容】
来源：http://kog.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nbt.zhoulong.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fyk.hfpthk.cn

SQL · Bash · C · C++
来源：http://umj.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mcz.aizwys.cn

【使用说明】
来源：http://sih.guowangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gne.guannengcc.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://flj.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zqf.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://huj.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://afv.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://grj.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vvw.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gso.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mwu.pengpengdd.cyou

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rgl.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lfm.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nwi.ctjpmb.com

【文件统计】
来源：http://lsd.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wiy.xylfe.cn

--------------------------------------------------------------------------------
来源：http://uez.sufxvd.cn

目  录
来源：http://tnz.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://tth.daria6918.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xbd.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wxx.gzhubu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://idm.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vln.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gsx.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vzt.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://chz.ctjpmb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bag.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hym.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iod.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xof.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tvq.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ibe.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dyk.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qml.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xfd.52xcode.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://svm.ybcxt.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jfi.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jio.vqdsnc.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://spd.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pqv.mhx1999.top

================================================================================
来源：http://web.daxiang520.top

A. 基础语法与类型
来源：http://xtb.shanyushiyangkeji.top

================================================================================
来源：http://jth.wangdashe.top

[A01] Hello World
来源：http://gfh.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://zlw.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://hlt.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://djy.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wkl.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://uwn.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://qza.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://vhl.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gpu.jiagoushi.top

[A02] 变量声明与赋值
来源：http://zoi.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ptz.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uug.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://stt.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fop.ywan-chungtsiang.top

Java: String name = "Alex"; int age = 20;
来源：http://wfu.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://hoy.gotoacloud.top

Ruby: name = "Alex"; age = 20
来源：http://yyi.shzxlz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vcb.daria6918.cn

[A03] 常量定义
来源：http://rxt.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cxj.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://lcs.52xcode.cn

JS:   const PI = 3.14159;
来源：http://qay.chenjidiqi.icu

TS:   const PI: number = 3.14159;
来源：http://eza.guannengcc.top

Java: static final double PI = 3.14159;
来源：http://otx.redwolf501.top

Go:   const PI = 3.14159
来源：http://slx.gotoacloud.top

Ruby: PI = 3.14159
来源：http://qgc.quarkkingdee.top

C#:   const double PI = 3.14159;
来源：http://azj.daria6918.cn

[A04] 判断变量类型
来源：http://xea.ydzc1.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zev.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://crf.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://grr.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://jco.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lxr.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://nxa.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://hmr.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://efh.jinyuanbaomall.cn

[A05] 整数除法与取模
来源：http://ihw.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jwb.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://khl.fengsongda.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cln.xziqi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yhz.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://wja.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://jky.zhaomingkeji.xyz

Ruby: 7 / 2; 7 % 2
来源：http://wso.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://fhy.fehbvm.com

[A06] 字符串转数字
来源：http://luc.yuanzhike.top

Py:   int("42"); float("3.14")
来源：http://fba.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kqs.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jfk.fengsongda.top

TS:   parseInt("42", 10); Number("42")
来源：http://nqj.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bek.zhoulong.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bln.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bqe.52xcode.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://koy.shanyushiyangtech.top

[A07] 数字转字符串
来源：http://kxy.aibaodan.cn

Py:   str(42)
来源：http://iwh.sweek.top

PHP:  (string) 42; strval(42)
来源：http://teb.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://gaf.sjlbkw.cn

TS:   String(42)
来源：http://kvo.wangshuangyany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pgh.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://ctu.9152youxi.cn

Ruby: 42.to_s
来源：http://dff.yj20258888.top

C#:   42.ToString()
来源：http://xop.xingfuxueyuan.xyz

[A08] 取整与四舍五入
来源：http://qjj.yanxiufei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ypt.sxryk.cn


<!-- 参考信息 -->