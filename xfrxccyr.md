代发 wailian999

[U53] PHP：空合并运算符
来源：http://heg.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://wii.zdqjudy.top

[U54] PHP：空安全调用
来源：http://akg.jinqigfzy.top

$obj?->method()
来源：http://xtx.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://vlv.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dtj.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://uki.kuanghao11.cn

f(a: 1, b: 2)
来源：http://fcd.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://ziz.haohaochexian.top

"值: {$a}"
来源：http://nik.haohaochexian.top

[U58] PHP：数组三件套
来源：http://tif.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lmd.cucudq.cn

[U59] PHP：自定义排序
来源：http://zps.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pzp.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://tfg.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ksv.fanxiaobao.xyz

[U61] PHP：正则
来源：http://dhg.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zhf.uphjek.com

[U62] PHP：日期对象
来源：http://xgs.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cia.cqqwz.cn

[U63] PHP：文件读写
来源：http://www.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qsv.aibaodan.cn

[U64] PHP：目录遍历
来源：http://dck.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://ptc.fktsv.cn

[U65] PHP：会话
来源：http://zjg.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yyz.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://owl.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lqx.yj20258888.top

[U67] PHP：处理文件上传
来源：http://lpe.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rkg.zhengqikj.top

[U68] PHP：PDO 连接
来源：http://kav.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://poa.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://cfp.shzxlz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hrh.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://flj.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fxo.xziqi.cn

[U71] PHP：抛出异常
来源：http://ydn.316326.xyz

throw new RuntimeException("失败", 500);
来源：http://zpt.c1oappe.top

[U72] PHP：写错误日志
来源：http://giz.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://crp.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://kpd.xylfe.cn

parse_ini_file("config.ini", true)
来源：http://vre.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://vmx.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://kbv.316326.xyz

[U75] PHP：依赖注入
来源：http://qdl.yuxming.cn

composer require psr/container
来源：http://jxb.zdqjudy.top

[U76] PHP：简单路由
来源：http://hsp.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zpn.snrcjt.cn

[U77] PHP：模板渲染
来源：http://kvw.uphjek.com

composer require twig/twig
来源：http://iuc.52xcode.cn

[U78] PHP：单元测试
来源：http://zhb.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://drl.ydzc1.top

[U79] PHP：静态分析
来源：http://ibl.yj20258.top

composer require --dev phpstan/phpstan
来源：http://izi.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://qas.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rzf.tianlin.xyz

[U81] JS：初始化项目
来源：http://dhb.gotoacloud.top

npm init -y;  npm i express
来源：http://opp.pengpengdd.cyou

[U82] JS：package.json 脚本
来源：http://gdm.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zna.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://mtq.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://etv.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://glb.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://bcy.andypj.xyz

[U85] JS：可选链
来源：http://idb.jqgufenzy.top

a?.b?.c
来源：http://kyi.shuidangran.top

[U86] JS：空值合并
来源：http://vyr.epnwcf.com

a ?? b
来源：http://juf.hfpthk.cn

[U87] JS：解构默认值
来源：http://xey.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://wrm.guannengcc.top

[U88] JS：对象展开合并
来源：http://qys.wangdashe.top

{ ...a, ...b }
来源：http://ior.kuanghao11.cn

[U89] JS：数组去重
来源：http://bxt.ydjk.org.cn

[...new Set(arr)]
来源：http://yfj.cdnleiting.top

[U90] JS：数字数组排序
来源：http://nnw.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://mfk.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://ljq.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jdy.yj202588.top

[U92] JS：深拷贝
来源：http://put.ppjwa.cn

structuredClone(obj)
来源：http://xtu.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://yhz.cheryme.top

`共 ${n} 条`
来源：http://ito.zycfv.cn

[U94] JS：箭头函数
来源：http://nsf.zycfv.cn

const double = x => x * 2;
来源：http://hop.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://fji.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://lbe.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://ibd.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nqa.cheryme.top

[U97] JS：并发请求
来源：http://rrs.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jlk.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://wwk.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fwc.epnwcf.com

[U99] JS：事件监听
来源：http://fzg.fzhhl.top

el.addEventListener("click", e => {})
来源：http://fpz.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://pbj.gaohongyu789.top

document.querySelector(".item")
来源：http://bmq.havefunace.top

[U101] JS：classList 操作
来源：http://buh.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://oke.vehdjk.com

[U102] JS：本地存储
来源：http://pxi.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bmz.gaohongyu789.top

[U103] JS：定时器
来源：http://vjw.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ewe.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://gbh.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zce.quarkkingdee.top

[U105] JS：节流
来源：http://gyq.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eei.andypj.xyz

[U106] JS：日期格式化
来源：http://fna.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kit.haohaochexian.top

[U107] JS：数字千分位
来源：http://hkh.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nwd.tian-w.cn

[U108] JS：随机整数
来源：http://umw.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vdf.sjlbkw.cn

[U109] JS：数组分组
来源：http://hau.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://het.ctjpmb.com

[U110] JS：数组分块
来源：http://mln.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ygj.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://hwz.c1oappe.top

new Map(Object.entries(obj))
来源：http://jth.xinyue.icu

[U112] JS：字符串补位
来源：http://hqa.zhongyouzk.top

"7".padStart(3, "0")
来源：http://igj.zhengqikj.top

[U113] JS：正则替换全部
来源：http://pwt.bjfxy.top

s.replaceAll("a", "b")
来源：http://ryy.yj202588.top

[U114] JS：JSON 深比较
来源：http://mby.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://osl.nanxinkj.top

[U115] JS：生成 UUID
来源：http://gbc.jqgufenzy.top

crypto.randomUUID()
来源：http://gur.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://faz.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://hqz.svipenyu.cn

[U117] JS：单元测试
来源：http://xlp.pycfn.com

npm i -D vitest;  npx vitest
来源：http://lvw.yongpay.top

[U118] JS：开发服务器
来源：http://jbt.tianlin.xyz

npm i -D vite;  npx vite
来源：http://swn.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://dsi.sxryk.cn

npx vite build
来源：http://urs.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://uzu.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://uwx.dashuyun.cn

================================================================================
来源：http://uxv.xuanzx.com

统计汇总
来源：http://pos.zycfv.cn

================================================================================
来源：http://dxx.shangyingyoupin.top

按语言统计（条）：
来源：http://ejq.zdqjudy.top

Python ......... 252
来源：http://vrn.xingfuxueyuan.xyz

PHP ............ 252
来源：http://nmj.gaohongyu789.top

JavaScript ..... 252
来源：http://mii.zhiwuduotai.top

TypeScript ..... 212
来源：http://mgo.jlsjyb.cn

Java ........... 212
来源：http://sbp.zhaomingkeji.xyz

Go ............. 212
来源：http://gnv.aibaodan.cn

Ruby ........... 212
来源：http://ezh.jianghu66.top

C# ............. 212
来源：http://aur.aibaodan.cn

C .............. 30
来源：http://bqt.haohaochexian.top

C++ ............ 30
来源：http://zxg.wangdashe.top

SQL ............ 90
来源：http://owx.ctjpmb.com

Bash ........... 80
来源：http://jte.shzxlz.cn

Kotlin ......... 15
来源：http://uhu.pycfn.com

Swift .......... 15
来源：http://uky.bjfxy.top

Lua ............ 10
来源：http://xto.gogol.net.cn

Perl ........... 10
来源：http://cmz.0kj1m.cn

Scala .......... 10
来源：http://dit.sufxvd.cn

------------------------------------
来源：http://tpf.meibo888.top

合计 ........... 2106 条
来源：http://vpa.yuanzhike.top

按章节统计：
来源：http://fsb.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dpu.bbcook.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vfa.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fvo.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ciu.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dmf.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mgu.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gwn.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://guq.zhengqikj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kas.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lpz.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ybj.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sbo.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rog.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mos.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ueh.guannengcc.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rac.sweek.top

Q SQL 专题                              90
来源：http://qmy.zhengqikj.top

R Bash 专题                             80
来源：http://kfy.hysaishi.cn

S C / C++ 专题                          60
来源：http://aaa.pengpengdd.cyou

T 其他语言补充                          60
来源：http://fmk.bbcook.cn

U 高频实用片段                         120
来源：http://wlo.xziqi.cn

------------------------------------
来源：http://hro.jlsjyb.cn

合计                                  2106 条
来源：http://iwd.sysykeji.top

--------------------------------------------------------------------------------
来源：http://zmr.cashguo.top

使用提醒
来源：http://kah.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://ejm.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hxw.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bgv.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fgy.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://puh.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yxh.hnqzz.top

—— 文件结束 ——
来源：http://cgd.gogol.net.cn

================================================================================
来源：http://pfj.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://qrj.tarul.cn

Common Programming Examples Cheat Book
来源：http://bqw.bjfxy.top

================================================================================
来源：http://ylk.yongpay.top

【收录内容】
来源：http://pue.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://cwa.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pjz.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://riy.yj20258888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vlb.fanxiaobao.xyz

【使用说明】
来源：http://hzr.shanyushiyangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lci.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mlk.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xuh.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://klf.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://pos.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xky.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tmv.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uwz.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xng.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tyl.svipenyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rix.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xlp.sufxvd.cn

【文件统计】
来源：http://qjd.cdnleiting.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ojb.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://rdk.52xcode.cn

目  录
来源：http://rjs.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://uyf.yvedp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yue.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hzg.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://urt.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hve.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pgr.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xwf.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oxr.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rii.shanyushiyangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vmo.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eea.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bvt.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dra.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iiv.meibo888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cqy.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jzz.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qxr.hesvh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oqn.yongpay.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wil.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bhd.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cbe.dashuyun.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ose.52xcode.cn

================================================================================
来源：http://xrk.zycfv.cn

A. 基础语法与类型
来源：http://vvl.iojbl.cn

================================================================================
来源：http://oxj.nanxuanxn.top

[A01] Hello World
来源：http://vil.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://dmq.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://sfg.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://uen.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ieq.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://xdn.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://fgs.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://acx.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vrs.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://egx.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ank.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ojj.aibaodan.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nda.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bfw.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://hab.shuidangran.top

Go:   name := "Alex"; age := 20
来源：http://vyn.cashguo.top

Ruby: name = "Alex"; age = 20
来源：http://lxu.epnwcf.com

C#:   string name = "Alex"; int age = 20;
来源：http://kzm.svipenyu.cn

[A03] 常量定义
来源：http://uoi.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oeh.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://xet.shanyushiyangkeji.top

JS:   const PI = 3.14159;
来源：http://dfp.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://fhu.yvedp.cn

Java: static final double PI = 3.14159;
来源：http://yxh.ydzc1.top

Go:   const PI = 3.14159
来源：http://bzt.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://mgk.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://fgi.c1oappe.top

[A04] 判断变量类型
来源：http://fjy.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ows.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hqu.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rmb.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://tui.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xym.snrcjt.cn

Go:   reflect.TypeOf(x).Name()
来源：http://axp.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xrs.zdbjq.cn

C#:   x.GetType().Name; x is int
来源：http://zfq.gzhubu.top

[A05] 整数除法与取模
来源：http://jnl.fehbvm.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wib.shuidangran.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rvt.zhixingplan.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zqj.tanke756.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ktx.sufxvd.cn

Java: 7 / 2; 7 % 2
来源：http://loo.ehwqpu.com

Go:   7 / 2; 7 % 2
来源：http://gos.yuxming.cn

Ruby: 7 / 2; 7 % 2
来源：http://vdf.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://rov.hcnkem.com

[A06] 字符串转数字
来源：http://pyr.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://usj.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gap.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pwi.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nme.jinqigfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fde.vehdjk.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ujy.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gtl.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tmc.yfazqb.com

[A07] 数字转字符串
来源：http://dpq.yuxming.cn

Py:   str(42)
来源：http://tii.tanke756.top

PHP:  (string) 42; strval(42)
来源：http://cij.haohaochexian.top


<!-- 参考信息 -->