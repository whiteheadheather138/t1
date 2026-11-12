代发 wailian999

[U47] PHP：联合类型
来源：http://dod.xuanzx.com

int|string $id
来源：http://uqe.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://vvw.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://abs.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://jgg.jqgfzy.top

public readonly string $name
来源：http://kbp.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://ffm.gzhubu.top

public function __construct(private int $id) {}
来源：http://dmv.0kj1m.cn

[U51] PHP：数组解构
来源：http://srd.bjfxy.top

[$a, $b] = $arr;
来源：http://olz.jyoumei.cn

[U52] PHP：箭头函数
来源：http://rrh.zdqjudy.top

$double = fn($x) => $x * 2;
来源：http://qcy.52xcode.cn

[U53] PHP：空合并运算符
来源：http://jjn.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://abt.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://pyi.feifeiyinyue.top

$obj?->method()
来源：http://any.gzhubu.top

[U55] PHP：match 表达式
来源：http://zta.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vdd.sufxvd.cn

[U56] PHP：命名参数
来源：http://wpv.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://kjd.havefunace.top

[U57] PHP：字符串插值
来源：http://nrz.fehbvm.com

"值: {$a}"
来源：http://sci.birdmap.top

[U58] PHP：数组三件套
来源：http://kdw.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://slm.zdbjq.cn

[U59] PHP：自定义排序
来源：http://jvd.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cpf.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://ulq.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ngd.zhongyouzk.top

[U61] PHP：正则
来源：http://iqk.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hwc.yj202588.top

[U62] PHP：日期对象
来源：http://rhm.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zwh.zhongyouzk.top

[U63] PHP：文件读写
来源：http://tve.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lzg.nwbrower.top

[U64] PHP：目录遍历
来源：http://ssz.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://ban.jinqigufen.top

[U65] PHP：会话
来源：http://tux.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://fxg.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://hpk.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bgp.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://wal.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://daz.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://uzh.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nwl.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://jnp.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aga.daria6918.cn

[U70] PHP：PDO 事务
来源：http://amx.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://afh.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://bnh.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://ydk.snrcjt.cn

[U72] PHP：写错误日志
来源：http://eph.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://yqi.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://zlp.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://har.mhx1999.top

[U74] PHP：读取环境变量
来源：http://hkt.hongshengwenyu.top

getenv("APP_ENV") ?: "production"
来源：http://spu.yvedp.cn

[U75] PHP：依赖注入
来源：http://mas.hnqzz.top

composer require psr/container
来源：http://ehh.zhoulong.xyz

[U76] PHP：简单路由
来源：http://txj.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qnw.uphjek.com

[U77] PHP：模板渲染
来源：http://ern.jianghu66.top

composer require twig/twig
来源：http://qba.smart0.xyz

[U78] PHP：单元测试
来源：http://rnk.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://pjk.jqgufenzy.top

[U79] PHP：静态分析
来源：http://lbt.havefunace.top

composer require --dev phpstan/phpstan
来源：http://zby.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://pwy.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://zen.jianghu66.top

[U81] JS：初始化项目
来源：http://rys.sysykeji.top

npm init -y;  npm i express
来源：http://zrb.sweek.top

[U82] JS：package.json 脚本
来源：http://qqk.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zks.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://auv.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://axp.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://yud.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://lyl.mhx1999.top

[U85] JS：可选链
来源：http://pyq.uphjek.com

a?.b?.c
来源：http://xgl.nanxinkj.top

[U86] JS：空值合并
来源：http://ocf.hcnkem.com

a ?? b
来源：http://dvs.aibaodan.cn

[U87] JS：解构默认值
来源：http://vns.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://yln.fengsongda.top

[U88] JS：对象展开合并
来源：http://byx.snrcjt.cn

{ ...a, ...b }
来源：http://wht.shzxlz.cn

[U89] JS：数组去重
来源：http://rcb.yongpay.top

[...new Set(arr)]
来源：http://zes.hywenlv.cn

[U90] JS：数字数组排序
来源：http://whf.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://axy.xinyue.icu

[U91] JS：对象键值遍历
来源：http://goy.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://not.cucudq.cn

[U92] JS：深拷贝
来源：http://jhd.pengpengdd.cyou

structuredClone(obj)
来源：http://gci.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://zhw.fktsv.cn

`共 ${n} 条`
来源：http://sot.yfazqb.com

[U94] JS：箭头函数
来源：http://yyd.sjlbkw.cn

const double = x => x * 2;
来源：http://zgr.hnqzz.top

[U95] JS：Promise 包装
来源：http://pqr.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://elz.nwbrower.top

[U96] JS：async/await 与异常
来源：http://uwc.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ngg.cucudq.cn

[U97] JS：并发请求
来源：http://mio.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://bkd.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://lpq.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cfa.meibo888.top

[U99] JS：事件监听
来源：http://uru.yueranfly.top

el.addEventListener("click", e => {})
来源：http://qoe.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://gzi.hywenlv.cn

document.querySelector(".item")
来源：http://lbl.jiagoushi.top

[U101] JS：classList 操作
来源：http://tql.bjfxy.top

el.classList.toggle("active")
来源：http://dvz.redwolf501.top

[U102] JS：本地存储
来源：http://jjk.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ljg.fengsongda.top

[U103] JS：定时器
来源：http://clu.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tyn.yonumen.top

[U104] JS：防抖
来源：http://dmm.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fps.zhongyouzk.top

[U105] JS：节流
来源：http://quh.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vaf.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://cjf.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kpp.tian-w.cn

[U107] JS：数字千分位
来源：http://dic.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iep.zdqjudy.top

[U108] JS：随机整数
来源：http://fdd.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dmy.sjlbkw.cn

[U109] JS：数组分组
来源：http://eyy.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://pnl.yfazqb.com

[U110] JS：数组分块
来源：http://rvw.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lhv.tian-w.cn

[U111] JS：对象转 Map
来源：http://jbw.jiagoushi.top

new Map(Object.entries(obj))
来源：http://skd.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://neh.birdmap.top

"7".padStart(3, "0")
来源：http://ohg.yj20258.top

[U113] JS：正则替换全部
来源：http://vhp.gaohongyu789.top

s.replaceAll("a", "b")
来源：http://hpu.xylfe.cn

[U114] JS：JSON 深比较
来源：http://wkd.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ezz.ehwqpu.com

[U115] JS：生成 UUID
来源：http://iui.tarul.cn

crypto.randomUUID()
来源：http://ake.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://hml.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://lih.ydzc1.top

[U117] JS：单元测试
来源：http://ron.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://xjo.ivvv.top

[U118] JS：开发服务器
来源：http://pze.svipenyu.cn

npm i -D vite;  npx vite
来源：http://geb.snrcjt.cn

[U119] JS：生产构建
来源：http://iks.hongshengwenyu.top

npx vite build
来源：http://aou.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://ctr.tarul.cn

import.meta.env.VITE_API_URL
来源：http://nxr.pengpengdd.cyou

================================================================================
来源：http://gfs.daria6918.cn

统计汇总
来源：http://hbh.ivvv.top

================================================================================
来源：http://cxy.ydzc1.top

按语言统计（条）：
来源：http://liy.zdqjudy.top

Python ......... 252
来源：http://dqu.smart0.xyz

PHP ............ 252
来源：http://dgx.yonumen.top

JavaScript ..... 252
来源：http://qzh.iojbl.cn

TypeScript ..... 212
来源：http://kwl.sjlbkw.cn

Java ........... 212
来源：http://oky.nanxinkj.top

Go ............. 212
来源：http://aee.yueranfly.top

Ruby ........... 212
来源：http://qvm.hnxiangtu.top

C# ............. 212
来源：http://uxi.nwbrower.top

C .............. 30
来源：http://rmw.yangfankeji.com

C++ ............ 30
来源：http://dhx.pycfn.com

SQL ............ 90
来源：http://mbl.jqgufenzy.top

Bash ........... 80
来源：http://stm.cdnleiting.top

Kotlin ......... 15
来源：http://uav.havefunace.top

Swift .......... 15
来源：http://xxc.yonumen.top

Lua ............ 10
来源：http://hqg.sysykeji.top

Perl ........... 10
来源：http://zmy.jianghu66.top

Scala .......... 10
来源：http://ooj.cashguo.top

------------------------------------
来源：http://swn.ybcxt.top

合计 ........... 2106 条
来源：http://tcx.tanke756.top

按章节统计：
来源：http://ebx.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qng.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wwi.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dih.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wjd.ydjk.org.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rfu.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gui.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iou.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ejz.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ajg.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cdj.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vja.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yev.yongpay.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jee.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ocl.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jjv.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cqe.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://mmi.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://zwz.epnwcf.com

S C / C++ 专题                          60
来源：http://opl.ydzc1.top

T 其他语言补充                          60
来源：http://ifx.zhaomingkeji.xyz

U 高频实用片段                         120
来源：http://ngl.zdbjq.cn

------------------------------------
来源：http://boz.hfpthk.cn

合计                                  2106 条
来源：http://bfx.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://rht.aizwys.cn

使用提醒
来源：http://ysr.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://mzv.jinqigufen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rsr.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vpn.xingfuxueyuan.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fzr.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://cgw.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xog.ctjpmb.com

—— 文件结束 ——
来源：http://lts.yangfankeji.com

================================================================================
来源：http://pzu.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://cfq.xylfe.cn

Common Programming Examples Cheat Book
来源：http://vlv.fehbvm.com

================================================================================
来源：http://wqx.tanke756.top

【收录内容】
来源：http://odd.chenlongwang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jtf.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jlp.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://skd.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://toc.hywenlv.cn

【使用说明】
来源：http://ofe.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eqr.fzhhl.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pbr.pycfn.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iax.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vmw.sufxvd.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kib.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wac.tian-w.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zhz.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wsi.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oig.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ure.fktsv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://afs.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zdf.hywenlv.cn

【文件统计】
来源：http://geo.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tmr.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://jeh.aizwys.cn

目  录
来源：http://alp.ivvv.top

--------------------------------------------------------------------------------
来源：http://new.xinyue.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gch.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uvd.ppjwa.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gql.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uca.52xcode.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ukb.zhengqikj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hyk.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://isn.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qyl.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xou.zdbjq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iet.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qhi.hcnkem.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jwg.quarkkingdee.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rgt.yj202588.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://saq.andypj.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mum.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tmr.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://whl.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tik.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fdh.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbd.cucudq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://anz.quarkkingdee.top

================================================================================
来源：http://ipv.chenzaomai.com

A. 基础语法与类型
来源：http://cwg.yuxming.cn

================================================================================
来源：http://lmu.zhixingplan.top

[A01] Hello World
来源：http://tni.bbcook.cn

Py:   print("Hello, World!")
来源：http://hwj.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://lnr.hammf.cn

JS:   console.log("Hello, World!");
来源：http://mzc.yuanzhike.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uad.nanxinkj.top

Java: System.out.println("Hello, World!");
来源：http://cqz.jinqigfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://ssg.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://zsf.shzxlz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dps.haohaochexian.top

[A02] 变量声明与赋值
来源：http://kma.jyoumei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nca.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bhv.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://gxk.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pjs.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://gcx.hongshengwenyu.top

Go:   name := "Alex"; age := 20
来源：http://zoz.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://fvi.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zti.jqgfzy.top

[A03] 常量定义
来源：http://mxy.hnxiangtu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://chx.chenjidiqi.icu

PHP:  const PI = 3.14159;
来源：http://foq.yj20258888.top

JS:   const PI = 3.14159;
来源：http://rir.ehwqpu.com

TS:   const PI: number = 3.14159;
来源：http://xkk.vehdjk.com

Java: static final double PI = 3.14159;
来源：http://mpj.cashguo.top

Go:   const PI = 3.14159
来源：http://ixt.jyoumei.cn

Ruby: PI = 3.14159
来源：http://pvn.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://zsz.cdnleiting.top

[A04] 判断变量类型
来源：http://srx.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://orq.ehwqpu.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yju.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qcm.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://gpr.vehdjk.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dxk.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://bqb.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yox.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://fyl.fktsv.cn

[A05] 整数除法与取模
来源：http://wgv.wangdashe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://coe.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://bdm.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kkf.hnxiangtu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mpj.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://lxl.ppjwa.cn

Go:   7 / 2; 7 % 2
来源：http://hdl.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://hjz.hcnkem.com

C#:   7 / 2; 7 % 2
来源：http://ygd.daria6918.cn


<!-- 参考信息 -->