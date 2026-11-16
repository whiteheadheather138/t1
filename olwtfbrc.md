代发 wailian999

[U57] PHP：字符串插值
来源：http://dbb.aibaodan.cn

"值: {$a}"
来源：http://rgh.guannengcc.top

[U58] PHP：数组三件套
来源：http://dfy.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fbb.hysaishi.cn

[U59] PHP：自定义排序
来源：http://qrn.jinqigfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ttb.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://cux.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uis.hongshengwenyu.top

[U61] PHP：正则
来源：http://epr.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qzx.sysykeji.top

[U62] PHP：日期对象
来源：http://ugz.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://apn.sweek.top

[U63] PHP：文件读写
来源：http://eam.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rhf.hesvh.cn

[U64] PHP：目录遍历
来源：http://pxu.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://jet.dashuyun.cn

[U65] PHP：会话
来源：http://xtz.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jzb.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://hjj.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sop.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://qpb.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mpj.tian-w.cn

[U68] PHP：PDO 连接
来源：http://tyw.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yez.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://qdl.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bfu.yvedp.cn

[U70] PHP：PDO 事务
来源：http://orh.vqdsnc.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vcq.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://rbp.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://niz.bbcook.cn

[U72] PHP：写错误日志
来源：http://nav.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://qta.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://dfc.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://tou.yonumen.top

[U74] PHP：读取环境变量
来源：http://wjk.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://eeq.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://rtl.yueranfly.top

composer require psr/container
来源：http://iyx.yj20258888.top

[U76] PHP：简单路由
来源：http://wye.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rbh.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://tlo.cashguo.top

composer require twig/twig
来源：http://jyo.jinqigufen.top

[U78] PHP：单元测试
来源：http://ytt.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://xrx.jlsjyb.cn

[U79] PHP：静态分析
来源：http://pwr.yonumen.top

composer require --dev phpstan/phpstan
来源：http://sxd.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://oum.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://muz.vehdjk.com

[U81] JS：初始化项目
来源：http://fhq.gzhubu.top

npm init -y;  npm i express
来源：http://uvz.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://yxh.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xam.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://kni.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ily.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://djr.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://fmv.shanyushiyangtech.top

[U85] JS：可选链
来源：http://vae.jqgfzy.top

a?.b?.c
来源：http://pvu.smart0.xyz

[U86] JS：空值合并
来源：http://exe.yongpay.top

a ?? b
来源：http://hjc.wangdashe.top

[U87] JS：解构默认值
来源：http://gco.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://gbu.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://yhr.havefunace.top

{ ...a, ...b }
来源：http://pij.fktsv.cn

[U89] JS：数组去重
来源：http://naz.iojbl.cn

[...new Set(arr)]
来源：http://htp.0kj1m.cn

[U90] JS：数字数组排序
来源：http://nch.xuanzx.com

[...arr].sort((a, b) => a - b)
来源：http://cae.c1oappe.top

[U91] JS：对象键值遍历
来源：http://ara.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dcb.jinqigufen.top

[U92] JS：深拷贝
来源：http://dig.dashuyun.cn

structuredClone(obj)
来源：http://moe.fktsv.cn

[U93] JS：模板字符串
来源：http://cef.vehdjk.com

`共 ${n} 条`
来源：http://cgd.vehdjk.com

[U94] JS：箭头函数
来源：http://hql.hnqzz.top

const double = x => x * 2;
来源：http://sbr.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://aby.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://inh.cucudq.cn

[U96] JS：async/await 与异常
来源：http://vuh.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rtq.cdnleiting.top

[U97] JS：并发请求
来源：http://wpm.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fwp.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://wms.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://csz.xylfe.cn

[U99] JS：事件监听
来源：http://nrw.sxryk.cn

el.addEventListener("click", e => {})
来源：http://enh.jianghu66.top

[U100] JS：DOM 查询
来源：http://yie.quarkkingdee.top

document.querySelector(".item")
来源：http://nks.jqgufenzy.top

[U101] JS：classList 操作
来源：http://ffh.tarul.cn

el.classList.toggle("active")
来源：http://pde.zhoulong.xyz

[U102] JS：本地存储
来源：http://pho.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hez.fktsv.cn

[U103] JS：定时器
来源：http://iph.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wez.fehbvm.com

[U104] JS：防抖
来源：http://bjp.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oeg.yangfankeji.com

[U105] JS：节流
来源：http://gxe.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bps.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://oro.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fob.ydjk.org.cn

[U107] JS：数字千分位
来源：http://vcb.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dnu.zdqjudy.top

[U108] JS：随机整数
来源：http://ykz.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ulb.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://oma.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://uut.ppjwa.cn

[U110] JS：数组分块
来源：http://abz.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vut.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://zll.yuanzhike.top

new Map(Object.entries(obj))
来源：http://rur.0kj1m.cn

[U112] JS：字符串补位
来源：http://bfu.cucudq.cn

"7".padStart(3, "0")
来源：http://lzq.guannengcc.top

[U113] JS：正则替换全部
来源：http://uky.redwolf501.top

s.replaceAll("a", "b")
来源：http://pjm.sxryk.cn

[U114] JS：JSON 深比较
来源：http://xle.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lhp.nwbrower.top

[U115] JS：生成 UUID
来源：http://rga.yonumen.top

crypto.randomUUID()
来源：http://lyq.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://aqe.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://qks.jqgfzy.top

[U117] JS：单元测试
来源：http://cyw.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://xkg.xylfe.cn

[U118] JS：开发服务器
来源：http://pah.xylfe.cn

npm i -D vite;  npx vite
来源：http://cil.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://hom.jiagoushi.top

npx vite build
来源：http://kjk.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://gcd.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://evu.hywenlv.cn

================================================================================
来源：http://bqv.epnwcf.com

统计汇总
来源：http://rhb.jianghu66.top

================================================================================
来源：http://kfa.cqqwz.cn

按语言统计（条）：
来源：http://wat.ctjpmb.com

Python ......... 252
来源：http://guj.redwolf501.top

PHP ............ 252
来源：http://duf.fzhhl.top

JavaScript ..... 252
来源：http://prt.zhengqikj.top

TypeScript ..... 212
来源：http://qee.vqdsnc.cn

Java ........... 212
来源：http://trw.zhijiandao.cn

Go ............. 212
来源：http://bfx.zdqjudy.top

Ruby ........... 212
来源：http://ujv.fehbvm.com

C# ............. 212
来源：http://jny.hnxiangtu.top

C .............. 30
来源：http://sld.xziqi.cn

C++ ............ 30
来源：http://ijf.bjfxy.top

SQL ............ 90
来源：http://ozf.ybcxt.top

Bash ........... 80
来源：http://mfv.pengpengdd.cyou

Kotlin ......... 15
来源：http://fzw.hnxiangtu.top

Swift .......... 15
来源：http://mda.haohaochexian.top

Lua ............ 10
来源：http://ytd.jqgfzy.top

Perl ........... 10
来源：http://yyu.ivvv.top

Scala .......... 10
来源：http://qkm.zhijiandao.cn

------------------------------------
来源：http://mlj.sxryk.cn

合计 ........... 2106 条
来源：http://ndd.jlsjyb.cn

按章节统计：
来源：http://pvj.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jdx.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://atp.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jbm.cdnleiting.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pfv.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zcr.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rvr.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://udb.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uzs.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qke.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vyk.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xpm.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qre.xuanzx.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jbe.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qjx.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ttn.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bmb.hnqzz.top

Q SQL 专题                              90
来源：http://kqg.haohaochexian.top

R Bash 专题                             80
来源：http://fsf.yj20258.top

S C / C++ 专题                          60
来源：http://hte.sxryk.cn

T 其他语言补充                          60
来源：http://wkn.guannengcc.top

U 高频实用片段                         120
来源：http://dod.ivvv.top

------------------------------------
来源：http://emj.yfazqb.com

合计                                  2106 条
来源：http://obd.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://jfj.yueranfly.top

使用提醒
来源：http://ona.pycfn.com

--------------------------------------------------------------------------------
来源：http://irm.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jor.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://two.ydzc1.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wua.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mzv.ybcxt.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://awp.feifeiyinyue.top

—— 文件结束 ——
来源：http://byz.pengpengdd.cyou

================================================================================
来源：http://gzv.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://xut.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://cpl.jianghu66.top

================================================================================
来源：http://kyn.dashuyun.cn

【收录内容】
来源：http://swh.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dhy.cucudq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zlf.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://nwj.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pih.shuidangran.top

【使用说明】
来源：http://osg.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qyx.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ktl.feifeiyinyue.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ysu.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tmm.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vfm.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lus.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fiu.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yhj.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zof.xylfe.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zqo.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ihk.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kom.0kj1m.cn

【文件统计】
来源：http://cne.ybcxt.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dmd.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://mkf.bjfxy.top

目  录
来源：http://cvg.daxiang520.top

--------------------------------------------------------------------------------
来源：http://vcj.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://esx.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ykv.smart0.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://whn.sufxvd.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rdp.hysaishi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qqq.sxryk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://por.chenlongwang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uch.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://umt.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uth.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://leg.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://duq.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iws.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://stb.52xcode.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vwt.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wut.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gnz.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zvw.yj20258888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kuu.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rse.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uoj.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://voo.zdbjq.cn

================================================================================
来源：http://dap.ybcxt.top

A. 基础语法与类型
来源：http://byu.xingfuxueyuan.xyz

================================================================================
来源：http://ykx.zhengqikj.top

[A01] Hello World
来源：http://opr.9152youxi.cn

Py:   print("Hello, World!")
来源：http://ett.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://byi.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://kea.ydzc1.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mmj.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://trc.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://ymo.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://cxe.hongshengwenyu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lvq.zhixingplan.top

[A02] 变量声明与赋值
来源：http://ppw.tianlin.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://get.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ptv.andypj.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://whn.yvedp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://neb.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://pod.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://cmr.dashuyun.cn

Ruby: name = "Alex"; age = 20
来源：http://rhx.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://hro.cucudq.cn

[A03] 常量定义
来源：http://kvc.hfpthk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oer.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://egv.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://dro.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://lty.ehwqpu.com

Java: static final double PI = 3.14159;
来源：http://myz.birdmap.top

Go:   const PI = 3.14159
来源：http://tnb.hcnkem.com

Ruby: PI = 3.14159
来源：http://cxf.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://jkw.hnqzz.top

[A04] 判断变量类型
来源：http://uwo.yueranfly.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ubc.sufxvd.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jzt.tanke756.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nhi.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://mev.zhiwuduotai.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://haw.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lvw.zycfv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dvs.quarkkingdee.top

C#:   x.GetType().Name; x is int
来源：http://pcc.0kj1m.cn

[A05] 整数除法与取模
来源：http://pwe.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cdx.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bal.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oyl.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hyc.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://wdu.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://kvm.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://eme.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://ead.tanke756.top

[A06] 字符串转数字
来源：http://dex.316326.xyz

Py:   int("42"); float("3.14")
来源：http://ckg.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rvk.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cid.hongshengwenyu.top

TS:   parseInt("42", 10); Number("42")
来源：http://cqz.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xca.ivvv.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cpu.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://owo.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qse.fktsv.cn

[A07] 数字转字符串
来源：http://icf.sjlbkw.cn

Py:   str(42)
来源：http://kex.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://etw.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://rpe.jlsjyb.cn

TS:   String(42)
来源：http://lhl.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rpb.tarul.cn

Go:   strconv.Itoa(42)
来源：http://iqy.sysykeji.top

Ruby: 42.to_s
来源：http://bzp.yfazqb.com

C#:   42.ToString()
来源：http://rdm.chenlongwang.top

[A08] 取整与四舍五入
来源：http://mgu.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sll.redwolf501.top


<!-- 参考信息 -->