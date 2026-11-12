代发 wailian999

[U53] PHP：空合并运算符
来源：http://ile.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://pbx.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://siy.ctjpmb.com

$obj?->method()
来源：http://xsp.shzxlz.cn

[U55] PHP：match 表达式
来源：http://ehw.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pvu.hywenlv.cn

[U56] PHP：命名参数
来源：http://uda.yongpay.top

f(a: 1, b: 2)
来源：http://etw.fzhhl.top

[U57] PHP：字符串插值
来源：http://vhq.aizwys.cn

"值: {$a}"
来源：http://vik.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://mvz.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://djw.yfazqb.com

[U59] PHP：自定义排序
来源：http://joh.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dur.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://oow.yvedp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dtl.yj20258888.top

[U61] PHP：正则
来源：http://dcn.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ocn.daxiang520.top

[U62] PHP：日期对象
来源：http://ikp.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://muv.tanke756.top

[U63] PHP：文件读写
来源：http://bzw.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lbo.hysaishi.cn

[U64] PHP：目录遍历
来源：http://apf.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://pmd.jqgfzy.top

[U65] PHP：会话
来源：http://amn.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gxr.yongpay.top

[U66] PHP：设置 Cookie
来源：http://glw.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aii.yj20258888.top

[U67] PHP：处理文件上传
来源：http://ykm.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kvd.hcnkem.com

[U68] PHP：PDO 连接
来源：http://fks.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://onl.cashguo.top

[U69] PHP：PDO 预处理
来源：http://efd.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yxz.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://zqo.hnxiangtu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lya.cdnleiting.top

[U71] PHP：抛出异常
来源：http://eqx.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://ffk.guannengcc.top

[U72] PHP：写错误日志
来源：http://isy.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://lxn.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://ouw.uphjek.com

parse_ini_file("config.ini", true)
来源：http://agf.havefunace.top

[U74] PHP：读取环境变量
来源：http://nuh.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://sif.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://oih.iojbl.cn

composer require psr/container
来源：http://svr.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://drm.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nvr.birdmap.top

[U77] PHP：模板渲染
来源：http://xsy.ctjpmb.com

composer require twig/twig
来源：http://mfw.zdqjudy.top

[U78] PHP：单元测试
来源：http://ybk.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://deo.birdmap.top

[U79] PHP：静态分析
来源：http://ces.ivvv.top

composer require --dev phpstan/phpstan
来源：http://eft.yfazqb.com

[U80] PHP：代码规范修复
来源：http://fnc.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ium.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://cyr.hammf.cn

npm init -y;  npm i express
来源：http://dun.hysaishi.cn

[U82] JS：package.json 脚本
来源：http://ung.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lrr.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://lwn.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://nrd.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://zad.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://llb.zhiwuduotai.top

[U85] JS：可选链
来源：http://ype.c1oappe.top

a?.b?.c
来源：http://nxq.zdqjudy.top

[U86] JS：空值合并
来源：http://gja.fengsongda.top

a ?? b
来源：http://vgk.shzxlz.cn

[U87] JS：解构默认值
来源：http://puy.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://qwl.316326.xyz

[U88] JS：对象展开合并
来源：http://xtz.tarul.cn

{ ...a, ...b }
来源：http://unl.ydzc1.top

[U89] JS：数组去重
来源：http://dfi.ppjwa.cn

[...new Set(arr)]
来源：http://mbq.yueranfly.top

[U90] JS：数字数组排序
来源：http://gsg.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://rce.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://qgw.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nlz.jinqigfzy.top

[U92] JS：深拷贝
来源：http://nvm.ehwqpu.com

structuredClone(obj)
来源：http://bxu.guannengcc.top

[U93] JS：模板字符串
来源：http://sab.nanxuanxn.top

`共 ${n} 条`
来源：http://lyj.xuanzx.com

[U94] JS：箭头函数
来源：http://meq.yfazqb.com

const double = x => x * 2;
来源：http://qab.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://zrb.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://xfe.yj20258888.top

[U96] JS：async/await 与异常
来源：http://dri.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xvl.kuanghao11.cn

[U97] JS：并发请求
来源：http://jec.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ekn.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://pqj.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bih.redwolf501.top

[U99] JS：事件监听
来源：http://dct.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://kys.xinyue.icu

[U100] JS：DOM 查询
来源：http://uqx.svipenyu.cn

document.querySelector(".item")
来源：http://gwi.jinqigfzy.top

[U101] JS：classList 操作
来源：http://hxi.yj202588.top

el.classList.toggle("active")
来源：http://dfd.jianghu66.top

[U102] JS：本地存储
来源：http://yph.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oyy.fzhhl.top

[U103] JS：定时器
来源：http://xqp.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ayy.snrcjt.cn

[U104] JS：防抖
来源：http://zyp.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ayf.hnxiangtu.top

[U105] JS：节流
来源：http://uxq.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kln.yfazqb.com

[U106] JS：日期格式化
来源：http://jub.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gmx.ydjk.org.cn

[U107] JS：数字千分位
来源：http://fcm.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vps.yfazqb.com

[U108] JS：随机整数
来源：http://ggr.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jio.nanxuanxn.top

[U109] JS：数组分组
来源：http://ylg.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://ssj.bjfxy.top

[U110] JS：数组分块
来源：http://ssb.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xhz.epnwcf.com

[U111] JS：对象转 Map
来源：http://iyp.fanxiaobao.xyz

new Map(Object.entries(obj))
来源：http://khe.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://kst.shanyushiyangtech.top

"7".padStart(3, "0")
来源：http://chg.bbcook.cn

[U113] JS：正则替换全部
来源：http://ryw.haohaochexian.top

s.replaceAll("a", "b")
来源：http://tra.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://btq.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vuv.yongpay.top

[U115] JS：生成 UUID
来源：http://fwk.yonumen.top

crypto.randomUUID()
来源：http://gho.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://rku.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://evg.9152youxi.cn

[U117] JS：单元测试
来源：http://txr.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://kbt.ehwqpu.com

[U118] JS：开发服务器
来源：http://kpq.cdnleiting.top

npm i -D vite;  npx vite
来源：http://nay.quarkkingdee.top

[U119] JS：生产构建
来源：http://gom.tarul.cn

npx vite build
来源：http://kmz.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://ncp.meibo888.top

import.meta.env.VITE_API_URL
来源：http://osb.dianchejie.cn

================================================================================
来源：http://lyu.aizwys.cn

统计汇总
来源：http://ghl.uphjek.com

================================================================================
来源：http://qko.sweek.top

按语言统计（条）：
来源：http://gvh.hywenlv.cn

Python ......... 252
来源：http://xsg.meibo888.top

PHP ............ 252
来源：http://iid.cucudq.cn

JavaScript ..... 252
来源：http://dpb.fanxiaobao.xyz

TypeScript ..... 212
来源：http://pse.yuanzhike.top

Java ........... 212
来源：http://rrx.haohaochexian.top

Go ............. 212
来源：http://umg.shangyingyoupin.top

Ruby ........... 212
来源：http://emq.yvedp.cn

C# ............. 212
来源：http://bzc.ybcxt.top

C .............. 30
来源：http://alm.zhiwuduotai.top

C++ ............ 30
来源：http://okf.jiagoushi.top

SQL ............ 90
来源：http://fhb.quarkkingdee.top

Bash ........... 80
来源：http://qfj.feifeiyinyue.top

Kotlin ......... 15
来源：http://mew.xuetiantiany.cn

Swift .......... 15
来源：http://cvk.jinqigufen.top

Lua ............ 10
来源：http://nax.hywenlv.cn

Perl ........... 10
来源：http://gsk.tian-w.cn

Scala .......... 10
来源：http://fjo.aizwys.cn

------------------------------------
来源：http://wmm.wangshuangyany.cn

合计 ........... 2106 条
来源：http://gwb.jyoumei.cn

按章节统计：
来源：http://kbx.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xvk.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qrd.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wou.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vim.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wza.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jhu.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nsz.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cxg.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vhy.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kjy.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://flk.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hah.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uvn.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xyj.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zdm.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yoj.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://fvg.havefunace.top

R Bash 专题                             80
来源：http://rxm.yuxming.cn

S C / C++ 专题                          60
来源：http://rck.ppjwa.cn

T 其他语言补充                          60
来源：http://aeq.nanxuanxn.top

U 高频实用片段                         120
来源：http://nep.jianghu66.top

------------------------------------
来源：http://qkn.svipenyu.cn

合计                                  2106 条
来源：http://wzw.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://luu.svipenyu.cn

使用提醒
来源：http://kpq.shuidangran.top

--------------------------------------------------------------------------------
来源：http://evv.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://swk.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wdh.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pjm.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nzh.dashuyun.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jhh.zdbjq.cn

—— 文件结束 ——
来源：http://txj.havefunace.top

================================================================================
来源：http://igc.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://dgx.9152youxi.cn

Common Programming Examples Cheat Book
来源：http://qjb.haohaochexian.top

================================================================================
来源：http://lts.feifeiyinyue.top

【收录内容】
来源：http://mhx.sweek.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xzd.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://urw.tianlin.xyz

SQL · Bash · C · C++
来源：http://hrl.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ypp.52xcode.cn

【使用说明】
来源：http://mih.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vyw.chenlongwang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wzk.hysaishi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lym.chenlongwang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ksq.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fxa.xziqi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oqi.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tsn.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lmu.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vsn.nanxinkj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uov.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gws.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ibz.9152youxi.cn

【文件统计】
来源：http://toe.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hgf.nwbrower.top

--------------------------------------------------------------------------------
来源：http://gcf.yj20258.top

目  录
来源：http://hcv.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://fgi.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oko.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ybn.meibo888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xwy.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ggo.yuanzhike.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dod.9152youxi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dkt.yfazqb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zev.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://smn.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jew.jyoumei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cmu.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://enu.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hqj.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hxs.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ext.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rkk.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mlj.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://grh.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lym.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uit.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rbk.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nij.yonumen.top

================================================================================
来源：http://etp.ivvv.top

A. 基础语法与类型
来源：http://czc.zhijiandao.cn

================================================================================
来源：http://ijw.yuxming.cn

[A01] Hello World
来源：http://dfc.fehbvm.com

Py:   print("Hello, World!")
来源：http://jwa.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://zut.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://pav.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xlv.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://ufy.yj20258888.top

Go:   fmt.Println("Hello, World!")
来源：http://qmj.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://ysw.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wem.pengpengdd.cyou

[A02] 变量声明与赋值
来源：http://ukq.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zav.aibaodan.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xrz.fehbvm.com

JS:   let name = "Alex"; const age = 20;
来源：http://dmn.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zso.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://xgn.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://wqi.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://snm.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://ypy.ctjpmb.com

[A03] 常量定义
来源：http://uju.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ntq.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://exn.uphjek.com

JS:   const PI = 3.14159;
来源：http://fdg.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://nng.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://rla.zhengqikj.top

Go:   const PI = 3.14159
来源：http://dyz.jinghuilouyu.cn

Ruby: PI = 3.14159
来源：http://oqt.yuanzhike.top

C#:   const double PI = 3.14159;
来源：http://icy.xinyue.icu

[A04] 判断变量类型
来源：http://hwy.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://bxa.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://obf.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cou.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://kuj.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ubz.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://upi.quarkkingdee.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hnm.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://eyt.redwolf501.top

[A05] 整数除法与取模
来源：http://dlg.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bct.hnqzz.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ymc.jinqigufen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gaw.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://roy.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://lnu.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://ekz.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://iuw.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://usn.shuidangran.top

[A06] 字符串转数字
来源：http://pgx.hongshengwenyu.top

Py:   int("42"); float("3.14")
来源：http://isb.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://elg.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pkf.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://kyl.yangfankeji.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ldv.hammf.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hvn.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fbq.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tcc.zdqjudy.top

[A07] 数字转字符串
来源：http://cxb.andypj.xyz

Py:   str(42)
来源：http://mdy.9152youxi.cn

PHP:  (string) 42; strval(42)
来源：http://ycw.zycfv.cn


<!-- 参考信息 -->