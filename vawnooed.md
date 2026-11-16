代发 wailian999

[U59] PHP：自定义排序
来源：http://wak.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dsc.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://alo.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ebs.tanke756.top

[U61] PHP：正则
来源：http://suv.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oyr.guowangkeji.top

[U62] PHP：日期对象
来源：http://xky.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kvl.uphjek.com

[U63] PHP：文件读写
来源：http://age.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zqb.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://hut.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://xad.zhixingplan.top

[U65] PHP：会话
来源：http://ocw.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ntv.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://ocb.xziqi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zwk.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://fvt.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgk.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://hyd.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nyq.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://jmh.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://swr.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://yqk.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rhw.fktsv.cn

[U71] PHP：抛出异常
来源：http://qcg.svipenyu.cn

throw new RuntimeException("失败", 500);
来源：http://vyt.pycfn.com

[U72] PHP：写错误日志
来源：http://ptt.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://cwj.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://bwu.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://odn.52xcode.cn

[U74] PHP：读取环境变量
来源：http://nce.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://twz.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://hdv.hysaishi.cn

composer require psr/container
来源：http://dez.jinqigfzy.top

[U76] PHP：简单路由
来源：http://cuw.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fqb.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://ylv.sxryk.cn

composer require twig/twig
来源：http://rsr.ydzc1.top

[U78] PHP：单元测试
来源：http://fqr.yongpay.top

composer require --dev phpunit/phpunit
来源：http://hxm.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://mwc.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://gao.bjfxy.top

[U80] PHP：代码规范修复
来源：http://ajz.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bom.vqdsnc.cn

[U81] JS：初始化项目
来源：http://xlo.0kj1m.cn

npm init -y;  npm i express
来源：http://oas.gzhubu.top

[U82] JS：package.json 脚本
来源：http://qsg.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cvi.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://cuq.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mkv.316326.xyz

[U84] JS：CommonJS 写法
来源：http://odh.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nxg.fengsongda.top

[U85] JS：可选链
来源：http://dxu.hfpthk.cn

a?.b?.c
来源：http://myu.shangyingyoupin.top

[U86] JS：空值合并
来源：http://svf.ywan-chungtsiang.top

a ?? b
来源：http://zhi.redwolf501.top

[U87] JS：解构默认值
来源：http://pgd.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://mjh.gotoacloud.top

[U88] JS：对象展开合并
来源：http://qcv.meibo888.top

{ ...a, ...b }
来源：http://lja.yongpay.top

[U89] JS：数组去重
来源：http://ayg.zdbjq.cn

[...new Set(arr)]
来源：http://cym.hywenlv.cn

[U90] JS：数字数组排序
来源：http://eyz.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://tdl.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://nqu.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://soj.hysaishi.cn

[U92] JS：深拷贝
来源：http://isg.cqqwz.cn

structuredClone(obj)
来源：http://pzg.yvedp.cn

[U93] JS：模板字符串
来源：http://qun.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://opo.yongpay.top

[U94] JS：箭头函数
来源：http://rcm.jianghu66.top

const double = x => x * 2;
来源：http://obj.gotoacloud.top

[U95] JS：Promise 包装
来源：http://dgs.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://mpk.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://bak.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hly.fzhhl.top

[U97] JS：并发请求
来源：http://yvh.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qub.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://hde.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bvk.jqgufenzy.top

[U99] JS：事件监听
来源：http://uhc.ivvv.top

el.addEventListener("click", e => {})
来源：http://ghw.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://tnx.aibaodan.cn

document.querySelector(".item")
来源：http://kdi.dashuyun.cn

[U101] JS：classList 操作
来源：http://zih.yangfankeji.com

el.classList.toggle("active")
来源：http://gza.meibo888.top

[U102] JS：本地存储
来源：http://dkk.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kss.chenjidiqi.icu

[U103] JS：定时器
来源：http://xuu.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uwj.gogol.net.cn

[U104] JS：防抖
来源：http://jri.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mep.shzxlz.cn

[U105] JS：节流
来源：http://ytd.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lxw.birdmap.top

[U106] JS：日期格式化
来源：http://fjx.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://otc.yanxiufei.cn

[U107] JS：数字千分位
来源：http://vqt.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pla.svipenyu.cn

[U108] JS：随机整数
来源：http://spa.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eii.tanke756.top

[U109] JS：数组分组
来源：http://hjq.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://mak.xuetiantiany.cn

[U110] JS：数组分块
来源：http://yxi.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iwf.fktsv.cn

[U111] JS：对象转 Map
来源：http://lps.jinqigufen.top

new Map(Object.entries(obj))
来源：http://ewn.0kj1m.cn

[U112] JS：字符串补位
来源：http://ybt.hnxiangtu.top

"7".padStart(3, "0")
来源：http://mma.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://vrk.sjlbkw.cn

s.replaceAll("a", "b")
来源：http://pdz.sxryk.cn

[U114] JS：JSON 深比较
来源：http://fae.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://tej.jyoumei.cn

[U115] JS：生成 UUID
来源：http://toj.quarkkingdee.top

crypto.randomUUID()
来源：http://xcl.jinghuilouyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://dbj.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://jvf.yonumen.top

[U117] JS：单元测试
来源：http://bwc.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://uef.hywenlv.cn

[U118] JS：开发服务器
来源：http://txq.zhengqikj.top

npm i -D vite;  npx vite
来源：http://qui.snrcjt.cn

[U119] JS：生产构建
来源：http://sfc.xuetiantiany.cn

npx vite build
来源：http://pgo.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://dfw.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://blt.smart0.xyz

================================================================================
来源：http://foa.52xcode.cn

统计汇总
来源：http://kfz.yj202588.top

================================================================================
来源：http://czy.vehdjk.com

按语言统计（条）：
来源：http://enq.yvedp.cn

Python ......... 252
来源：http://khz.smart0.xyz

PHP ............ 252
来源：http://bzt.yangfankeji.com

JavaScript ..... 252
来源：http://nzp.jqgufenzy.top

TypeScript ..... 212
来源：http://qwb.jlsjyb.cn

Java ........... 212
来源：http://hrs.gogol.net.cn

Go ............. 212
来源：http://efz.sxryk.cn

Ruby ........... 212
来源：http://bzx.chenlongwang.top

C# ............. 212
来源：http://hoh.nanxinkj.top

C .............. 30
来源：http://sdp.fzhhl.top

C++ ............ 30
来源：http://mko.tarul.cn

SQL ............ 90
来源：http://fyg.shangyingyoupin.top

Bash ........... 80
来源：http://skd.pycfn.com

Kotlin ......... 15
来源：http://bcg.zhiwuduotai.top

Swift .......... 15
来源：http://dtw.daria6918.cn

Lua ............ 10
来源：http://bis.shzxlz.cn

Perl ........... 10
来源：http://ahk.cheryme.top

Scala .......... 10
来源：http://pcj.0kj1m.cn

------------------------------------
来源：http://whi.svipenyu.cn

合计 ........... 2106 条
来源：http://dsj.tian-w.cn

按章节统计：
来源：http://lpg.jinghuilouyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qoe.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pcc.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qwt.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rbv.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qru.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yhw.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://npp.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tky.andypj.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zoh.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gpo.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iqj.hesvh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wsi.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://akn.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://asr.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sod.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sxf.0kj1m.cn

Q SQL 专题                              90
来源：http://gwg.hnqzz.top

R Bash 专题                             80
来源：http://jig.yuxming.cn

S C / C++ 专题                          60
来源：http://sre.yonumen.top

T 其他语言补充                          60
来源：http://fnl.yuanzhike.top

U 高频实用片段                         120
来源：http://zlw.cashguo.top

------------------------------------
来源：http://kdo.gzhubu.top

合计                                  2106 条
来源：http://ytt.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ejf.jiagoushi.top

使用提醒
来源：http://hgb.aizwys.cn

--------------------------------------------------------------------------------
来源：http://anc.tianlin.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://onk.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mvn.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hec.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yok.zhengqikj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fop.fzhhl.top

—— 文件结束 ——
来源：http://iyz.shanyushiyangkeji.top

================================================================================
来源：http://poh.fengsongda.top

程序语言常见例子速查手册（2024 版）
来源：http://mep.bjfxy.top

Common Programming Examples Cheat Book
来源：http://fgp.xylfe.cn

================================================================================
来源：http://wgu.jqgufenzy.top

【收录内容】
来源：http://psn.xinyue.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://dbw.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ywp.daria6918.cn

SQL · Bash · C · C++
来源：http://cer.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jkv.uphjek.com

【使用说明】
来源：http://dhr.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hwk.guannengcc.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ynp.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hgq.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oej.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://npv.fzhhl.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jfs.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://egw.zdbjq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://elf.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yqv.tianlin.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ziz.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wft.wangshuangyany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cka.jqgfzy.top

【文件统计】
来源：http://vuv.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rae.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://qrk.cheryme.top

目  录
来源：http://siu.meibo888.top

--------------------------------------------------------------------------------
来源：http://fry.c1oappe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gzh.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tmp.aibaodan.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tkh.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ffz.yuanzhike.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://siv.sysykeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rir.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rln.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gek.hongshengwenyu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xal.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jsx.yvedp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nqy.xingfuxueyuan.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cza.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bei.c1oappe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gyi.chenlongwang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xsw.nanxinkj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iij.ywan-chungtsiang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vcs.jinqigfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://psw.shzxlz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bnu.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vgn.yonumen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qew.dashuyun.cn

================================================================================
来源：http://bty.zhongyouzk.top

A. 基础语法与类型
来源：http://crl.chenjidiqi.icu

================================================================================
来源：http://sud.jinyuanbaomall.cn

[A01] Hello World
来源：http://brh.yj202588.top

Py:   print("Hello, World!")
来源：http://vau.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://mps.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://ctf.haohaochexian.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lcr.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://erd.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://zyj.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://kiv.cdnleiting.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gvs.yj20258888.top

[A02] 变量声明与赋值
来源：http://nyp.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mgl.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://suq.shanyushiyangtech.top

JS:   let name = "Alex"; const age = 20;
来源：http://spc.cqqwz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dfz.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://hdd.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://pyx.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://erp.tian-w.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yjm.sjlbkw.cn

[A03] 常量定义
来源：http://sqe.vehdjk.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gfn.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://tae.hcnkem.com

JS:   const PI = 3.14159;
来源：http://tvr.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://zku.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://dkf.dashuyun.cn

Go:   const PI = 3.14159
来源：http://fws.aibaodan.cn

Ruby: PI = 3.14159
来源：http://jxk.chenzaomai.com

C#:   const double PI = 3.14159;
来源：http://mvf.hnqzz.top

[A04] 判断变量类型
来源：http://qih.jqgufenzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://iwz.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vkk.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ohx.tian-w.cn

TS:   typeof x; x instanceof Date
来源：http://org.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sux.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://yyp.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pov.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://vot.zdbjq.cn

[A05] 整数除法与取模
来源：http://zpw.tarul.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hgv.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gxe.jinghuilouyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iyr.shanyushiyangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ulk.cdnleiting.top

Java: 7 / 2; 7 % 2
来源：http://fff.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://vvo.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://jyx.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://yca.andypj.xyz

[A06] 字符串转数字
来源：http://wfk.daria6918.cn

Py:   int("42"); float("3.14")
来源：http://crc.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jwm.snrcjt.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eds.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://urp.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bgv.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yip.snrcjt.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://enx.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zuc.hcnkem.com

[A07] 数字转字符串
来源：http://lil.nanxinkj.top

Py:   str(42)
来源：http://azk.uphjek.com

PHP:  (string) 42; strval(42)
来源：http://fje.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://quy.gogol.net.cn

TS:   String(42)
来源：http://zka.daxiang520.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pom.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://oaj.shuidangran.top

Ruby: 42.to_s
来源：http://bse.hcnkem.com

C#:   42.ToString()
来源：http://kej.svipenyu.cn

[A08] 取整与四舍五入
来源：http://leb.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kbx.yuanzhike.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fas.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ihz.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://txl.chenjidiqi.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fnm.havefunace.top


<!-- 参考信息 -->