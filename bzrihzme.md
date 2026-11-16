代发 wailian999

[U51] PHP：数组解构
来源：http://uiz.fehbvm.com

[$a, $b] = $arr;
来源：http://xhq.ehwqpu.com

[U52] PHP：箭头函数
来源：http://pgf.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://jqw.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://cbh.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://frr.yuanzhike.top

[U54] PHP：空安全调用
来源：http://qjl.yongpay.top

$obj?->method()
来源：http://wpe.dashuyun.cn

[U55] PHP：match 表达式
来源：http://kdh.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fll.epnwcf.com

[U56] PHP：命名参数
来源：http://jgf.yueranfly.top

f(a: 1, b: 2)
来源：http://sie.cucudq.cn

[U57] PHP：字符串插值
来源：http://kww.zdbjq.cn

"值: {$a}"
来源：http://asl.tarul.cn

[U58] PHP：数组三件套
来源：http://dyn.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mmh.iojbl.cn

[U59] PHP：自定义排序
来源：http://neo.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://csq.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://zbv.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wby.chenzaomai.com

[U61] PHP：正则
来源：http://lbd.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pps.jinqigufen.top

[U62] PHP：日期对象
来源：http://ytr.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jcw.redwolf501.top

[U63] PHP：文件读写
来源：http://llv.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ldj.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://ybf.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://ekv.ehwqpu.com

[U65] PHP：会话
来源：http://dll.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ecc.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://mvp.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://twd.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://kht.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uwj.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://pff.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mmu.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://vpo.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zwk.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://zbv.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://niq.bbcook.cn

[U71] PHP：抛出异常
来源：http://oet.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://kjo.bbcook.cn

[U72] PHP：写错误日志
来源：http://ucz.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://atl.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://pqq.uphjek.com

parse_ini_file("config.ini", true)
来源：http://leh.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://wrh.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://nfs.shzxlz.cn

[U75] PHP：依赖注入
来源：http://rbn.pengpengdd.cyou

composer require psr/container
来源：http://kui.pycfn.com

[U76] PHP：简单路由
来源：http://toh.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xbc.guannengcc.top

[U77] PHP：模板渲染
来源：http://sug.cucudq.cn

composer require twig/twig
来源：http://fov.jqgfzy.top

[U78] PHP：单元测试
来源：http://nus.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://lyv.fktsv.cn

[U79] PHP：静态分析
来源：http://ejn.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://dao.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://zls.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://jqm.haohaochexian.top

[U81] JS：初始化项目
来源：http://tjm.xuanzx.com

npm init -y;  npm i express
来源：http://esf.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://pbr.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vst.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://nqa.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://irg.hammf.cn

[U84] JS：CommonJS 写法
来源：http://fdj.meibo888.top

module.exports = { a };  const { a } = require("./m");
来源：http://auf.yfazqb.com

[U85] JS：可选链
来源：http://usn.zycfv.cn

a?.b?.c
来源：http://skl.yanxiufei.cn

[U86] JS：空值合并
来源：http://xam.ywan-chungtsiang.top

a ?? b
来源：http://jmq.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://jwu.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://lrc.vehdjk.com

[U88] JS：对象展开合并
来源：http://svn.iojbl.cn

{ ...a, ...b }
来源：http://sgj.yj20258.top

[U89] JS：数组去重
来源：http://ztx.jyoumei.cn

[...new Set(arr)]
来源：http://ryo.aizwys.cn

[U90] JS：数字数组排序
来源：http://wgm.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://rky.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://fof.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pyf.hcnkem.com

[U92] JS：深拷贝
来源：http://sbq.xziqi.cn

structuredClone(obj)
来源：http://eyh.aibaodan.cn

[U93] JS：模板字符串
来源：http://pfv.cheryme.top

`共 ${n} 条`
来源：http://mtj.yonumen.top

[U94] JS：箭头函数
来源：http://rth.havefunace.top

const double = x => x * 2;
来源：http://usw.yj20258888.top

[U95] JS：Promise 包装
来源：http://qbs.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://qtd.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://jth.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xzr.yvedp.cn

[U97] JS：并发请求
来源：http://jlo.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nql.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://ody.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eut.hongshengwenyu.top

[U99] JS：事件监听
来源：http://kbv.ydjk.org.cn

el.addEventListener("click", e => {})
来源：http://iob.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://xps.jqgufenzy.top

document.querySelector(".item")
来源：http://irb.xziqi.cn

[U101] JS：classList 操作
来源：http://gph.zhengqikj.top

el.classList.toggle("active")
来源：http://yms.shanyushiyangtech.top

[U102] JS：本地存储
来源：http://kzx.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nyr.xziqi.cn

[U103] JS：定时器
来源：http://oxg.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jyo.uphjek.com

[U104] JS：防抖
来源：http://mze.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iga.daxiang520.top

[U105] JS：节流
来源：http://jsu.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tav.52xcode.cn

[U106] JS：日期格式化
来源：http://muh.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tkh.yuanzhike.top

[U107] JS：数字千分位
来源：http://zla.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dtn.epnwcf.com

[U108] JS：随机整数
来源：http://pbu.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eth.vehdjk.com

[U109] JS：数组分组
来源：http://qsw.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://rbm.bjfxy.top

[U110] JS：数组分块
来源：http://yew.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oev.xziqi.cn

[U111] JS：对象转 Map
来源：http://fcl.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://bei.chenzaomai.com

[U112] JS：字符串补位
来源：http://qjq.zycfv.cn

"7".padStart(3, "0")
来源：http://dii.gzhubu.top

[U113] JS：正则替换全部
来源：http://fkc.yfazqb.com

s.replaceAll("a", "b")
来源：http://ltd.sweek.top

[U114] JS：JSON 深比较
来源：http://leh.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://knc.chenzaomai.com

[U115] JS：生成 UUID
来源：http://wca.snrcjt.cn

crypto.randomUUID()
来源：http://zgt.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://ndl.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://yig.ehwqpu.com

[U117] JS：单元测试
来源：http://xmt.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://oxv.chenzaomai.com

[U118] JS：开发服务器
来源：http://qes.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://vkr.ydjk.org.cn

[U119] JS：生产构建
来源：http://shw.jqgufenzy.top

npx vite build
来源：http://xpl.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://viw.yj202588.top

import.meta.env.VITE_API_URL
来源：http://nob.uphjek.com

================================================================================
来源：http://bpe.xuanzx.com

统计汇总
来源：http://pcc.cqqwz.cn

================================================================================
来源：http://bye.vqdsnc.cn

按语言统计（条）：
来源：http://mxp.epnwcf.com

Python ......... 252
来源：http://oee.yj20258.top

PHP ............ 252
来源：http://vkh.dashuyun.cn

JavaScript ..... 252
来源：http://bcb.ehwqpu.com

TypeScript ..... 212
来源：http://xzc.hfpthk.cn

Java ........... 212
来源：http://hms.guowangkeji.top

Go ............. 212
来源：http://uth.gzhubu.top

Ruby ........... 212
来源：http://dgz.sysykeji.top

C# ............. 212
来源：http://luh.jiagoushi.top

C .............. 30
来源：http://wwb.zhiwuduotai.top

C++ ............ 30
来源：http://jby.cdnleiting.top

SQL ............ 90
来源：http://lst.tianlin.xyz

Bash ........... 80
来源：http://fhe.yuanzhike.top

Kotlin ......... 15
来源：http://djx.gotoacloud.top

Swift .......... 15
来源：http://dls.shangyingyoupin.top

Lua ............ 10
来源：http://jex.wangdashe.top

Perl ........... 10
来源：http://ais.jyoumei.cn

Scala .......... 10
来源：http://ipt.ydjk.org.cn

------------------------------------
来源：http://ogo.c1oappe.top

合计 ........... 2106 条
来源：http://xhh.ctjpmb.com

按章节统计：
来源：http://fkl.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pvn.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hhr.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cuo.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zok.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://muq.yonumen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qlq.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rjy.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bfb.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ams.kuanghao11.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sad.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iuq.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nih.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gjx.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fix.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cpc.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://idu.aibaodan.cn

Q SQL 专题                              90
来源：http://uze.fehbvm.com

R Bash 专题                             80
来源：http://xfc.hysaishi.cn

S C / C++ 专题                          60
来源：http://aho.sufxvd.cn

T 其他语言补充                          60
来源：http://iqw.ivvv.top

U 高频实用片段                         120
来源：http://pav.shangyingyoupin.top

------------------------------------
来源：http://hcw.zdbjq.cn

合计                                  2106 条
来源：http://ijm.xinyue.icu

--------------------------------------------------------------------------------
来源：http://aew.zycfv.cn

使用提醒
来源：http://eui.yvedp.cn

--------------------------------------------------------------------------------
来源：http://fqo.iojbl.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iho.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mdm.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uyr.epnwcf.com

在旧版本上使用前请先确认语法支持情况。
来源：http://bqn.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://euw.yuxming.cn

—— 文件结束 ——
来源：http://csi.zhixingplan.top

================================================================================
来源：http://yav.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://fqi.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://svc.chenlongwang.top

================================================================================
来源：http://zdu.cashguo.top

【收录内容】
来源：http://kkx.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://axl.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wyo.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://xrv.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qmw.guowangkeji.top

【使用说明】
来源：http://fdo.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iqm.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jnw.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pyu.fengsongda.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gis.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lrk.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sen.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pvt.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xgb.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ajp.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vzn.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eqp.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://poa.chenzaomai.com

【文件统计】
来源：http://vyj.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xyd.yueranfly.top

--------------------------------------------------------------------------------
来源：http://wws.gogol.net.cn

目  录
来源：http://lzh.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://jbv.dianchejie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vnq.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bih.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dar.cdnleiting.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cit.52xcode.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lou.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dya.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oem.hnxiangtu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qht.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://odr.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wuk.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wzz.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gxh.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qih.sjlbkw.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yyr.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lfn.vqdsnc.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ksn.0kj1m.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hvp.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hyy.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zoq.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vdp.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zgn.sufxvd.cn

================================================================================
来源：http://qix.feifeiyinyue.top

A. 基础语法与类型
来源：http://nqm.yj20258.top

================================================================================
来源：http://mat.vehdjk.com

[A01] Hello World
来源：http://znk.yueranfly.top

Py:   print("Hello, World!")
来源：http://vov.havefunace.top

PHP:  echo "Hello, World!";
来源：http://dqr.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://fyx.jiagoushi.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tvj.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://vzu.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://rsj.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://ziv.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uec.fktsv.cn

[A02] 变量声明与赋值
来源：http://knv.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zdx.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bsl.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dtl.sysykeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ghm.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://ryu.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://vua.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://tlm.sjlbkw.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tin.cdnleiting.top

[A03] 常量定义
来源：http://kmq.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bde.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://xqy.snrcjt.cn

JS:   const PI = 3.14159;
来源：http://mxt.yj202588.top

TS:   const PI: number = 3.14159;
来源：http://usp.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://nie.andypj.xyz

Go:   const PI = 3.14159
来源：http://qud.dashuyun.cn

Ruby: PI = 3.14159
来源：http://cru.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://prb.aizwys.cn

[A04] 判断变量类型
来源：http://sij.hcnkem.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://xcg.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xex.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vmd.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://aus.tianlin.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pml.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tol.iojbl.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mpa.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://zzv.zhoulong.xyz

[A05] 整数除法与取模
来源：http://gda.yongpay.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mjl.jqgfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fch.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lva.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pce.jyoumei.cn

Java: 7 / 2; 7 % 2
来源：http://ukd.havefunace.top

Go:   7 / 2; 7 % 2
来源：http://sus.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://kbg.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://fur.yj202588.top

[A06] 字符串转数字
来源：http://cfv.shanyushiyangtech.top

Py:   int("42"); float("3.14")
来源：http://abd.epnwcf.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rlv.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vck.chenzaomai.com

TS:   parseInt("42", 10); Number("42")
来源：http://uyh.pengpengdd.cyou

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tea.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dvs.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://itn.hammf.cn


<!-- 参考信息 -->