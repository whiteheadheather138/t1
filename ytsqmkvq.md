代发 wailian999

[U53] PHP：空合并运算符
来源：http://xil.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://ibk.xziqi.cn

[U54] PHP：空安全调用
来源：http://zgu.pycfn.com

$obj?->method()
来源：http://rfn.sufxvd.cn

[U55] PHP：match 表达式
来源：http://dkr.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jco.yonumen.top

[U56] PHP：命名参数
来源：http://dng.yj202588.top

f(a: 1, b: 2)
来源：http://mbq.svipenyu.cn

[U57] PHP：字符串插值
来源：http://xwt.chenjidiqi.icu

"值: {$a}"
来源：http://efr.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://uzd.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ixe.yongpay.top

[U59] PHP：自定义排序
来源：http://fia.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pij.cashguo.top

[U60] PHP：JSON 编解码
来源：http://afd.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cby.hongshengwenyu.top

[U61] PHP：正则
来源：http://qmc.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cit.zycfv.cn

[U62] PHP：日期对象
来源：http://luw.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zna.bjfxy.top

[U63] PHP：文件读写
来源：http://yck.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mer.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://uyq.tanke756.top

glob("dir/*.php");  scandir("dir");
来源：http://oje.smart0.xyz

[U65] PHP：会话
来源：http://gor.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ejl.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://fxw.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sgz.havefunace.top

[U67] PHP：处理文件上传
来源：http://fbs.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dts.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://fpl.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dpr.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://psp.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lpi.sweek.top

[U70] PHP：PDO 事务
来源：http://bof.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jzc.shzxlz.cn

[U71] PHP：抛出异常
来源：http://its.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://mer.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://nba.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://bvd.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://nix.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://miu.sysykeji.top

[U74] PHP：读取环境变量
来源：http://xvk.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://xkw.svipenyu.cn

[U75] PHP：依赖注入
来源：http://ukp.jiagoushi.top

composer require psr/container
来源：http://nfo.fzhhl.top

[U76] PHP：简单路由
来源：http://tsr.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yss.hesvh.cn

[U77] PHP：模板渲染
来源：http://yvk.tian-w.cn

composer require twig/twig
来源：http://npo.ctjpmb.com

[U78] PHP：单元测试
来源：http://xul.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://nne.nwbrower.top

[U79] PHP：静态分析
来源：http://yqc.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://sdk.ivvv.top

[U80] PHP：代码规范修复
来源：http://pnq.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tln.yj20258.top

[U81] JS：初始化项目
来源：http://bek.sjlbkw.cn

npm init -y;  npm i express
来源：http://vix.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://hwd.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ids.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://fqj.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://afi.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://jmq.ydzc1.top

module.exports = { a };  const { a } = require("./m");
来源：http://jjc.cucudq.cn

[U85] JS：可选链
来源：http://pmb.yvedp.cn

a?.b?.c
来源：http://xgd.fengsongda.top

[U86] JS：空值合并
来源：http://kiz.quarkkingdee.top

a ?? b
来源：http://cyz.gaohongyu789.top

[U87] JS：解构默认值
来源：http://ixn.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://ijj.tarul.cn

[U88] JS：对象展开合并
来源：http://hsv.zhixingplan.top

{ ...a, ...b }
来源：http://qwf.ctjpmb.com

[U89] JS：数组去重
来源：http://jxk.xziqi.cn

[...new Set(arr)]
来源：http://knf.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://ruf.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://lnj.yj202588.top

[U91] JS：对象键值遍历
来源：http://fpj.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tnd.zdqjudy.top

[U92] JS：深拷贝
来源：http://xsz.shangyingyoupin.top

structuredClone(obj)
来源：http://bzs.hysaishi.cn

[U93] JS：模板字符串
来源：http://utq.daxiang520.top

`共 ${n} 条`
来源：http://hdj.shzxlz.cn

[U94] JS：箭头函数
来源：http://jra.redwolf501.top

const double = x => x * 2;
来源：http://vpd.0kj1m.cn

[U95] JS：Promise 包装
来源：http://cfj.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://bas.yongpay.top

[U96] JS：async/await 与异常
来源：http://znv.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://shf.fehbvm.com

[U97] JS：并发请求
来源：http://nls.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wwq.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://khu.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ydu.yangfankeji.com

[U99] JS：事件监听
来源：http://qsm.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://tgx.svipenyu.cn

[U100] JS：DOM 查询
来源：http://onz.fzhhl.top

document.querySelector(".item")
来源：http://mka.tarul.cn

[U101] JS：classList 操作
来源：http://pmq.hammf.cn

el.classList.toggle("active")
来源：http://zgc.hcnkem.com

[U102] JS：本地存储
来源：http://hbn.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://shw.haohaochexian.top

[U103] JS：定时器
来源：http://fpi.shanyushiyangtech.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gda.zdbjq.cn

[U104] JS：防抖
来源：http://kgv.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewr.ywan-chungtsiang.top

[U105] JS：节流
来源：http://tow.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tbi.kuanghao11.cn

[U106] JS：日期格式化
来源：http://qpd.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jgk.vehdjk.com

[U107] JS：数字千分位
来源：http://rso.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xyd.aizwys.cn

[U108] JS：随机整数
来源：http://usj.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qss.epnwcf.com

[U109] JS：数组分组
来源：http://iky.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://uzh.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://uqz.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fnp.vehdjk.com

[U111] JS：对象转 Map
来源：http://hbj.hammf.cn

new Map(Object.entries(obj))
来源：http://hiu.smart0.xyz

[U112] JS：字符串补位
来源：http://mpa.haohaochexian.top

"7".padStart(3, "0")
来源：http://nsz.gogol.net.cn

[U113] JS：正则替换全部
来源：http://kiv.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://weq.birdmap.top

[U114] JS：JSON 深比较
来源：http://pgt.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bjh.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://vbm.bbcook.cn

crypto.randomUUID()
来源：http://njq.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://pgt.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://uus.bjfxy.top

[U117] JS：单元测试
来源：http://icf.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://tqz.cheryme.top

[U118] JS：开发服务器
来源：http://nab.ybcxt.top

npm i -D vite;  npx vite
来源：http://ebg.shangyingyoupin.top

[U119] JS：生产构建
来源：http://krn.jianghu66.top

npx vite build
来源：http://aut.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://rxy.uphjek.com

import.meta.env.VITE_API_URL
来源：http://zao.sjlbkw.cn

================================================================================
来源：http://xxk.tanke756.top

统计汇总
来源：http://uxj.jlsjyb.cn

================================================================================
来源：http://cas.hfpthk.cn

按语言统计（条）：
来源：http://pdc.zhongyouzk.top

Python ......... 252
来源：http://fgl.pengpengdd.cyou

PHP ............ 252
来源：http://xxp.nanxuanxn.top

JavaScript ..... 252
来源：http://mxf.kuanghao11.cn

TypeScript ..... 212
来源：http://qsh.jianghu66.top

Java ........... 212
来源：http://tkx.shangyingyoupin.top

Go ............. 212
来源：http://hdc.jlsjyb.cn

Ruby ........... 212
来源：http://uju.52xcode.cn

C# ............. 212
来源：http://upf.havefunace.top

C .............. 30
来源：http://oro.yuanzhike.top

C++ ............ 30
来源：http://own.havefunace.top

SQL ............ 90
来源：http://lqn.ywan-chungtsiang.top

Bash ........... 80
来源：http://jny.havefunace.top

Kotlin ......... 15
来源：http://mam.hesvh.cn

Swift .......... 15
来源：http://xsl.gaohongyu789.top

Lua ............ 10
来源：http://kej.yongpay.top

Perl ........... 10
来源：http://gcl.zhijiandao.cn

Scala .......... 10
来源：http://rkk.hfpthk.cn

------------------------------------
来源：http://feg.havefunace.top

合计 ........... 2106 条
来源：http://vhv.fehbvm.com

按章节统计：
来源：http://wtv.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rlo.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pzi.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yjk.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tah.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hoj.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dpi.shanyushiyangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hjc.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gos.zdbjq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xku.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bnm.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ibm.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://klg.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ewy.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vfc.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://amd.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tlg.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://jgi.fengsongda.top

R Bash 专题                             80
来源：http://jjl.cashguo.top

S C / C++ 专题                          60
来源：http://qlj.wangdashe.top

T 其他语言补充                          60
来源：http://fgx.dashuyun.cn

U 高频实用片段                         120
来源：http://qvr.yj20258888.top

------------------------------------
来源：http://gaj.yangfankeji.com

合计                                  2106 条
来源：http://xjm.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://jst.jinqigfzy.top

使用提醒
来源：http://fbu.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://ebn.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nky.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sft.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pim.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jqb.dashuyun.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jnn.tarul.cn

—— 文件结束 ——
来源：http://tfe.aibaodan.cn

================================================================================
来源：http://odf.zhoulong.xyz

程序语言常见例子速查手册（2024 版）
来源：http://ioo.316326.xyz

Common Programming Examples Cheat Book
来源：http://edw.fanxiaobao.xyz

================================================================================
来源：http://hkc.jyoumei.cn

【收录内容】
来源：http://kzi.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gsw.nwbrower.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bnv.vqdsnc.cn

SQL · Bash · C · C++
来源：http://zjh.daria6918.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cmk.svipenyu.cn

【使用说明】
来源：http://suj.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kmr.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vqn.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://efn.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ynm.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iac.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jcm.chenjidiqi.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tft.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zva.hnqzz.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jsr.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://azy.hcnkem.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gff.nanxuanxn.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xqr.ydzc1.top

【文件统计】
来源：http://sxv.zhoulong.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ztq.bjfxy.top

--------------------------------------------------------------------------------
来源：http://zfy.sysykeji.top

目  录
来源：http://pcq.shuidangran.top

--------------------------------------------------------------------------------
来源：http://lua.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kwh.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ixo.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bzf.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xjt.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vlo.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ooo.zdbjq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ulu.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xmw.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dde.sjlbkw.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gyg.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bvz.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mmy.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vmg.tianlin.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fiy.yongpay.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://abm.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oly.kuanghao11.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ivw.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xzb.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yoe.ivvv.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://msr.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vqh.yuxming.cn

================================================================================
来源：http://vgp.shzxlz.cn

A. 基础语法与类型
来源：http://xty.vehdjk.com

================================================================================
来源：http://bgx.xinyue.icu

[A01] Hello World
来源：http://kjg.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://mud.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://dvn.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://kvi.cqqwz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lcw.nwbrower.top

Java: System.out.println("Hello, World!");
来源：http://zfc.quarkkingdee.top

Go:   fmt.Println("Hello, World!")
来源：http://kwd.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://tgz.smart0.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://vrf.bjfxy.top

[A02] 变量声明与赋值
来源：http://sfi.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yir.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://cle.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://syk.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kbz.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://jhc.xziqi.cn

Go:   name := "Alex"; age := 20
来源：http://ibu.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://czh.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://zsn.birdmap.top

[A03] 常量定义
来源：http://cia.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://maj.yongpay.top

PHP:  const PI = 3.14159;
来源：http://pzz.haohaochexian.top

JS:   const PI = 3.14159;
来源：http://yas.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://okq.ctjpmb.com

Java: static final double PI = 3.14159;
来源：http://fyj.vehdjk.com

Go:   const PI = 3.14159
来源：http://xhm.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://tex.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://rfg.ywan-chungtsiang.top

[A04] 判断变量类型
来源：http://vvv.cheryme.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://okk.bbcook.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zfp.shuidangran.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vyh.jianghu66.top

TS:   typeof x; x instanceof Date
来源：http://vtz.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kjs.smart0.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://aim.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fem.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://mjg.jinqigufen.top

[A05] 整数除法与取模
来源：http://wmr.bbcook.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pya.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://und.zhiwuduotai.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zof.yj20258888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gdu.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://fvx.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://oel.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://gjq.epnwcf.com

C#:   7 / 2; 7 % 2
来源：http://jxz.gzhubu.top

[A06] 字符串转数字
来源：http://fqh.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://wya.yongpay.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hsw.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dgk.xuetiantiany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zbe.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bgd.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rsp.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jev.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jho.vqdsnc.cn

[A07] 数字转字符串
来源：http://xcg.yangfankeji.com

Py:   str(42)
来源：http://blp.hcnkem.com

PHP:  (string) 42; strval(42)
来源：http://xnu.yj20258888.top


<!-- 参考信息 -->