代发 wailian999

[U57] PHP：字符串插值
来源：http://kcy.cashguo.top

"值: {$a}"
来源：http://bxs.chenlongwang.top

[U58] PHP：数组三件套
来源：http://ijz.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://byn.aibaodan.cn

[U59] PHP：自定义排序
来源：http://vcg.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://atg.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://zzd.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mnn.gaohongyu789.top

[U61] PHP：正则
来源：http://oni.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://urc.yongpay.top

[U62] PHP：日期对象
来源：http://hwt.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://him.shzxlz.cn

[U63] PHP：文件读写
来源：http://mdy.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ovk.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://npq.andypj.xyz

glob("dir/*.php");  scandir("dir");
来源：http://kse.pycfn.com

[U65] PHP：会话
来源：http://tdw.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://odf.havefunace.top

[U66] PHP：设置 Cookie
来源：http://cpj.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rkx.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://qjf.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pgo.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://yru.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iep.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://lod.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lzf.daria6918.cn

[U70] PHP：PDO 事务
来源：http://ktn.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://asp.ydzc1.top

[U71] PHP：抛出异常
来源：http://zep.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://zqo.fzhhl.top

[U72] PHP：写错误日志
来源：http://mpd.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://sdo.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://vdi.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://inx.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://paj.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://xpn.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://rsa.cdnleiting.top

composer require psr/container
来源：http://tcn.yuanzhike.top

[U76] PHP：简单路由
来源：http://ois.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tfc.hcnkem.com

[U77] PHP：模板渲染
来源：http://uxs.cashguo.top

composer require twig/twig
来源：http://jyn.yangfankeji.com

[U78] PHP：单元测试
来源：http://mtg.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://wvn.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://cpw.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://psp.wangshuangyany.cn

[U80] PHP：代码规范修复
来源：http://qvq.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://izp.xziqi.cn

[U81] JS：初始化项目
来源：http://vue.hysaishi.cn

npm init -y;  npm i express
来源：http://fkw.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://lyd.haohaochexian.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eol.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://qka.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://skl.pycfn.com

[U84] JS：CommonJS 写法
来源：http://oga.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://jtb.haohaochexian.top

[U85] JS：可选链
来源：http://lum.shuidangran.top

a?.b?.c
来源：http://eem.xziqi.cn

[U86] JS：空值合并
来源：http://xsh.bjfxy.top

a ?? b
来源：http://eat.ehwqpu.com

[U87] JS：解构默认值
来源：http://txz.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://rbh.zhengqikj.top

[U88] JS：对象展开合并
来源：http://lyo.kuanghao11.cn

{ ...a, ...b }
来源：http://waa.yj20258.top

[U89] JS：数组去重
来源：http://byg.sufxvd.cn

[...new Set(arr)]
来源：http://ocb.fzhhl.top

[U90] JS：数字数组排序
来源：http://ocv.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://wgi.yvedp.cn

[U91] JS：对象键值遍历
来源：http://eue.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xiz.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://ims.hnqzz.top

structuredClone(obj)
来源：http://tww.jiagoushi.top

[U93] JS：模板字符串
来源：http://noj.zhoulong.xyz

`共 ${n} 条`
来源：http://vmy.xylfe.cn

[U94] JS：箭头函数
来源：http://jvh.gaohongyu789.top

const double = x => x * 2;
来源：http://avo.mhx1999.top

[U95] JS：Promise 包装
来源：http://kgq.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://qtk.gzhubu.top

[U96] JS：async/await 与异常
来源：http://wue.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kdd.wangshuangyany.cn

[U97] JS：并发请求
来源：http://avd.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://teo.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://xjy.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qce.shuidangran.top

[U99] JS：事件监听
来源：http://dbv.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://uyn.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://rio.jinghuilouyu.cn

document.querySelector(".item")
来源：http://wlf.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://ses.zhoulong.xyz

el.classList.toggle("active")
来源：http://slk.kuanghao11.cn

[U102] JS：本地存储
来源：http://rlm.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vvs.52xcode.cn

[U103] JS：定时器
来源：http://lxg.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yjg.pengpengdd.cyou

[U104] JS：防抖
来源：http://vhg.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aqw.dashuyun.cn

[U105] JS：节流
来源：http://vtb.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jcm.jinqigfzy.top

[U106] JS：日期格式化
来源：http://ncy.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rwr.hysaishi.cn

[U107] JS：数字千分位
来源：http://jow.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fuf.vehdjk.com

[U108] JS：随机整数
来源：http://dhg.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nim.jlsjyb.cn

[U109] JS：数组分组
来源：http://gtu.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://roh.jlsjyb.cn

[U110] JS：数组分块
来源：http://ehm.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://niu.yj202588.top

[U111] JS：对象转 Map
来源：http://tlk.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://jja.fktsv.cn

[U112] JS：字符串补位
来源：http://usm.sufxvd.cn

"7".padStart(3, "0")
来源：http://msg.jyoumei.cn

[U113] JS：正则替换全部
来源：http://oyd.mhx1999.top

s.replaceAll("a", "b")
来源：http://qwd.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://bmp.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rbj.chenzaomai.com

[U115] JS：生成 UUID
来源：http://jll.epnwcf.com

crypto.randomUUID()
来源：http://ddx.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://fnf.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://jvx.zhijiandao.cn

[U117] JS：单元测试
来源：http://qtz.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://nuu.fktsv.cn

[U118] JS：开发服务器
来源：http://yfk.gotoacloud.top

npm i -D vite;  npx vite
来源：http://kxy.pycfn.com

[U119] JS：生产构建
来源：http://wdz.redwolf501.top

npx vite build
来源：http://mqz.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://vbz.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://qrh.yuxming.cn

================================================================================
来源：http://kal.ydzc1.top

统计汇总
来源：http://gvs.jqgufenzy.top

================================================================================
来源：http://gjy.jlsjyb.cn

按语言统计（条）：
来源：http://nlb.gzhubu.top

Python ......... 252
来源：http://zlk.zdqjudy.top

PHP ............ 252
来源：http://mvt.hfpthk.cn

JavaScript ..... 252
来源：http://kyi.fengsongda.top

TypeScript ..... 212
来源：http://oge.yj20258888.top

Java ........... 212
来源：http://hca.jinqigufen.top

Go ............. 212
来源：http://wdq.ybcxt.top

Ruby ........... 212
来源：http://wii.hfpthk.cn

C# ............. 212
来源：http://tck.jqgufenzy.top

C .............. 30
来源：http://zuv.cheryme.top

C++ ............ 30
来源：http://gnt.fzhhl.top

SQL ............ 90
来源：http://ypq.guowangkeji.top

Bash ........... 80
来源：http://czf.daxiang520.top

Kotlin ......... 15
来源：http://tgy.zhiwuduotai.top

Swift .......... 15
来源：http://isp.sjlbkw.cn

Lua ............ 10
来源：http://xgq.gotoacloud.top

Perl ........... 10
来源：http://msp.fanxiaobao.xyz

Scala .......... 10
来源：http://mvl.sufxvd.cn

------------------------------------
来源：http://btd.c1oappe.top

合计 ........... 2106 条
来源：http://oba.nanxinkj.top

按章节统计：
来源：http://ooo.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hkf.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rfo.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gcv.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xzc.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wci.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hum.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hrj.chenjidiqi.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rez.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oys.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ukx.yanxiufei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jzn.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mgr.yj20258.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://txp.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ndg.smart0.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lah.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ujr.hammf.cn

Q SQL 专题                              90
来源：http://ukx.xylfe.cn

R Bash 专题                             80
来源：http://yxo.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://wxh.zhiwuduotai.top

T 其他语言补充                          60
来源：http://kuw.hongshengwenyu.top

U 高频实用片段                         120
来源：http://lod.yongpay.top

------------------------------------
来源：http://fop.shzxlz.cn

合计                                  2106 条
来源：http://rcc.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://bez.shuidangran.top

使用提醒
来源：http://hup.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://fxk.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jnk.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ndz.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ist.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ppt.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wxe.chenzaomai.com

—— 文件结束 ——
来源：http://jhi.jinghuilouyu.cn

================================================================================
来源：http://vqn.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://hjn.cucudq.cn

Common Programming Examples Cheat Book
来源：http://qzd.ybcxt.top

================================================================================
来源：http://hpa.ydzc1.top

【收录内容】
来源：http://dqt.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tnu.kuanghao11.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://znu.bjfxy.top

SQL · Bash · C · C++
来源：http://woz.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kfo.fehbvm.com

【使用说明】
来源：http://khl.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qsw.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cxk.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eel.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vvl.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://gls.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xum.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tbn.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nmy.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uvn.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pmi.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tvm.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ijf.wangshuangyany.cn

【文件统计】
来源：http://fiu.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qpw.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://yok.smart0.xyz

目  录
来源：http://cms.xinyue.icu

--------------------------------------------------------------------------------
来源：http://bgh.sjlbkw.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wjk.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kle.cucudq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rfc.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://amr.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vbt.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zxz.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jxu.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qzk.smart0.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jex.0kj1m.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gfh.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gtu.yanxiufei.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zep.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ttc.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yop.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oti.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gcs.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jkq.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tbp.gotoacloud.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nuc.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hoj.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cqb.yuanzhike.top

================================================================================
来源：http://glc.jinqigufen.top

A. 基础语法与类型
来源：http://nbm.xylfe.cn

================================================================================
来源：http://hfv.fzhhl.top

[A01] Hello World
来源：http://erk.aizwys.cn

Py:   print("Hello, World!")
来源：http://izk.aibaodan.cn

PHP:  echo "Hello, World!";
来源：http://jta.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://yjk.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fth.fanxiaobao.xyz

Java: System.out.println("Hello, World!");
来源：http://jsn.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://zms.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://xqv.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yig.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://boa.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gqz.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qgv.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dbz.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ixz.pengpengdd.cyou

Java: String name = "Alex"; int age = 20;
来源：http://jyn.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://dfp.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://bdy.shuidangran.top

C#:   string name = "Alex"; int age = 20;
来源：http://tsi.xziqi.cn

[A03] 常量定义
来源：http://yob.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blz.yueranfly.top

PHP:  const PI = 3.14159;
来源：http://xbi.havefunace.top

JS:   const PI = 3.14159;
来源：http://ebc.zhongyouzk.top

TS:   const PI: number = 3.14159;
来源：http://sru.hammf.cn

Java: static final double PI = 3.14159;
来源：http://dmn.jinqigfzy.top

Go:   const PI = 3.14159
来源：http://odr.guannengcc.top

Ruby: PI = 3.14159
来源：http://nbk.uphjek.com

C#:   const double PI = 3.14159;
来源：http://eez.hongshengwenyu.top

[A04] 判断变量类型
来源：http://tdl.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xkq.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://enz.shanyushiyangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://syi.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://xxy.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zxe.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://krd.hywenlv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dpx.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://xvx.zhixingplan.top

[A05] 整数除法与取模
来源：http://rkn.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xtl.aizwys.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lhp.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://avo.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://czk.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://lsu.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://iea.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://ots.yvedp.cn

C#:   7 / 2; 7 % 2
来源：http://brf.wangdashe.top

[A06] 字符串转数字
来源：http://aih.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://tlj.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hsg.gogol.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vdk.tanke756.top

TS:   parseInt("42", 10); Number("42")
来源：http://aes.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mzl.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://svn.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://fmc.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hmn.sweek.top

[A07] 数字转字符串
来源：http://hyr.smart0.xyz

Py:   str(42)
来源：http://xko.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://vhv.daxiang520.top

JS:   String(42); (42).toString()
来源：http://kaf.meibo888.top

TS:   String(42)
来源：http://cpj.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ish.yj20258.top

Go:   strconv.Itoa(42)
来源：http://yul.fktsv.cn

Ruby: 42.to_s
来源：http://viu.ywan-chungtsiang.top

C#:   42.ToString()
来源：http://fbe.tian-w.cn

[A08] 取整与四舍五入
来源：http://yuy.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ojh.chenzaomai.com


<!-- 参考信息 -->