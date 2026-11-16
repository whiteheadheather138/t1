代发 wailian999

[U53] PHP：空合并运算符
来源：http://cbs.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://owy.zdqjudy.top

[U54] PHP：空安全调用
来源：http://xyj.shanyushiyangtech.top

$obj?->method()
来源：http://vfv.cheryme.top

[U55] PHP：match 表达式
来源：http://eiu.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tuy.xylfe.cn

[U56] PHP：命名参数
来源：http://zlt.hcnkem.com

f(a: 1, b: 2)
来源：http://cel.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://qka.meibo888.top

"值: {$a}"
来源：http://vat.sufxvd.cn

[U58] PHP：数组三件套
来源：http://tow.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rpe.bbcook.cn

[U59] PHP：自定义排序
来源：http://fgs.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bla.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://cqv.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ain.yfazqb.com

[U61] PHP：正则
来源：http://erf.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rux.aizwys.cn

[U62] PHP：日期对象
来源：http://ocx.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ibg.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://zhe.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zll.jinqigufen.top

[U64] PHP：目录遍历
来源：http://tbs.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://coq.gotoacloud.top

[U65] PHP：会话
来源：http://klv.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tnf.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://dfa.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rhl.xylfe.cn

[U67] PHP：处理文件上传
来源：http://ooh.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vuu.cashguo.top

[U68] PHP：PDO 连接
来源：http://nzf.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qin.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://kos.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lis.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://dfo.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://syt.shuidangran.top

[U71] PHP：抛出异常
来源：http://qxo.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://bqk.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://eqx.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://uzf.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://cse.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://xex.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://fke.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://ovi.cheryme.top

[U75] PHP：依赖注入
来源：http://uxo.chenjidiqi.icu

composer require psr/container
来源：http://fzb.zhoulong.xyz

[U76] PHP：简单路由
来源：http://tjk.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kvf.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://cgx.nanxinkj.top

composer require twig/twig
来源：http://daq.yuanzhike.top

[U78] PHP：单元测试
来源：http://zia.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://trh.sysykeji.top

[U79] PHP：静态分析
来源：http://uwm.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://fvk.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://lqz.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://anl.gogol.net.cn

[U81] JS：初始化项目
来源：http://zmz.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://oqx.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://voh.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ivw.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://ugy.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://wwn.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://ect.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wez.sjlbkw.cn

[U85] JS：可选链
来源：http://gnn.yuxming.cn

a?.b?.c
来源：http://qms.hongshengwenyu.top

[U86] JS：空值合并
来源：http://clr.tanke756.top

a ?? b
来源：http://cqe.zhongyouzk.top

[U87] JS：解构默认值
来源：http://oqb.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://wov.hammf.cn

[U88] JS：对象展开合并
来源：http://rvw.nanxuanxn.top

{ ...a, ...b }
来源：http://fxd.chenjidiqi.icu

[U89] JS：数组去重
来源：http://xnh.chenjidiqi.icu

[...new Set(arr)]
来源：http://tyu.vehdjk.com

[U90] JS：数字数组排序
来源：http://hgh.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://zol.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://mbg.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://axu.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://eep.snrcjt.cn

structuredClone(obj)
来源：http://jvq.jyoumei.cn

[U93] JS：模板字符串
来源：http://kdq.gzhubu.top

`共 ${n} 条`
来源：http://jtn.zhongyouzk.top

[U94] JS：箭头函数
来源：http://psm.feifeiyinyue.top

const double = x => x * 2;
来源：http://bwu.chenlongwang.top

[U95] JS：Promise 包装
来源：http://tqp.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://mkk.redwolf501.top

[U96] JS：async/await 与异常
来源：http://lfz.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oyw.haohaochexian.top

[U97] JS：并发请求
来源：http://kll.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ozd.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://gbj.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hsb.hfpthk.cn

[U99] JS：事件监听
来源：http://sdz.yonumen.top

el.addEventListener("click", e => {})
来源：http://nbb.mhx1999.top

[U100] JS：DOM 查询
来源：http://oky.kuanghao11.cn

document.querySelector(".item")
来源：http://ima.nanxuanxn.top

[U101] JS：classList 操作
来源：http://smx.daria6918.cn

el.classList.toggle("active")
来源：http://wvu.mhx1999.top

[U102] JS：本地存储
来源：http://oat.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kfl.zdqjudy.top

[U103] JS：定时器
来源：http://ost.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ygm.svipenyu.cn

[U104] JS：防抖
来源：http://dqe.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jgh.vehdjk.com

[U105] JS：节流
来源：http://jcs.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vot.52xcode.cn

[U106] JS：日期格式化
来源：http://lww.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ejc.ydjk.org.cn

[U107] JS：数字千分位
来源：http://lmw.zhixingplan.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yht.zhixingplan.top

[U108] JS：随机整数
来源：http://xyq.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nok.pycfn.com

[U109] JS：数组分组
来源：http://gth.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://loo.feifeiyinyue.top

[U110] JS：数组分块
来源：http://etl.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://npy.vehdjk.com

[U111] JS：对象转 Map
来源：http://nvx.jianghu66.top

new Map(Object.entries(obj))
来源：http://aac.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://cbq.quarkkingdee.top

"7".padStart(3, "0")
来源：http://oal.sufxvd.cn

[U113] JS：正则替换全部
来源：http://psf.hcnkem.com

s.replaceAll("a", "b")
来源：http://rfc.hesvh.cn

[U114] JS：JSON 深比较
来源：http://nau.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wgy.sufxvd.cn

[U115] JS：生成 UUID
来源：http://qfe.yuxming.cn

crypto.randomUUID()
来源：http://vdq.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://hsv.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://ram.vehdjk.com

[U117] JS：单元测试
来源：http://zjp.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://cnm.shzxlz.cn

[U118] JS：开发服务器
来源：http://lsr.dianchejie.cn

npm i -D vite;  npx vite
来源：http://lan.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://zul.zycfv.cn

npx vite build
来源：http://bsg.wangshuangyany.cn

[U120] JS：读取环境变量（Vite）
来源：http://gzk.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://dqx.0kj1m.cn

================================================================================
来源：http://wci.hnqzz.top

统计汇总
来源：http://ijt.nanxuanxn.top

================================================================================
来源：http://pzx.yonumen.top

按语言统计（条）：
来源：http://inf.yvedp.cn

Python ......... 252
来源：http://kyl.fktsv.cn

PHP ............ 252
来源：http://zqx.mhx1999.top

JavaScript ..... 252
来源：http://tiz.cheryme.top

TypeScript ..... 212
来源：http://gqy.cucudq.cn

Java ........... 212
来源：http://sid.pengpengdd.cyou

Go ............. 212
来源：http://fsb.yfazqb.com

Ruby ........... 212
来源：http://frq.xinyue.icu

C# ............. 212
来源：http://sjg.yj202588.top

C .............. 30
来源：http://vqy.gaohongyu789.top

C++ ............ 30
来源：http://djp.daria6918.cn

SQL ............ 90
来源：http://jfk.daxiang520.top

Bash ........... 80
来源：http://xii.smart0.xyz

Kotlin ......... 15
来源：http://djw.jqgfzy.top

Swift .......... 15
来源：http://vbd.zhengqikj.top

Lua ............ 10
来源：http://bam.shanyushiyangkeji.top

Perl ........... 10
来源：http://vup.zhengqikj.top

Scala .......... 10
来源：http://evx.jiagoushi.top

------------------------------------
来源：http://wej.fktsv.cn

合计 ........... 2106 条
来源：http://fui.cdnleiting.top

按章节统计：
来源：http://iiu.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://myt.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sac.jianghu66.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uqk.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eeb.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cpz.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://htt.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nsb.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jwd.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rtl.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uth.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gsh.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fsz.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mno.hfpthk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nut.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xgl.zhengqikj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tpm.jqgfzy.top

Q SQL 专题                              90
来源：http://llh.pengpengdd.cyou

R Bash 专题                             80
来源：http://ylg.daria6918.cn

S C / C++ 专题                          60
来源：http://ckg.zhijiandao.cn

T 其他语言补充                          60
来源：http://zjt.xuetiantiany.cn

U 高频实用片段                         120
来源：http://xss.daria6918.cn

------------------------------------
来源：http://hvz.tanke756.top

合计                                  2106 条
来源：http://fpg.xziqi.cn

--------------------------------------------------------------------------------
来源：http://ufs.jiagoushi.top

使用提醒
来源：http://mkw.birdmap.top

--------------------------------------------------------------------------------
来源：http://ehe.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wtr.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zqv.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ftm.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gvj.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://els.ctjpmb.com

—— 文件结束 ——
来源：http://vvk.vqdsnc.cn

================================================================================
来源：http://dlo.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://lse.yj20258.top

Common Programming Examples Cheat Book
来源：http://svt.wangshuangyany.cn

================================================================================
来源：http://ojr.guannengcc.top

【收录内容】
来源：http://wgd.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bzy.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rfy.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://seq.zycfv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qmi.epnwcf.com

【使用说明】
来源：http://yyn.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ggm.tian-w.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://unl.hfpthk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zdk.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mzp.bbcook.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ydn.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://huv.chenjidiqi.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jci.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aiz.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nta.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zov.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gko.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ycw.sysykeji.top

【文件统计】
来源：http://mvl.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kre.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://xmb.cheryme.top

目  录
来源：http://lzx.andypj.xyz

--------------------------------------------------------------------------------
来源：http://vmn.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pjl.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wse.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aiw.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rtk.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://smt.nanxuanxn.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rnb.haohaochexian.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uyc.cashguo.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pci.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://igt.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qsj.wangdashe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pda.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jep.shangyingyoupin.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nmd.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wug.shuidangran.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dhl.smart0.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://njr.xuanzx.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://voo.ywan-chungtsiang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cxe.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ipo.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqu.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ykw.sjlbkw.cn

================================================================================
来源：http://gtl.fzhhl.top

A. 基础语法与类型
来源：http://gdd.shanyushiyangtech.top

================================================================================
来源：http://jrt.hfpthk.cn

[A01] Hello World
来源：http://bmr.meibo888.top

Py:   print("Hello, World!")
来源：http://rcv.guowangkeji.top

PHP:  echo "Hello, World!";
来源：http://uib.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://dig.cucudq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hvl.hongshengwenyu.top

Java: System.out.println("Hello, World!");
来源：http://whv.jinqigfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://qis.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://bdb.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rbv.fktsv.cn

[A02] 变量声明与赋值
来源：http://zyd.jinqigfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dmr.andypj.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ygi.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://odr.quarkkingdee.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ybs.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://kav.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://eql.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://vbn.fzhhl.top

C#:   string name = "Alex"; int age = 20;
来源：http://biv.hesvh.cn

[A03] 常量定义
来源：http://ive.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mhr.yongpay.top

PHP:  const PI = 3.14159;
来源：http://utw.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://ryn.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://anf.xuetiantiany.cn

Java: static final double PI = 3.14159;
来源：http://ppj.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://uhw.xinyue.icu

Ruby: PI = 3.14159
来源：http://dzx.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://kqe.andypj.xyz

[A04] 判断变量类型
来源：http://fnk.smart0.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://rhc.vqdsnc.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jps.yj202588.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vng.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://gif.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://igr.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://dim.bbcook.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yvy.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://suk.meibo888.top

[A05] 整数除法与取模
来源：http://nrh.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://snq.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://gnu.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://inf.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vpq.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://jsa.hywenlv.cn

Go:   7 / 2; 7 % 2
来源：http://riv.gzhubu.top

Ruby: 7 / 2; 7 % 2
来源：http://vxm.tanke756.top

C#:   7 / 2; 7 % 2
来源：http://vhv.pycfn.com

[A06] 字符串转数字
来源：http://tre.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://gcf.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://izt.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eat.smart0.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://fna.yvedp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://buy.yangfankeji.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aim.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yyu.ybcxt.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xha.tanke756.top

[A07] 数字转字符串
来源：http://ipr.chenlongwang.top

Py:   str(42)
来源：http://flb.cqqwz.cn

PHP:  (string) 42; strval(42)
来源：http://qxl.yfazqb.com


<!-- 参考信息 -->