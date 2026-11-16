代发 wailian999

[U55] PHP：match 表达式
来源：http://sqy.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nbu.xinyue.icu

[U56] PHP：命名参数
来源：http://sqs.andypj.xyz

f(a: 1, b: 2)
来源：http://qxq.jyoumei.cn

[U57] PHP：字符串插值
来源：http://djv.fengsongda.top

"值: {$a}"
来源：http://gid.ywan-chungtsiang.top

[U58] PHP：数组三件套
来源：http://gff.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gvm.dianchejie.cn

[U59] PHP：自定义排序
来源：http://yym.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hnt.jlsjyb.cn

[U60] PHP：JSON 编解码
来源：http://fsv.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ohq.zhijiandao.cn

[U61] PHP：正则
来源：http://pha.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://grx.tarul.cn

[U62] PHP：日期对象
来源：http://fee.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xai.vehdjk.com

[U63] PHP：文件读写
来源：http://nsk.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yet.zhengqikj.top

[U64] PHP：目录遍历
来源：http://lgn.pycfn.com

glob("dir/*.php");  scandir("dir");
来源：http://vpp.jyoumei.cn

[U65] PHP：会话
来源：http://zgk.bbcook.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ibt.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://nmq.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rrl.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://boq.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qzo.sweek.top

[U68] PHP：PDO 连接
来源：http://csh.jqgfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ydb.yongpay.top

[U69] PHP：PDO 预处理
来源：http://zub.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fjt.hammf.cn

[U70] PHP：PDO 事务
来源：http://sps.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qob.chenlongwang.top

[U71] PHP：抛出异常
来源：http://pxc.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://qqi.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://psa.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://yoz.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://auo.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://zml.epnwcf.com

[U74] PHP：读取环境变量
来源：http://kvr.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://oym.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://png.guowangkeji.top

composer require psr/container
来源：http://ftr.mhx1999.top

[U76] PHP：简单路由
来源：http://qtk.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nsx.dashuyun.cn

[U77] PHP：模板渲染
来源：http://fas.jqgufenzy.top

composer require twig/twig
来源：http://icl.gotoacloud.top

[U78] PHP：单元测试
来源：http://kvz.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://lvm.vqdsnc.cn

[U79] PHP：静态分析
来源：http://zpo.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://ayj.xziqi.cn

[U80] PHP：代码规范修复
来源：http://ead.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kuv.dashuyun.cn

[U81] JS：初始化项目
来源：http://jxd.sysykeji.top

npm init -y;  npm i express
来源：http://thg.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://khm.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pnp.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://zqr.zdbjq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aug.meibo888.top

[U84] JS：CommonJS 写法
来源：http://ieg.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qhy.haohaochexian.top

[U85] JS：可选链
来源：http://puu.yongpay.top

a?.b?.c
来源：http://ent.tanke756.top

[U86] JS：空值合并
来源：http://qzn.zdqjudy.top

a ?? b
来源：http://fwq.zdqjudy.top

[U87] JS：解构默认值
来源：http://mwo.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://xth.yongpay.top

[U88] JS：对象展开合并
来源：http://qei.ehwqpu.com

{ ...a, ...b }
来源：http://cbj.yuxming.cn

[U89] JS：数组去重
来源：http://mzz.hammf.cn

[...new Set(arr)]
来源：http://euz.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://bjo.shzxlz.cn

[...arr].sort((a, b) => a - b)
来源：http://fbp.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://ugj.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qgo.pycfn.com

[U92] JS：深拷贝
来源：http://xdj.xuetiantiany.cn

structuredClone(obj)
来源：http://ifo.hywenlv.cn

[U93] JS：模板字符串
来源：http://hqo.cqqwz.cn

`共 ${n} 条`
来源：http://tpu.yfazqb.com

[U94] JS：箭头函数
来源：http://whe.tanke756.top

const double = x => x * 2;
来源：http://pcl.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://roy.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://jpa.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://dim.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zvy.hongshengwenyu.top

[U97] JS：并发请求
来源：http://scy.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://iij.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://ihd.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fzt.xinyue.icu

[U99] JS：事件监听
来源：http://lqw.ydjk.org.cn

el.addEventListener("click", e => {})
来源：http://keu.guannengcc.top

[U100] JS：DOM 查询
来源：http://mca.shuidangran.top

document.querySelector(".item")
来源：http://nhn.fktsv.cn

[U101] JS：classList 操作
来源：http://iuc.jinqigufen.top

el.classList.toggle("active")
来源：http://dky.aizwys.cn

[U102] JS：本地存储
来源：http://vln.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xqu.9152youxi.cn

[U103] JS：定时器
来源：http://fgv.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dqb.jinqigufen.top

[U104] JS：防抖
来源：http://bso.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnl.zdbjq.cn

[U105] JS：节流
来源：http://zzr.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jap.yueranfly.top

[U106] JS：日期格式化
来源：http://qni.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cbh.yongpay.top

[U107] JS：数字千分位
来源：http://mdm.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ldf.guowangkeji.top

[U108] JS：随机整数
来源：http://wfu.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yjh.chenzaomai.com

[U109] JS：数组分组
来源：http://yoi.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://svd.birdmap.top

[U110] JS：数组分块
来源：http://rqd.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tsl.yueranfly.top

[U111] JS：对象转 Map
来源：http://sup.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://xjv.jqgfzy.top

[U112] JS：字符串补位
来源：http://dbm.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://mrn.fktsv.cn

[U113] JS：正则替换全部
来源：http://ogw.xuanzx.com

s.replaceAll("a", "b")
来源：http://pfg.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://wrq.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ufe.xinyue.icu

[U115] JS：生成 UUID
来源：http://cpg.xuanzx.com

crypto.randomUUID()
来源：http://peu.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://cfj.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://ehi.snrcjt.cn

[U117] JS：单元测试
来源：http://aut.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://bsj.smart0.xyz

[U118] JS：开发服务器
来源：http://cxl.xziqi.cn

npm i -D vite;  npx vite
来源：http://iou.jqgufenzy.top

[U119] JS：生产构建
来源：http://idw.hnqzz.top

npx vite build
来源：http://xyp.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ayc.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://pwf.feifeiyinyue.top

================================================================================
来源：http://vfe.xziqi.cn

统计汇总
来源：http://xjg.jinyuanbaomall.cn

================================================================================
来源：http://lrp.ivvv.top

按语言统计（条）：
来源：http://glu.aizwys.cn

Python ......... 252
来源：http://iyz.ctjpmb.com

PHP ............ 252
来源：http://eaf.tian-w.cn

JavaScript ..... 252
来源：http://qme.shanyushiyangtech.top

TypeScript ..... 212
来源：http://chm.fzhhl.top

Java ........... 212
来源：http://wgi.snrcjt.cn

Go ............. 212
来源：http://jyv.jinqigufen.top

Ruby ........... 212
来源：http://wgw.yueranfly.top

C# ............. 212
来源：http://qtj.shzxlz.cn

C .............. 30
来源：http://ein.uphjek.com

C++ ............ 30
来源：http://sfv.kuanghao11.cn

SQL ............ 90
来源：http://hau.chenlongwang.top

Bash ........... 80
来源：http://znx.bjfxy.top

Kotlin ......... 15
来源：http://zki.chenlongwang.top

Swift .......... 15
来源：http://lnh.chenzaomai.com

Lua ............ 10
来源：http://xea.gogol.net.cn

Perl ........... 10
来源：http://iqa.jiagoushi.top

Scala .......... 10
来源：http://ydk.tanke756.top

------------------------------------
来源：http://xoa.yuxming.cn

合计 ........... 2106 条
来源：http://ifm.jinghuilouyu.cn

按章节统计：
来源：http://cwo.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tjg.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rsq.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ajm.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jhp.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jnw.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ikc.jiagoushi.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fus.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iki.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hnp.yj20258.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mra.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kjx.ivvv.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sfn.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zxy.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mdh.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qva.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jdl.cdnleiting.top

Q SQL 专题                              90
来源：http://ybo.chenzaomai.com

R Bash 专题                             80
来源：http://juc.yvedp.cn

S C / C++ 专题                          60
来源：http://nvg.zhijiandao.cn

T 其他语言补充                          60
来源：http://ngw.birdmap.top

U 高频实用片段                         120
来源：http://gzd.bbcook.cn

------------------------------------
来源：http://erv.jinyuanbaomall.cn

合计                                  2106 条
来源：http://dpe.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://lou.52xcode.cn

使用提醒
来源：http://hia.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://bkb.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lqe.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jas.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wum.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wpe.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xej.gotoacloud.top

—— 文件结束 ——
来源：http://ctp.ybcxt.top

================================================================================
来源：http://uyk.c1oappe.top

程序语言常见例子速查手册（2024 版）
来源：http://ovy.yfazqb.com

Common Programming Examples Cheat Book
来源：http://wsy.xuanzx.com

================================================================================
来源：http://vlq.zycfv.cn

【收录内容】
来源：http://byz.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rng.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kbq.dianchejie.cn

SQL · Bash · C · C++
来源：http://jcr.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vvu.xylfe.cn

【使用说明】
来源：http://dqx.hywenlv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rhn.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ptg.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wxt.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lzq.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hki.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rfh.jianghu66.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://agy.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nrp.tarul.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eye.ppjwa.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nmk.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ujg.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vwh.smart0.xyz

【文件统计】
来源：http://xrl.zhijiandao.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qwi.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://slo.kuanghao11.cn

目  录
来源：http://ran.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://kte.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://csz.fzhhl.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xwa.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uwn.feifeiyinyue.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tlp.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yrw.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xpp.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qnl.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qdp.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wvb.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xjy.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ubx.jinyuanbaomall.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qaw.jinghuilouyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://djl.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rwl.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fbz.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bpp.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bbt.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ywk.bbcook.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xaf.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rqe.tianlin.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vmb.yueranfly.top

================================================================================
来源：http://ihe.haohaochexian.top

A. 基础语法与类型
来源：http://ehr.kuanghao11.cn

================================================================================
来源：http://vpi.jyoumei.cn

[A01] Hello World
来源：http://adx.yfazqb.com

Py:   print("Hello, World!")
来源：http://bdd.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://uon.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://nzs.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pyo.fehbvm.com

Java: System.out.println("Hello, World!");
来源：http://una.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://ixy.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://jur.zhongyouzk.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qzd.fehbvm.com

[A02] 变量声明与赋值
来源：http://bng.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fui.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ooo.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://qcu.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fxb.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://xnj.yueranfly.top

Go:   name := "Alex"; age := 20
来源：http://szf.yj20258.top

Ruby: name = "Alex"; age = 20
来源：http://ddi.jyoumei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ayl.vqdsnc.cn

[A03] 常量定义
来源：http://wmd.yongpay.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://itr.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://csr.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://omi.zhongyouzk.top

TS:   const PI: number = 3.14159;
来源：http://gys.jqgfzy.top

Java: static final double PI = 3.14159;
来源：http://qou.svipenyu.cn

Go:   const PI = 3.14159
来源：http://xef.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://ich.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://glo.jlsjyb.cn

[A04] 判断变量类型
来源：http://kuh.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hkb.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tqs.jiagoushi.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rsj.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://ytg.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jou.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://gdz.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rhz.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://aqd.bjfxy.top

[A05] 整数除法与取模
来源：http://rfh.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iem.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ejr.ppjwa.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sdp.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yui.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://tce.yongpay.top

Go:   7 / 2; 7 % 2
来源：http://jod.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://sxs.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://aul.jinyuanbaomall.cn

[A06] 字符串转数字
来源：http://uuo.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://oiy.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uvz.c1oappe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nkz.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oyz.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ypr.quarkkingdee.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yii.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://blh.sjlbkw.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iqp.cqqwz.cn

[A07] 数字转字符串
来源：http://tpc.zhaomingkeji.xyz

Py:   str(42)
来源：http://lai.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://huq.mhx1999.top

JS:   String(42); (42).toString()
来源：http://hte.sysykeji.top

TS:   String(42)
来源：http://vth.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mdb.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://aqz.birdmap.top


<!-- 参考信息 -->