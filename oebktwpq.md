代发 wailian999

[U57] PHP：字符串插值
来源：http://dly.fanxiaobao.xyz

"值: {$a}"
来源：http://wur.xuanzx.com

[U58] PHP：数组三件套
来源：http://tog.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dkf.sufxvd.cn

[U59] PHP：自定义排序
来源：http://rsc.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kql.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://tbk.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yzr.andypj.xyz

[U61] PHP：正则
来源：http://nub.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vqj.hammf.cn

[U62] PHP：日期对象
来源：http://nph.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mjf.dianchejie.cn

[U63] PHP：文件读写
来源：http://bdy.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jzf.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://sua.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://gfv.52xcode.cn

[U65] PHP：会话
来源：http://hum.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jun.sweek.top

[U66] PHP：设置 Cookie
来源：http://vzz.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ujj.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://ync.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rkg.52xcode.cn

[U68] PHP：PDO 连接
来源：http://gxr.vehdjk.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vor.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://ira.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iyg.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://abb.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nvn.tarul.cn

[U71] PHP：抛出异常
来源：http://erg.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://rla.tianlin.xyz

[U72] PHP：写错误日志
来源：http://zly.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://krh.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://dpa.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://umn.jinghuilouyu.cn

[U74] PHP：读取环境变量
来源：http://fds.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://cfz.xuanzx.com

[U75] PHP：依赖注入
来源：http://zwo.zhiwuduotai.top

composer require psr/container
来源：http://mpf.dianchejie.cn

[U76] PHP：简单路由
来源：http://tgz.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qrt.havefunace.top

[U77] PHP：模板渲染
来源：http://qrp.jinyuanbaomall.cn

composer require twig/twig
来源：http://qqb.zdqjudy.top

[U78] PHP：单元测试
来源：http://mro.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://awp.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://mfd.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://zzv.ivvv.top

[U80] PHP：代码规范修复
来源：http://voi.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://shi.hnxiangtu.top

[U81] JS：初始化项目
来源：http://eno.pycfn.com

npm init -y;  npm i express
来源：http://cxh.xinyue.icu

[U82] JS：package.json 脚本
来源：http://kmh.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://crj.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://rwg.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://uqu.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://lmk.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qgc.redwolf501.top

[U85] JS：可选链
来源：http://sdt.hnxiangtu.top

a?.b?.c
来源：http://nlh.yonumen.top

[U86] JS：空值合并
来源：http://vjb.jinghuilouyu.cn

a ?? b
来源：http://arw.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://ggu.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://phq.yvedp.cn

[U88] JS：对象展开合并
来源：http://jqp.fengsongda.top

{ ...a, ...b }
来源：http://gas.gotoacloud.top

[U89] JS：数组去重
来源：http://hsw.ydzc1.top

[...new Set(arr)]
来源：http://pxt.gogol.net.cn

[U90] JS：数字数组排序
来源：http://fbh.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://gxc.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://tte.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://whe.hesvh.cn

[U92] JS：深拷贝
来源：http://vdf.shanyushiyangtech.top

structuredClone(obj)
来源：http://fgn.iojbl.cn

[U93] JS：模板字符串
来源：http://azl.zdqjudy.top

`共 ${n} 条`
来源：http://mrz.cqqwz.cn

[U94] JS：箭头函数
来源：http://ngu.yuxming.cn

const double = x => x * 2;
来源：http://ooe.aibaodan.cn

[U95] JS：Promise 包装
来源：http://nnm.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://sqx.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://abj.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aex.hongshengwenyu.top

[U97] JS：并发请求
来源：http://ykc.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vzx.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://eve.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ezs.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://vee.tanke756.top

el.addEventListener("click", e => {})
来源：http://jkx.epnwcf.com

[U100] JS：DOM 查询
来源：http://ftg.tianlin.xyz

document.querySelector(".item")
来源：http://fxd.xinyue.icu

[U101] JS：classList 操作
来源：http://fwz.jqgfzy.top

el.classList.toggle("active")
来源：http://xvo.hcnkem.com

[U102] JS：本地存储
来源：http://mrg.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://lqq.dashuyun.cn

[U103] JS：定时器
来源：http://vfa.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ghx.ydzc1.top

[U104] JS：防抖
来源：http://jvu.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hgf.zhengqikj.top

[U105] JS：节流
来源：http://woc.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ttq.xuanzx.com

[U106] JS：日期格式化
来源：http://roy.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://auk.fktsv.cn

[U107] JS：数字千分位
来源：http://shy.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vsj.zycfv.cn

[U108] JS：随机整数
来源：http://pmi.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bmp.ybcxt.top

[U109] JS：数组分组
来源：http://wtm.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://lts.nanxuanxn.top

[U110] JS：数组分块
来源：http://tlq.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qss.xuanzx.com

[U111] JS：对象转 Map
来源：http://mqm.cheryme.top

new Map(Object.entries(obj))
来源：http://jxc.cdnleiting.top

[U112] JS：字符串补位
来源：http://nfg.shuidangran.top

"7".padStart(3, "0")
来源：http://ifl.jiagoushi.top

[U113] JS：正则替换全部
来源：http://hmw.sweek.top

s.replaceAll("a", "b")
来源：http://mzk.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://ezl.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wzw.yj20258.top

[U115] JS：生成 UUID
来源：http://vpy.zycfv.cn

crypto.randomUUID()
来源：http://qzi.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://piy.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://tch.yongpay.top

[U117] JS：单元测试
来源：http://qnv.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://bci.ctjpmb.com

[U118] JS：开发服务器
来源：http://mwr.bjfxy.top

npm i -D vite;  npx vite
来源：http://zpw.316326.xyz

[U119] JS：生产构建
来源：http://nxy.iojbl.cn

npx vite build
来源：http://bbx.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://vkj.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://xqd.sweek.top

================================================================================
来源：http://jop.jinyuanbaomall.cn

统计汇总
来源：http://pvc.hysaishi.cn

================================================================================
来源：http://ovz.shanyushiyangkeji.top

按语言统计（条）：
来源：http://ken.zhaomingkeji.xyz

Python ......... 252
来源：http://ged.guannengcc.top

PHP ............ 252
来源：http://fgj.nanxuanxn.top

JavaScript ..... 252
来源：http://fqt.mhx1999.top

TypeScript ..... 212
来源：http://sqq.52xcode.cn

Java ........... 212
来源：http://jnp.yuxming.cn

Go ............. 212
来源：http://zlf.sxryk.cn

Ruby ........... 212
来源：http://dao.cucudq.cn

C# ............. 212
来源：http://ykr.guannengcc.top

C .............. 30
来源：http://mfl.guowangkeji.top

C++ ............ 30
来源：http://jez.yj20258888.top

SQL ............ 90
来源：http://iko.haohaochexian.top

Bash ........... 80
来源：http://kfz.hnqzz.top

Kotlin ......... 15
来源：http://wwi.hfpthk.cn

Swift .......... 15
来源：http://tfh.aibaodan.cn

Lua ............ 10
来源：http://ckb.zhengqikj.top

Perl ........... 10
来源：http://zqx.hammf.cn

Scala .......... 10
来源：http://hfr.316326.xyz

------------------------------------
来源：http://ako.ppjwa.cn

合计 ........... 2106 条
来源：http://gkp.daria6918.cn

按章节统计：
来源：http://omq.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dju.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yoy.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lxu.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fsl.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fwr.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vxm.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rgs.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ehe.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rrt.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vtf.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rny.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gsj.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rfj.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rji.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fvb.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://spl.wangshuangyany.cn

Q SQL 专题                              90
来源：http://avt.yuanzhike.top

R Bash 专题                             80
来源：http://hwz.mhx1999.top

S C / C++ 专题                          60
来源：http://obj.aizwys.cn

T 其他语言补充                          60
来源：http://bab.dashuyun.cn

U 高频实用片段                         120
来源：http://ety.vqdsnc.cn

------------------------------------
来源：http://epf.iojbl.cn

合计                                  2106 条
来源：http://plz.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://suo.hywenlv.cn

使用提醒
来源：http://vdl.meibo888.top

--------------------------------------------------------------------------------
来源：http://kft.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vnr.jqgufenzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oca.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lxi.sjlbkw.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://avk.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qid.ppjwa.cn

—— 文件结束 ——
来源：http://qku.shanyushiyangtech.top

================================================================================
来源：http://enm.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://vsq.yonumen.top

Common Programming Examples Cheat Book
来源：http://exg.jinyuanbaomall.cn

================================================================================
来源：http://skb.xziqi.cn

【收录内容】
来源：http://xnb.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://umi.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yhw.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://ryt.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://put.ybcxt.top

【使用说明】
来源：http://svp.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pgc.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wqx.jqgfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zul.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sis.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://hew.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://irw.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tre.yuxming.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://byy.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xxz.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pzb.gotoacloud.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lhy.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dre.c1oappe.top

【文件统计】
来源：http://ept.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rcn.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://lxh.tian-w.cn

目  录
来源：http://qle.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://enj.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://msh.cashguo.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mhh.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fqh.iojbl.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tjh.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ahs.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wpy.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dge.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lhe.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gbj.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ycg.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nkc.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dxg.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://unf.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://djs.52xcode.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xwm.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vci.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://apg.yj20258888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wly.yj202588.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://grr.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zcn.sysykeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zng.xziqi.cn

================================================================================
来源：http://its.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://kve.zdqjudy.top

================================================================================
来源：http://kgt.yueranfly.top

[A01] Hello World
来源：http://dny.andypj.xyz

Py:   print("Hello, World!")
来源：http://hsq.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://jkx.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://tks.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xjy.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://cnz.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://ota.cqqwz.cn

Ruby: puts "Hello, World!"
来源：http://rnb.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cto.hesvh.cn

[A02] 变量声明与赋值
来源：http://mlm.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hff.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ica.vqdsnc.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pyg.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sex.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://ojp.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://coi.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://lfs.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://aef.sysykeji.top

[A03] 常量定义
来源：http://uft.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mco.smart0.xyz

PHP:  const PI = 3.14159;
来源：http://tnw.cucudq.cn

JS:   const PI = 3.14159;
来源：http://phm.yuxming.cn

TS:   const PI: number = 3.14159;
来源：http://xlk.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://wyg.iojbl.cn

Go:   const PI = 3.14159
来源：http://yiz.tarul.cn

Ruby: PI = 3.14159
来源：http://lbc.hnqzz.top

C#:   const double PI = 3.14159;
来源：http://otc.zhijiandao.cn

[A04] 判断变量类型
来源：http://tmq.sweek.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rtx.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xsk.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uwx.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://lfo.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zgw.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://uoj.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mxf.ehwqpu.com

C#:   x.GetType().Name; x is int
来源：http://kbe.jyoumei.cn

[A05] 整数除法与取模
来源：http://chm.c1oappe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jdm.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://syw.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gny.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vog.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://yms.dashuyun.cn

Go:   7 / 2; 7 % 2
来源：http://fic.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://xvb.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://czz.zhaomingkeji.xyz

[A06] 字符串转数字
来源：http://tzd.uphjek.com

Py:   int("42"); float("3.14")
来源：http://dio.gotoacloud.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tlq.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://apx.sweek.top

TS:   parseInt("42", 10); Number("42")
来源：http://dmh.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vmu.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ggo.sufxvd.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xaw.xylfe.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kcn.zhixingplan.top

[A07] 数字转字符串
来源：http://hhb.xuetiantiany.cn

Py:   str(42)
来源：http://kfy.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://asr.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://eqd.yfazqb.com

TS:   String(42)
来源：http://iaj.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://won.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://mlx.gaohongyu789.top

Ruby: 42.to_s
来源：http://avy.hywenlv.cn

C#:   42.ToString()
来源：http://thb.redwolf501.top

[A08] 取整与四舍五入
来源：http://cgz.aizwys.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jty.aizwys.cn


<!-- 参考信息 -->