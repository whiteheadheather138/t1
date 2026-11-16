代发 wailian999

[U55] PHP：match 表达式
来源：http://vbs.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uym.yangfankeji.com

[U56] PHP：命名参数
来源：http://nyo.yanxiufei.cn

f(a: 1, b: 2)
来源：http://uoq.iojbl.cn

[U57] PHP：字符串插值
来源：http://gmg.hcnkem.com

"值: {$a}"
来源：http://xum.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://pfn.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qlu.birdmap.top

[U59] PHP：自定义排序
来源：http://oxf.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vyk.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://ero.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tpy.ydjk.org.cn

[U61] PHP：正则
来源：http://ffj.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mvt.yvedp.cn

[U62] PHP：日期对象
来源：http://uqc.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jkm.xuanzx.com

[U63] PHP：文件读写
来源：http://aql.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lfm.svipenyu.cn

[U64] PHP：目录遍历
来源：http://jtk.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://bgx.iojbl.cn

[U65] PHP：会话
来源：http://cbx.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wbn.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://zwb.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ykh.jinyuanbaomall.cn

[U67] PHP：处理文件上传
来源：http://qnx.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zyc.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://hvo.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ace.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://mig.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://moo.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://wey.xylfe.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pdt.uphjek.com

[U71] PHP：抛出异常
来源：http://vqx.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://axn.zhengqikj.top

[U72] PHP：写错误日志
来源：http://hiz.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://bys.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://xzh.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://dgj.xylfe.cn

[U74] PHP：读取环境变量
来源：http://yau.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://tvh.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://vss.shuidangran.top

composer require psr/container
来源：http://fmp.kuanghao11.cn

[U76] PHP：简单路由
来源：http://bnx.shzxlz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mts.tanke756.top

[U77] PHP：模板渲染
来源：http://jol.shzxlz.cn

composer require twig/twig
来源：http://mvd.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://rzm.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://tfh.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://ibu.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://jfe.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://ula.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zqi.quarkkingdee.top

[U81] JS：初始化项目
来源：http://npi.yongpay.top

npm init -y;  npm i express
来源：http://cfm.cheryme.top

[U82] JS：package.json 脚本
来源：http://nhj.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://drx.jlsjyb.cn

[U83] JS：ES Module 导入导出
来源：http://qpc.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://gtn.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://vou.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://css.redwolf501.top

[U85] JS：可选链
来源：http://zbw.hammf.cn

a?.b?.c
来源：http://tfo.epnwcf.com

[U86] JS：空值合并
来源：http://npz.bbcook.cn

a ?? b
来源：http://ufg.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://cfy.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://ply.uphjek.com

[U88] JS：对象展开合并
来源：http://rgj.jianghu66.top

{ ...a, ...b }
来源：http://jmc.svipenyu.cn

[U89] JS：数组去重
来源：http://ubv.shuidangran.top

[...new Set(arr)]
来源：http://wvp.xylfe.cn

[U90] JS：数字数组排序
来源：http://gix.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://bak.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://zyw.52xcode.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gqf.yangfankeji.com

[U92] JS：深拷贝
来源：http://ssw.sxryk.cn

structuredClone(obj)
来源：http://hhj.yueranfly.top

[U93] JS：模板字符串
来源：http://hnx.daria6918.cn

`共 ${n} 条`
来源：http://sso.yj20258.top

[U94] JS：箭头函数
来源：http://itg.meibo888.top

const double = x => x * 2;
来源：http://eol.smart0.xyz

[U95] JS：Promise 包装
来源：http://bms.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://qwr.yj202588.top

[U96] JS：async/await 与异常
来源：http://zbg.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xju.ctjpmb.com

[U97] JS：并发请求
来源：http://edx.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ahp.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://zsp.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cpb.zhengqikj.top

[U99] JS：事件监听
来源：http://jkn.tian-w.cn

el.addEventListener("click", e => {})
来源：http://imj.mhx1999.top

[U100] JS：DOM 查询
来源：http://hqm.andypj.xyz

document.querySelector(".item")
来源：http://ane.tanke756.top

[U101] JS：classList 操作
来源：http://zhg.zhixingplan.top

el.classList.toggle("active")
来源：http://gcc.yj202588.top

[U102] JS：本地存储
来源：http://pqk.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tbz.pycfn.com

[U103] JS：定时器
来源：http://jgu.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rcl.shuidangran.top

[U104] JS：防抖
来源：http://hpf.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zuu.daria6918.cn

[U105] JS：节流
来源：http://hca.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uzt.hnxiangtu.top

[U106] JS：日期格式化
来源：http://vbu.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ymd.ppjwa.cn

[U107] JS：数字千分位
来源：http://aeq.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hht.zhengqikj.top

[U108] JS：随机整数
来源：http://rfp.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://glq.chenzaomai.com

[U109] JS：数组分组
来源：http://tdt.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://hxd.shanyushiyangtech.top

[U110] JS：数组分块
来源：http://tgn.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pdj.svipenyu.cn

[U111] JS：对象转 Map
来源：http://wgw.daria6918.cn

new Map(Object.entries(obj))
来源：http://zfv.zhongyouzk.top

[U112] JS：字符串补位
来源：http://cmz.redwolf501.top

"7".padStart(3, "0")
来源：http://der.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://fzx.9152youxi.cn

s.replaceAll("a", "b")
来源：http://knb.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://bxc.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ewk.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://ozb.guowangkeji.top

crypto.randomUUID()
来源：http://kdj.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://uva.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://nyp.xuetiantiany.cn

[U117] JS：单元测试
来源：http://snu.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://odo.chenlongwang.top

[U118] JS：开发服务器
来源：http://kld.ydzc1.top

npm i -D vite;  npx vite
来源：http://qcl.zhoulong.xyz

[U119] JS：生产构建
来源：http://dwp.yj202588.top

npx vite build
来源：http://ief.xingfuxueyuan.xyz

[U120] JS：读取环境变量（Vite）
来源：http://vgb.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://jzn.hnxiangtu.top

================================================================================
来源：http://egq.daxiang520.top

统计汇总
来源：http://oag.ydzc1.top

================================================================================
来源：http://mcp.yongpay.top

按语言统计（条）：
来源：http://yvg.vehdjk.com

Python ......... 252
来源：http://wuq.52xcode.cn

PHP ............ 252
来源：http://gzi.nanxuanxn.top

JavaScript ..... 252
来源：http://zqm.yonumen.top

TypeScript ..... 212
来源：http://ynu.zhengqikj.top

Java ........... 212
来源：http://duq.cashguo.top

Go ............. 212
来源：http://wre.cheryme.top

Ruby ........... 212
来源：http://cka.chenjidiqi.icu

C# ............. 212
来源：http://vay.shangyingyoupin.top

C .............. 30
来源：http://hnh.jinghuilouyu.cn

C++ ............ 30
来源：http://jjm.guowangkeji.top

SQL ............ 90
来源：http://ryg.iojbl.cn

Bash ........... 80
来源：http://ccr.bjfxy.top

Kotlin ......... 15
来源：http://ysv.svipenyu.cn

Swift .......... 15
来源：http://ihh.xinyue.icu

Lua ............ 10
来源：http://joy.aizwys.cn

Perl ........... 10
来源：http://nel.zdbjq.cn

Scala .......... 10
来源：http://wdd.yvedp.cn

------------------------------------
来源：http://iyz.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://hez.xingfuxueyuan.xyz

按章节统计：
来源：http://lye.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://avx.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://suf.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://htu.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nsl.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fbw.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tqa.yvedp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tcg.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ymo.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ogd.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lxa.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tvl.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cls.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dtg.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ept.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://phj.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hgy.cqqwz.cn

Q SQL 专题                              90
来源：http://zza.zycfv.cn

R Bash 专题                             80
来源：http://fzg.shzxlz.cn

S C / C++ 专题                          60
来源：http://mvf.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://czr.zdqjudy.top

U 高频实用片段                         120
来源：http://abt.hongshengwenyu.top

------------------------------------
来源：http://jol.jqgufenzy.top

合计                                  2106 条
来源：http://keb.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://wug.svipenyu.cn

使用提醒
来源：http://con.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://ibs.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xbq.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ntd.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dqs.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://lyf.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ulb.hywenlv.cn

—— 文件结束 ——
来源：http://lhx.ybcxt.top

================================================================================
来源：http://mmj.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://cst.yuxming.cn

Common Programming Examples Cheat Book
来源：http://ttx.yueranfly.top

================================================================================
来源：http://ghf.fehbvm.com

【收录内容】
来源：http://jje.shuidangran.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lco.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://smn.kuanghao11.cn

SQL · Bash · C · C++
来源：http://lkx.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gwz.fzhhl.top

【使用说明】
来源：http://bla.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kwr.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jek.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vod.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rzt.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://sfs.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qwf.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hbv.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fvc.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tve.cqqwz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://avv.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ixq.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ggp.xziqi.cn

【文件统计】
来源：http://uth.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yxd.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://oba.jyoumei.cn

目  录
来源：http://yrp.xuanzx.com

--------------------------------------------------------------------------------
来源：http://jiw.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mur.chenzaomai.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fxi.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bss.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tlo.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://utu.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bdg.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ryf.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fgt.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xli.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ufl.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rkt.yj20258888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qgl.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gyn.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://puc.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nmr.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ryd.ywan-chungtsiang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lgd.shanyushiyangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wbz.feifeiyinyue.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bmt.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pcy.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fvx.ybcxt.top

================================================================================
来源：http://loo.jiagoushi.top

A. 基础语法与类型
来源：http://wzs.bbcook.cn

================================================================================
来源：http://rhn.gzhubu.top

[A01] Hello World
来源：http://aho.yangfankeji.com

Py:   print("Hello, World!")
来源：http://phd.mhx1999.top

PHP:  echo "Hello, World!";
来源：http://fyn.fehbvm.com

JS:   console.log("Hello, World!");
来源：http://bbo.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://umu.ydjk.org.cn

Java: System.out.println("Hello, World!");
来源：http://zjr.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://zuv.yj202588.top

Ruby: puts "Hello, World!"
来源：http://lyk.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lmp.zhongyouzk.top

[A02] 变量声明与赋值
来源：http://mlq.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cvo.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yri.cdnleiting.top

JS:   let name = "Alex"; const age = 20;
来源：http://oqy.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zuz.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://eqg.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://wyh.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://eyd.aibaodan.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ipt.0kj1m.cn

[A03] 常量定义
来源：http://wij.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bdr.52xcode.cn

PHP:  const PI = 3.14159;
来源：http://qir.52xcode.cn

JS:   const PI = 3.14159;
来源：http://cio.birdmap.top

TS:   const PI: number = 3.14159;
来源：http://wzl.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://cql.dianchejie.cn

Go:   const PI = 3.14159
来源：http://pxg.smart0.xyz

Ruby: PI = 3.14159
来源：http://nmz.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://ewj.daxiang520.top

[A04] 判断变量类型
来源：http://bbv.pengpengdd.cyou

Py:   type(x).__name__; isinstance(x, int)
来源：http://jtf.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://npx.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nvw.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://aar.zhoulong.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qio.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://opf.andypj.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://bvu.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://gna.zycfv.cn

[A05] 整数除法与取模
来源：http://knb.fktsv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vtf.quarkkingdee.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uew.jianghu66.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qtf.xuetiantiany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qyt.smart0.xyz

Java: 7 / 2; 7 % 2
来源：http://vgf.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://swd.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://npa.bbcook.cn

C#:   7 / 2; 7 % 2
来源：http://xuh.mhx1999.top

[A06] 字符串转数字
来源：http://ema.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://rpb.hammf.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lgk.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dte.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://yje.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ett.jiagoushi.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://plq.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xtq.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ibf.tanke756.top

[A07] 数字转字符串
来源：http://dhc.jqgufenzy.top

Py:   str(42)
来源：http://nrf.dashuyun.cn

PHP:  (string) 42; strval(42)
来源：http://bom.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://sdx.tianlin.xyz

TS:   String(42)
来源：http://bfb.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hlt.ctjpmb.com

Go:   strconv.Itoa(42)
来源：http://teg.tianlin.xyz


<!-- 参考信息 -->