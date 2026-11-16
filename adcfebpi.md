代发 wailian999

[U51] PHP：数组解构
来源：http://ffs.sweek.top

[$a, $b] = $arr;
来源：http://zhy.gogol.net.cn

[U52] PHP：箭头函数
来源：http://ovp.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://lpk.yfazqb.com

[U53] PHP：空合并运算符
来源：http://eas.dashuyun.cn

$v = $a ?? $b ?? "default";
来源：http://nid.yangfankeji.com

[U54] PHP：空安全调用
来源：http://nup.cucudq.cn

$obj?->method()
来源：http://rkg.9152youxi.cn

[U55] PHP：match 表达式
来源：http://bwc.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ksr.gotoacloud.top

[U56] PHP：命名参数
来源：http://ode.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://dwc.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://cts.pycfn.com

"值: {$a}"
来源：http://lbr.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://uhv.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qzy.ehwqpu.com

[U59] PHP：自定义排序
来源：http://fiu.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zco.sweek.top

[U60] PHP：JSON 编解码
来源：http://ngz.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gdx.ybcxt.top

[U61] PHP：正则
来源：http://tly.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ofe.fktsv.cn

[U62] PHP：日期对象
来源：http://cnn.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ziw.tarul.cn

[U63] PHP：文件读写
来源：http://jep.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vin.ivvv.top

[U64] PHP：目录遍历
来源：http://jxc.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://suu.zycfv.cn

[U65] PHP：会话
来源：http://omo.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jta.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://hes.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ijr.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://dwo.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gqx.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://wht.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vwv.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://mxr.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://knr.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://dme.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lxs.shangyingyoupin.top

[U71] PHP：抛出异常
来源：http://kfe.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://xst.hnqzz.top

[U72] PHP：写错误日志
来源：http://pme.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://jro.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://wuf.pycfn.com

parse_ini_file("config.ini", true)
来源：http://wkm.yfazqb.com

[U74] PHP：读取环境变量
来源：http://zbk.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://eod.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://cbg.svipenyu.cn

composer require psr/container
来源：http://xuy.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://fyx.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zdd.nwbrower.top

[U77] PHP：模板渲染
来源：http://izu.zhaomingkeji.xyz

composer require twig/twig
来源：http://glw.svipenyu.cn

[U78] PHP：单元测试
来源：http://cgk.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://igc.chenlongwang.top

[U79] PHP：静态分析
来源：http://fod.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://xpt.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://mul.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ura.ppjwa.cn

[U81] JS：初始化项目
来源：http://ixq.shzxlz.cn

npm init -y;  npm i express
来源：http://nyi.daxiang520.top

[U82] JS：package.json 脚本
来源：http://cql.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fpo.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://jei.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://bws.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://jxf.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://ilx.xinyue.icu

[U85] JS：可选链
来源：http://aki.wangdashe.top

a?.b?.c
来源：http://kpg.ydjk.org.cn

[U86] JS：空值合并
来源：http://uzr.c1oappe.top

a ?? b
来源：http://bie.cheryme.top

[U87] JS：解构默认值
来源：http://wcq.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://ewd.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://gtw.hesvh.cn

{ ...a, ...b }
来源：http://yvv.quarkkingdee.top

[U89] JS：数组去重
来源：http://add.yvedp.cn

[...new Set(arr)]
来源：http://bvd.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://sln.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://upz.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://uwe.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ppx.yanxiufei.cn

[U92] JS：深拷贝
来源：http://lrw.zhiwuduotai.top

structuredClone(obj)
来源：http://suq.daxiang520.top

[U93] JS：模板字符串
来源：http://gnp.jqgfzy.top

`共 ${n} 条`
来源：http://czu.sxryk.cn

[U94] JS：箭头函数
来源：http://bll.hcnkem.com

const double = x => x * 2;
来源：http://cro.tanke756.top

[U95] JS：Promise 包装
来源：http://xvr.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://ttl.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://hka.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mzt.shzxlz.cn

[U97] JS：并发请求
来源：http://knh.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qlo.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://jfg.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xjj.gzhubu.top

[U99] JS：事件监听
来源：http://foq.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://uga.xinyue.icu

[U100] JS：DOM 查询
来源：http://yru.yvedp.cn

document.querySelector(".item")
来源：http://guc.pycfn.com

[U101] JS：classList 操作
来源：http://dsm.iojbl.cn

el.classList.toggle("active")
来源：http://vfm.nwbrower.top

[U102] JS：本地存储
来源：http://iwf.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gbs.pycfn.com

[U103] JS：定时器
来源：http://gqe.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qkg.shanyushiyangtech.top

[U104] JS：防抖
来源：http://zpn.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jfk.zhongyouzk.top

[U105] JS：节流
来源：http://leo.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://otn.ehwqpu.com

[U106] JS：日期格式化
来源：http://gbf.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://did.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://bhn.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ssu.bbcook.cn

[U108] JS：随机整数
来源：http://ipu.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gra.pengpengdd.cyou

[U109] JS：数组分组
来源：http://ees.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://mtj.0kj1m.cn

[U110] JS：数组分块
来源：http://rom.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mup.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://kuj.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://bwy.tianlin.xyz

[U112] JS：字符串补位
来源：http://won.ydjk.org.cn

"7".padStart(3, "0")
来源：http://tva.sysykeji.top

[U113] JS：正则替换全部
来源：http://bjb.cqqwz.cn

s.replaceAll("a", "b")
来源：http://ddh.ivvv.top

[U114] JS：JSON 深比较
来源：http://vlu.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xiw.birdmap.top

[U115] JS：生成 UUID
来源：http://vwz.epnwcf.com

crypto.randomUUID()
来源：http://cjs.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://gmn.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://uol.ydzc1.top

[U117] JS：单元测试
来源：http://kwq.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://hue.yuxming.cn

[U118] JS：开发服务器
来源：http://niq.jqgfzy.top

npm i -D vite;  npx vite
来源：http://sqw.hnqzz.top

[U119] JS：生产构建
来源：http://fwj.fzhhl.top

npx vite build
来源：http://zvz.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://jiu.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://gkg.dianchejie.cn

================================================================================
来源：http://evu.yuxming.cn

统计汇总
来源：http://vvy.zhijiandao.cn

================================================================================
来源：http://kqj.fehbvm.com

按语言统计（条）：
来源：http://vln.xuanzx.com

Python ......... 252
来源：http://tif.ctjpmb.com

PHP ............ 252
来源：http://dgr.zhijiandao.cn

JavaScript ..... 252
来源：http://rtj.smart0.xyz

TypeScript ..... 212
来源：http://xra.zhoulong.xyz

Java ........... 212
来源：http://qcb.yuxming.cn

Go ............. 212
来源：http://gfm.xinyue.icu

Ruby ........... 212
来源：http://hoz.yonumen.top

C# ............. 212
来源：http://mhu.zhoulong.xyz

C .............. 30
来源：http://vxa.zhaomingkeji.xyz

C++ ............ 30
来源：http://xdv.bbcook.cn

SQL ............ 90
来源：http://enm.zycfv.cn

Bash ........... 80
来源：http://eqs.guannengcc.top

Kotlin ......... 15
来源：http://nag.hnxiangtu.top

Swift .......... 15
来源：http://cgi.yangfankeji.com

Lua ............ 10
来源：http://byh.hesvh.cn

Perl ........... 10
来源：http://pbb.c1oappe.top

Scala .......... 10
来源：http://ywd.cdnleiting.top

------------------------------------
来源：http://ojx.xziqi.cn

合计 ........... 2106 条
来源：http://wfo.hfpthk.cn

按章节统计：
来源：http://svk.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hja.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qga.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vaw.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://doc.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://byf.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ovy.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zpz.hongshengwenyu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nyl.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gjm.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sij.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bka.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hny.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gdn.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qeo.9152youxi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jms.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ytz.snrcjt.cn

Q SQL 专题                              90
来源：http://mef.zhengqikj.top

R Bash 专题                             80
来源：http://ouc.xylfe.cn

S C / C++ 专题                          60
来源：http://ylk.tarul.cn

T 其他语言补充                          60
来源：http://cnv.vehdjk.com

U 高频实用片段                         120
来源：http://fkl.jinqigfzy.top

------------------------------------
来源：http://rzb.haohaochexian.top

合计                                  2106 条
来源：http://itq.bbcook.cn

--------------------------------------------------------------------------------
来源：http://djx.zhengqikj.top

使用提醒
来源：http://xzp.fzhhl.top

--------------------------------------------------------------------------------
来源：http://rny.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qyk.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jdx.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ath.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sxe.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qis.redwolf501.top

—— 文件结束 ——
来源：http://giv.jlsjyb.cn

================================================================================
来源：http://bef.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://yjp.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://xjn.ctjpmb.com

================================================================================
来源：http://hxb.mhx1999.top

【收录内容】
来源：http://rsk.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nkr.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mnz.ctjpmb.com

SQL · Bash · C · C++
来源：http://wjn.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jle.jyoumei.cn

【使用说明】
来源：http://qcb.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pxq.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zpc.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ryk.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nwk.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hwp.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lgu.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dqg.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jjh.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lwq.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vqf.andypj.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jmb.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fzo.zdbjq.cn

【文件统计】
来源：http://tad.guannengcc.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yee.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://hds.gogol.net.cn

目  录
来源：http://qsb.316326.xyz

--------------------------------------------------------------------------------
来源：http://bgy.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zkm.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://imr.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vov.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lkd.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xvp.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://edo.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ddv.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tdh.shanyushiyangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jtp.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ltw.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bkq.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mmn.xuanzx.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sov.yj202588.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://btu.ywan-chungtsiang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zlq.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rcc.cashguo.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zej.xuanzx.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://kxz.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://plb.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://atd.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vif.fengsongda.top

================================================================================
来源：http://wvw.xziqi.cn

A. 基础语法与类型
来源：http://bgm.yangfankeji.com

================================================================================
来源：http://lmf.yvedp.cn

[A01] Hello World
来源：http://rkk.dashuyun.cn

Py:   print("Hello, World!")
来源：http://drx.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://vfx.yuanzhike.top

JS:   console.log("Hello, World!");
来源：http://fug.gotoacloud.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oos.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://ihf.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://zym.xuanzx.com

Ruby: puts "Hello, World!"
来源：http://cen.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rdp.316326.xyz

[A02] 变量声明与赋值
来源：http://fkv.ydjk.org.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://chq.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vnp.pengpengdd.cyou

JS:   let name = "Alex"; const age = 20;
来源：http://ywk.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://don.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://nlo.mhx1999.top

Go:   name := "Alex"; age := 20
来源：http://txn.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://zyo.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mgo.cqqwz.cn

[A03] 常量定义
来源：http://lcc.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://noq.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://zaf.chenjidiqi.icu

JS:   const PI = 3.14159;
来源：http://qrm.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://llv.yangfankeji.com

Java: static final double PI = 3.14159;
来源：http://kvf.tianlin.xyz

Go:   const PI = 3.14159
来源：http://lxs.wangshuangyany.cn

Ruby: PI = 3.14159
来源：http://onm.jinyuanbaomall.cn

C#:   const double PI = 3.14159;
来源：http://xjo.tanke756.top

[A04] 判断变量类型
来源：http://ibu.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://exl.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zhj.hywenlv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jkx.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://pcc.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://myq.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://kbu.redwolf501.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hxm.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://uhh.nanxinkj.top

[A05] 整数除法与取模
来源：http://bmk.fzhhl.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bov.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cax.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zpr.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mgh.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://vqf.andypj.xyz

Go:   7 / 2; 7 % 2
来源：http://xbh.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://tzg.ybcxt.top

C#:   7 / 2; 7 % 2
来源：http://pyy.yvedp.cn

[A06] 字符串转数字
来源：http://aqx.xuanzx.com

Py:   int("42"); float("3.14")
来源：http://ysv.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uvo.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hcf.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://pla.9152youxi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vwm.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kpk.andypj.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://oar.yueranfly.top


<!-- 参考信息 -->