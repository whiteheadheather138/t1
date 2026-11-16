代发 wailian999

[U59] PHP：自定义排序
来源：http://jnx.chenzaomai.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yuw.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://pfc.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bth.52xcode.cn

[U61] PHP：正则
来源：http://ayf.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kbz.daxiang520.top

[U62] PHP：日期对象
来源：http://lha.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xov.ydjk.org.cn

[U63] PHP：文件读写
来源：http://ebn.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zoz.zycfv.cn

[U64] PHP：目录遍历
来源：http://suz.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://lhk.chenlongwang.top

[U65] PHP：会话
来源：http://cqz.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://zdh.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://toh.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://use.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://hlt.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xdz.birdmap.top

[U68] PHP：PDO 连接
来源：http://jlf.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qrs.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://bfu.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yrx.yj20258.top

[U70] PHP：PDO 事务
来源：http://jpc.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qxn.shuidangran.top

[U71] PHP：抛出异常
来源：http://edm.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://irx.yueranfly.top

[U72] PHP：写错误日志
来源：http://aqv.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://bpc.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://rcl.yj202588.top

parse_ini_file("config.ini", true)
来源：http://rog.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://abt.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://cfx.jiagoushi.top

[U75] PHP：依赖注入
来源：http://xuh.wangdashe.top

composer require psr/container
来源：http://gto.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://qbu.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pzl.c1oappe.top

[U77] PHP：模板渲染
来源：http://squ.9152youxi.cn

composer require twig/twig
来源：http://tol.pycfn.com

[U78] PHP：单元测试
来源：http://nmk.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://orq.hywenlv.cn

[U79] PHP：静态分析
来源：http://uvt.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://ivs.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://qtx.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jdb.c1oappe.top

[U81] JS：初始化项目
来源：http://tih.chenlongwang.top

npm init -y;  npm i express
来源：http://nwc.fzhhl.top

[U82] JS：package.json 脚本
来源：http://yza.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mfm.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://pbj.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://ysu.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://tfa.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dcq.pycfn.com

[U85] JS：可选链
来源：http://tbl.fzhhl.top

a?.b?.c
来源：http://xuy.yuanzhike.top

[U86] JS：空值合并
来源：http://bxp.shzxlz.cn

a ?? b
来源：http://wzl.hnqzz.top

[U87] JS：解构默认值
来源：http://era.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://jsk.shuidangran.top

[U88] JS：对象展开合并
来源：http://zhy.zdqjudy.top

{ ...a, ...b }
来源：http://sbc.yuxming.cn

[U89] JS：数组去重
来源：http://ony.wangdashe.top

[...new Set(arr)]
来源：http://glq.jiagoushi.top

[U90] JS：数字数组排序
来源：http://flw.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://iql.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://pom.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jcd.gogol.net.cn

[U92] JS：深拷贝
来源：http://qkn.cheryme.top

structuredClone(obj)
来源：http://ztp.yueranfly.top

[U93] JS：模板字符串
来源：http://xey.xylfe.cn

`共 ${n} 条`
来源：http://tfu.svipenyu.cn

[U94] JS：箭头函数
来源：http://rbj.shzxlz.cn

const double = x => x * 2;
来源：http://ywd.xziqi.cn

[U95] JS：Promise 包装
来源：http://szg.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://vdl.smart0.xyz

[U96] JS：async/await 与异常
来源：http://btd.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kgv.xuanzx.com

[U97] JS：并发请求
来源：http://fbl.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cxz.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://ojn.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fsc.zhongyouzk.top

[U99] JS：事件监听
来源：http://xxq.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://zlv.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://pbc.zycfv.cn

document.querySelector(".item")
来源：http://smr.hnqzz.top

[U101] JS：classList 操作
来源：http://iot.zhoulong.xyz

el.classList.toggle("active")
来源：http://gvy.yj202588.top

[U102] JS：本地存储
来源：http://zug.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dzr.havefunace.top

[U103] JS：定时器
来源：http://epl.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://urv.hnxiangtu.top

[U104] JS：防抖
来源：http://jfx.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ydv.hongshengwenyu.top

[U105] JS：节流
来源：http://pfs.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aiv.pycfn.com

[U106] JS：日期格式化
来源：http://dij.mhx1999.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jxd.hysaishi.cn

[U107] JS：数字千分位
来源：http://jvw.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qvj.bbcook.cn

[U108] JS：随机整数
来源：http://kkn.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gln.bjfxy.top

[U109] JS：数组分组
来源：http://iuw.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://fma.jiagoushi.top

[U110] JS：数组分块
来源：http://lwh.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xux.ppjwa.cn

[U111] JS：对象转 Map
来源：http://szp.yj20258.top

new Map(Object.entries(obj))
来源：http://smr.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://lah.aizwys.cn

"7".padStart(3, "0")
来源：http://btv.52xcode.cn

[U113] JS：正则替换全部
来源：http://xhw.iojbl.cn

s.replaceAll("a", "b")
来源：http://lno.hammf.cn

[U114] JS：JSON 深比较
来源：http://jyk.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zca.dashuyun.cn

[U115] JS：生成 UUID
来源：http://itx.ppjwa.cn

crypto.randomUUID()
来源：http://vxe.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://tjb.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://xlh.wangshuangyany.cn

[U117] JS：单元测试
来源：http://fld.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://chs.316326.xyz

[U118] JS：开发服务器
来源：http://hxs.ydzc1.top

npm i -D vite;  npx vite
来源：http://xam.hesvh.cn

[U119] JS：生产构建
来源：http://rae.jqgfzy.top

npx vite build
来源：http://fro.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://rbb.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://xub.yj202588.top

================================================================================
来源：http://axj.hnxiangtu.top

统计汇总
来源：http://dmu.havefunace.top

================================================================================
来源：http://wpj.c1oappe.top

按语言统计（条）：
来源：http://yum.cucudq.cn

Python ......... 252
来源：http://xni.quarkkingdee.top

PHP ............ 252
来源：http://cfe.pycfn.com

JavaScript ..... 252
来源：http://jvg.fanxiaobao.xyz

TypeScript ..... 212
来源：http://fdz.fengsongda.top

Java ........... 212
来源：http://wma.yj20258888.top

Go ............. 212
来源：http://bud.gzhubu.top

Ruby ........... 212
来源：http://xwh.hysaishi.cn

C# ............. 212
来源：http://ecc.pycfn.com

C .............. 30
来源：http://xbc.xylfe.cn

C++ ............ 30
来源：http://dwo.shanyushiyangkeji.top

SQL ............ 90
来源：http://sjp.sufxvd.cn

Bash ........... 80
来源：http://bmb.ydjk.org.cn

Kotlin ......... 15
来源：http://pjq.yj20258888.top

Swift .......... 15
来源：http://ocu.sysykeji.top

Lua ............ 10
来源：http://ynb.sysykeji.top

Perl ........... 10
来源：http://jkj.kuanghao11.cn

Scala .......... 10
来源：http://qba.jinghuilouyu.cn

------------------------------------
来源：http://obh.cqqwz.cn

合计 ........... 2106 条
来源：http://rpl.c1oappe.top

按章节统计：
来源：http://ntw.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://suv.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dyl.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mvh.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://csx.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kah.svipenyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ntl.tian-w.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://otu.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rgo.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://byd.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lzn.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nwq.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qpu.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mal.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nof.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uel.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mut.sufxvd.cn

Q SQL 专题                              90
来源：http://rbb.feifeiyinyue.top

R Bash 专题                             80
来源：http://eql.epnwcf.com

S C / C++ 专题                          60
来源：http://vox.jiagoushi.top

T 其他语言补充                          60
来源：http://egr.wangdashe.top

U 高频实用片段                         120
来源：http://mlj.iojbl.cn

------------------------------------
来源：http://zul.yfazqb.com

合计                                  2106 条
来源：http://dnl.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://jhk.yj202588.top

使用提醒
来源：http://igk.cashguo.top

--------------------------------------------------------------------------------
来源：http://ive.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wnu.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mxu.yueranfly.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zzj.yongpay.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ayw.aizwys.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hhi.snrcjt.cn

—— 文件结束 ——
来源：http://evt.52xcode.cn

================================================================================
来源：http://mgd.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://hlt.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://gzs.hnqzz.top

================================================================================
来源：http://giv.tarul.cn

【收录内容】
来源：http://ots.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://aaw.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://acd.vqdsnc.cn

SQL · Bash · C · C++
来源：http://dix.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mjb.pengpengdd.cyou

【使用说明】
来源：http://izl.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://alg.sweek.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kyx.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://emc.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rxf.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hhi.fengsongda.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bvh.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vhf.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://byp.gaohongyu789.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nju.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mtf.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dwr.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bez.fzhhl.top

【文件统计】
来源：http://bxb.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mlv.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://gvn.hywenlv.cn

目  录
来源：http://vth.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://rjn.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aze.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oco.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hdg.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ajx.ppjwa.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zte.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zgy.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tga.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fuu.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dje.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mce.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qot.yanxiufei.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ino.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hda.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mad.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wqr.yanxiufei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jwq.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://axf.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cds.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dkf.fzhhl.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jdh.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://czp.xylfe.cn

================================================================================
来源：http://mfo.ehwqpu.com

A. 基础语法与类型
来源：http://uue.xingfuxueyuan.xyz

================================================================================
来源：http://oug.yongpay.top

[A01] Hello World
来源：http://xrf.zdqjudy.top

Py:   print("Hello, World!")
来源：http://gay.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://wfw.shuidangran.top

JS:   console.log("Hello, World!");
来源：http://hsh.yongpay.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fxi.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://pdh.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://oqq.fehbvm.com

Ruby: puts "Hello, World!"
来源：http://ywa.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qbk.uphjek.com

[A02] 变量声明与赋值
来源：http://jsa.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kqi.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wox.gzhubu.top

JS:   let name = "Alex"; const age = 20;
来源：http://big.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xuk.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://jrz.haohaochexian.top

Go:   name := "Alex"; age := 20
来源：http://wrq.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://ijh.jyoumei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vub.0kj1m.cn

[A03] 常量定义
来源：http://fof.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iku.yueranfly.top

PHP:  const PI = 3.14159;
来源：http://xje.tarul.cn

JS:   const PI = 3.14159;
来源：http://glq.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://eqn.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://njg.chenjidiqi.icu

Go:   const PI = 3.14159
来源：http://eow.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://ecc.wangdashe.top

C#:   const double PI = 3.14159;
来源：http://wla.yfazqb.com

[A04] 判断变量类型
来源：http://ojf.jinghuilouyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vfw.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dps.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rnx.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://zgm.chenjidiqi.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qsi.yueranfly.top

Go:   reflect.TypeOf(x).Name()
来源：http://wic.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bau.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://jwq.nwbrower.top

[A05] 整数除法与取模
来源：http://bom.pycfn.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://opl.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://sln.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cwi.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dsg.yuxming.cn

Java: 7 / 2; 7 % 2
来源：http://wtv.0kj1m.cn

Go:   7 / 2; 7 % 2
来源：http://cks.birdmap.top

Ruby: 7 / 2; 7 % 2
来源：http://vlw.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://mff.zhongyouzk.top

[A06] 字符串转数字
来源：http://xlm.zhengqikj.top

Py:   int("42"); float("3.14")
来源：http://rkt.mhx1999.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ezt.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wks.svipenyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tvr.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ieg.birdmap.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wtg.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mym.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gum.fengsongda.top

[A07] 数字转字符串
来源：http://xnh.feifeiyinyue.top

Py:   str(42)
来源：http://ete.meibo888.top

PHP:  (string) 42; strval(42)
来源：http://ckr.yueranfly.top

JS:   String(42); (42).toString()
来源：http://tgs.chenjidiqi.icu

TS:   String(42)
来源：http://jxe.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://dku.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://ygk.epnwcf.com

Ruby: 42.to_s
来源：http://qxm.hcnkem.com

C#:   42.ToString()
来源：http://doe.yangfankeji.com

[A08] 取整与四舍五入
来源：http://ukg.52xcode.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://siy.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nxv.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kdk.hywenlv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tif.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vwj.yueranfly.top


<!-- 参考信息 -->