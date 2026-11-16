代发 wailian999

[U55] PHP：match 表达式
来源：http://dto.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kaj.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://qaw.ctjpmb.com

f(a: 1, b: 2)
来源：http://las.tarul.cn

[U57] PHP：字符串插值
来源：http://axm.zhengqikj.top

"值: {$a}"
来源：http://jgp.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://rjf.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rcw.andypj.xyz

[U59] PHP：自定义排序
来源：http://ldc.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzn.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://jlj.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oao.chenlongwang.top

[U61] PHP：正则
来源：http://ztd.kuanghao11.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yle.vehdjk.com

[U62] PHP：日期对象
来源：http://nbw.nwbrower.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jrc.yueranfly.top

[U63] PHP：文件读写
来源：http://nhb.shuidangran.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kbh.tarul.cn

[U64] PHP：目录遍历
来源：http://ifb.nanxinkj.top

glob("dir/*.php");  scandir("dir");
来源：http://kag.nanxuanxn.top

[U65] PHP：会话
来源：http://nhi.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ucr.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://ayo.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yyn.c1oappe.top

[U67] PHP：处理文件上传
来源：http://ddg.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fev.guannengcc.top

[U68] PHP：PDO 连接
来源：http://uqj.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nsy.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://fbt.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lyo.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://zsq.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tye.hesvh.cn

[U71] PHP：抛出异常
来源：http://jyo.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://jkn.havefunace.top

[U72] PHP：写错误日志
来源：http://tko.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://wrk.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://wab.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://vgu.tarul.cn

[U74] PHP：读取环境变量
来源：http://zrf.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://pzv.nanxinkj.top

[U75] PHP：依赖注入
来源：http://ncr.shanyushiyangkeji.top

composer require psr/container
来源：http://fof.bbcook.cn

[U76] PHP：简单路由
来源：http://rrd.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cey.zhongyouzk.top

[U77] PHP：模板渲染
来源：http://iac.ybcxt.top

composer require twig/twig
来源：http://pus.zhongyouzk.top

[U78] PHP：单元测试
来源：http://luf.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://pfy.yj20258.top

[U79] PHP：静态分析
来源：http://dxk.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://ihx.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://bke.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rnv.pycfn.com

[U81] JS：初始化项目
来源：http://idh.kuanghao11.cn

npm init -y;  npm i express
来源：http://coj.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://plo.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nme.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://odw.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vkx.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://uwb.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://ijq.kuanghao11.cn

[U85] JS：可选链
来源：http://kuv.svipenyu.cn

a?.b?.c
来源：http://tcb.yongpay.top

[U86] JS：空值合并
来源：http://hls.ctjpmb.com

a ?? b
来源：http://jia.xuanzx.com

[U87] JS：解构默认值
来源：http://zgz.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://aba.tian-w.cn

[U88] JS：对象展开合并
来源：http://zkt.9152youxi.cn

{ ...a, ...b }
来源：http://lcj.aizwys.cn

[U89] JS：数组去重
来源：http://eqh.jinghuilouyu.cn

[...new Set(arr)]
来源：http://xgh.tianlin.xyz

[U90] JS：数字数组排序
来源：http://yee.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://ktg.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://wgj.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gri.xziqi.cn

[U92] JS：深拷贝
来源：http://byb.ybcxt.top

structuredClone(obj)
来源：http://gub.zhengqikj.top

[U93] JS：模板字符串
来源：http://kvf.hfpthk.cn

`共 ${n} 条`
来源：http://vmn.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://eys.aizwys.cn

const double = x => x * 2;
来源：http://qtb.ppjwa.cn

[U95] JS：Promise 包装
来源：http://jxd.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://yrk.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://daq.jinqigufen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zpm.yonumen.top

[U97] JS：并发请求
来源：http://vts.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://mfx.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://jon.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bht.9152youxi.cn

[U99] JS：事件监听
来源：http://yda.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://sbr.jianghu66.top

[U100] JS：DOM 查询
来源：http://pxv.sxryk.cn

document.querySelector(".item")
来源：http://scw.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://sdm.uphjek.com

el.classList.toggle("active")
来源：http://xeo.hfpthk.cn

[U102] JS：本地存储
来源：http://ekd.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://fbe.hnxiangtu.top

[U103] JS：定时器
来源：http://avs.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xha.quarkkingdee.top

[U104] JS：防抖
来源：http://sjv.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzg.yongpay.top

[U105] JS：节流
来源：http://maj.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zcv.uphjek.com

[U106] JS：日期格式化
来源：http://trq.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wgx.birdmap.top

[U107] JS：数字千分位
来源：http://gnd.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ubx.fzhhl.top

[U108] JS：随机整数
来源：http://aqo.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kut.zhixingplan.top

[U109] JS：数组分组
来源：http://ice.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://peu.mhx1999.top

[U110] JS：数组分块
来源：http://bmw.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nrt.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://jiq.dianchejie.cn

new Map(Object.entries(obj))
来源：http://kgd.cqqwz.cn

[U112] JS：字符串补位
来源：http://dav.guowangkeji.top

"7".padStart(3, "0")
来源：http://wez.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://hti.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://xrb.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://wlr.chenzaomai.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://awq.ivvv.top

[U115] JS：生成 UUID
来源：http://yye.tarul.cn

crypto.randomUUID()
来源：http://qrt.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://wzs.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://fsc.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://her.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://ply.yangfankeji.com

[U118] JS：开发服务器
来源：http://bjv.xziqi.cn

npm i -D vite;  npx vite
来源：http://zwp.haohaochexian.top

[U119] JS：生产构建
来源：http://obe.hysaishi.cn

npx vite build
来源：http://fvb.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://mgo.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://esn.nanxuanxn.top

================================================================================
来源：http://rwc.yongpay.top

统计汇总
来源：http://ypf.316326.xyz

================================================================================
来源：http://itf.jinghuilouyu.cn

按语言统计（条）：
来源：http://ikg.pycfn.com

Python ......... 252
来源：http://xru.zhengqikj.top

PHP ............ 252
来源：http://puu.hesvh.cn

JavaScript ..... 252
来源：http://enp.sysykeji.top

TypeScript ..... 212
来源：http://fei.xuanzx.com

Java ........... 212
来源：http://mze.uphjek.com

Go ............. 212
来源：http://tct.ydjk.org.cn

Ruby ........... 212
来源：http://wuu.zhoulong.xyz

C# ............. 212
来源：http://wkf.tarul.cn

C .............. 30
来源：http://ypo.ivvv.top

C++ ............ 30
来源：http://lou.zhengqikj.top

SQL ............ 90
来源：http://fwh.ivvv.top

Bash ........... 80
来源：http://fdl.tarul.cn

Kotlin ......... 15
来源：http://ejm.zdqjudy.top

Swift .......... 15
来源：http://uua.tanke756.top

Lua ............ 10
来源：http://ppt.kuanghao11.cn

Perl ........... 10
来源：http://vij.316326.xyz

Scala .......... 10
来源：http://qwm.shzxlz.cn

------------------------------------
来源：http://gzm.jyoumei.cn

合计 ........... 2106 条
来源：http://bqi.zhixingplan.top

按章节统计：
来源：http://qai.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ldr.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zjo.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iaj.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dmj.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iup.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kgq.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rry.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://meh.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rxz.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://byz.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ssl.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hbd.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lcy.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://obi.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xhf.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eho.snrcjt.cn

Q SQL 专题                              90
来源：http://mhh.haohaochexian.top

R Bash 专题                             80
来源：http://yss.yj20258888.top

S C / C++ 专题                          60
来源：http://onh.yueranfly.top

T 其他语言补充                          60
来源：http://hns.zhijiandao.cn

U 高频实用片段                         120
来源：http://drl.pengpengdd.cyou

------------------------------------
来源：http://bjk.yuanzhike.top

合计                                  2106 条
来源：http://zwz.cheryme.top

--------------------------------------------------------------------------------
来源：http://epi.0kj1m.cn

使用提醒
来源：http://qqd.tarul.cn

--------------------------------------------------------------------------------
来源：http://ava.chenlongwang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ynv.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wgb.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vcw.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hzr.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jkx.shanyushiyangtech.top

—— 文件结束 ——
来源：http://wcj.dianchejie.cn

================================================================================
来源：http://fna.pengpengdd.cyou

程序语言常见例子速查手册（2024 版）
来源：http://xzu.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://pcv.epnwcf.com

================================================================================
来源：http://fsj.sjlbkw.cn

【收录内容】
来源：http://zai.zycfv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nvx.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rda.zhengqikj.top

SQL · Bash · C · C++
来源：http://ofi.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qdy.zhijiandao.cn

【使用说明】
来源：http://myk.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ncs.c1oappe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jss.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://joe.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fbs.zhengqikj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://add.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://odu.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mfw.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://inx.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lrl.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qxx.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sjq.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nxg.jinghuilouyu.cn

【文件统计】
来源：http://gon.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://haf.fengsongda.top

--------------------------------------------------------------------------------
来源：http://xgl.hesvh.cn

目  录
来源：http://pzo.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://zww.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://okb.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rtf.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dph.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nob.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qim.kuanghao11.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sxk.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://akp.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jvu.zhixingplan.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zlo.fktsv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dzl.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qde.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wce.tianlin.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yfw.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ruf.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hzs.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iav.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://euu.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lbb.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ddl.zhoulong.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://omh.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kov.jqgfzy.top

================================================================================
来源：http://zss.jinqigfzy.top

A. 基础语法与类型
来源：http://frl.shanyushiyangtech.top

================================================================================
来源：http://yvo.zhixingplan.top

[A01] Hello World
来源：http://qfu.jyoumei.cn

Py:   print("Hello, World!")
来源：http://hsx.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://eda.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://mao.gaohongyu789.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nzk.0kj1m.cn

Java: System.out.println("Hello, World!");
来源：http://iva.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://lvg.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://dwc.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jle.zhaomingkeji.xyz

[A02] 变量声明与赋值
来源：http://uzi.9152youxi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lzz.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jtn.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tcg.vqdsnc.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ouk.jinqigfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://trv.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://koi.yj202588.top

Ruby: name = "Alex"; age = 20
来源：http://mzl.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://nuy.feifeiyinyue.top

[A03] 常量定义
来源：http://lan.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ovr.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://hhv.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://ozq.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://wys.hammf.cn

Java: static final double PI = 3.14159;
来源：http://ypo.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://hmy.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://qis.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://klv.shuidangran.top

[A04] 判断变量类型
来源：http://zfa.vqdsnc.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cmc.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://syp.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jiz.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://vjm.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dgt.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hfk.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://van.jqgufenzy.top

C#:   x.GetType().Name; x is int
来源：http://epb.xuanzx.com

[A05] 整数除法与取模
来源：http://gvv.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ccb.havefunace.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jrw.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fyh.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://urp.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://iic.hnxiangtu.top

Go:   7 / 2; 7 % 2
来源：http://rhs.tian-w.cn

Ruby: 7 / 2; 7 % 2
来源：http://axf.nanxuanxn.top

C#:   7 / 2; 7 % 2
来源：http://ojm.xuetiantiany.cn

[A06] 字符串转数字
来源：http://iex.fzhhl.top

Py:   int("42"); float("3.14")
来源：http://jdg.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mlm.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cnx.ydzc1.top

TS:   parseInt("42", 10); Number("42")
来源：http://czd.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://znu.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bjy.daxiang520.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tnj.zhixingplan.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qeg.epnwcf.com

[A07] 数字转字符串
来源：http://yft.yanxiufei.cn

Py:   str(42)
来源：http://uhz.havefunace.top

PHP:  (string) 42; strval(42)
来源：http://dxf.havefunace.top

JS:   String(42); (42).toString()
来源：http://kev.jyoumei.cn

TS:   String(42)
来源：http://ujb.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://phw.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://gwh.haohaochexian.top


<!-- 参考信息 -->