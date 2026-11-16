代发 wailian999

[U55] PHP：match 表达式
来源：http://brx.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://prr.yongpay.top

[U56] PHP：命名参数
来源：http://rui.fehbvm.com

f(a: 1, b: 2)
来源：http://qya.birdmap.top

[U57] PHP：字符串插值
来源：http://ncs.xuetiantiany.cn

"值: {$a}"
来源：http://gbx.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://ivd.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iuk.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://ifn.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jfq.gogol.net.cn

[U60] PHP：JSON 编解码
来源：http://tyl.epnwcf.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lmu.cheryme.top

[U61] PHP：正则
来源：http://cpl.yuanzhike.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mld.vehdjk.com

[U62] PHP：日期对象
来源：http://rqn.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lsv.316326.xyz

[U63] PHP：文件读写
来源：http://wpq.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ero.fktsv.cn

[U64] PHP：目录遍历
来源：http://foa.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://mxj.yj20258888.top

[U65] PHP：会话
来源：http://uax.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://cty.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://lkm.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lot.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://ixe.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qui.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://mau.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rff.havefunace.top

[U69] PHP：PDO 预处理
来源：http://ttu.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qzs.ivvv.top

[U70] PHP：PDO 事务
来源：http://yyo.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ngt.jqgfzy.top

[U71] PHP：抛出异常
来源：http://mzh.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://rkq.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://pdh.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://vlf.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://byk.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://mom.ydzc1.top

[U74] PHP：读取环境变量
来源：http://cbi.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://hjm.ybcxt.top

[U75] PHP：依赖注入
来源：http://yic.yj20258.top

composer require psr/container
来源：http://pca.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://hvh.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ykm.yongpay.top

[U77] PHP：模板渲染
来源：http://jdn.hysaishi.cn

composer require twig/twig
来源：http://xvu.fzhhl.top

[U78] PHP：单元测试
来源：http://tdy.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://htk.cashguo.top

[U79] PHP：静态分析
来源：http://uqu.uphjek.com

composer require --dev phpstan/phpstan
来源：http://nth.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://bvc.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bdk.jiagoushi.top

[U81] JS：初始化项目
来源：http://aoa.shangyingyoupin.top

npm init -y;  npm i express
来源：http://tfw.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://mra.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zoy.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://eco.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iyx.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://hgp.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://pud.meibo888.top

[U85] JS：可选链
来源：http://wul.jqgufenzy.top

a?.b?.c
来源：http://aeu.hysaishi.cn

[U86] JS：空值合并
来源：http://emo.ydjk.org.cn

a ?? b
来源：http://ecu.vehdjk.com

[U87] JS：解构默认值
来源：http://pmu.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://aze.svipenyu.cn

[U88] JS：对象展开合并
来源：http://qqt.sysykeji.top

{ ...a, ...b }
来源：http://cdr.zycfv.cn

[U89] JS：数组去重
来源：http://pfo.zhaomingkeji.xyz

[...new Set(arr)]
来源：http://vux.c1oappe.top

[U90] JS：数字数组排序
来源：http://rht.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://byx.daria6918.cn

[U91] JS：对象键值遍历
来源：http://agw.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tqc.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://uzm.yj20258.top

structuredClone(obj)
来源：http://zyz.hnqzz.top

[U93] JS：模板字符串
来源：http://ahe.tian-w.cn

`共 ${n} 条`
来源：http://fjl.hcnkem.com

[U94] JS：箭头函数
来源：http://qkw.yueranfly.top

const double = x => x * 2;
来源：http://hub.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://cvy.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://brk.fehbvm.com

[U96] JS：async/await 与异常
来源：http://hws.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pgb.yuxming.cn

[U97] JS：并发请求
来源：http://lly.vehdjk.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://iaw.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://wja.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mwp.meibo888.top

[U99] JS：事件监听
来源：http://qdf.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://aab.zhaomingkeji.xyz

[U100] JS：DOM 查询
来源：http://xug.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://xmi.zhengqikj.top

[U101] JS：classList 操作
来源：http://epc.feifeiyinyue.top

el.classList.toggle("active")
来源：http://pjh.hesvh.cn

[U102] JS：本地存储
来源：http://rru.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cfz.jqgufenzy.top

[U103] JS：定时器
来源：http://cvn.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://imf.shuidangran.top

[U104] JS：防抖
来源：http://dln.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bxq.zhoulong.xyz

[U105] JS：节流
来源：http://wwc.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vhe.redwolf501.top

[U106] JS：日期格式化
来源：http://jyt.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jjh.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://fkg.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://liz.zdqjudy.top

[U108] JS：随机整数
来源：http://art.tarul.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nco.jinqigfzy.top

[U109] JS：数组分组
来源：http://pae.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://xfq.yfazqb.com

[U110] JS：数组分块
来源：http://udn.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wba.ehwqpu.com

[U111] JS：对象转 Map
来源：http://xny.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://whh.fzhhl.top

[U112] JS：字符串补位
来源：http://liw.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://aay.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://mag.ppjwa.cn

s.replaceAll("a", "b")
来源：http://eth.hongshengwenyu.top

[U114] JS：JSON 深比较
来源：http://kqy.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ffa.cheryme.top

[U115] JS：生成 UUID
来源：http://wpi.chenlongwang.top

crypto.randomUUID()
来源：http://gpv.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://jjg.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://egg.ctjpmb.com

[U117] JS：单元测试
来源：http://jkb.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://otm.xziqi.cn

[U118] JS：开发服务器
来源：http://wfg.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://jxu.chenlongwang.top

[U119] JS：生产构建
来源：http://ybz.nanxuanxn.top

npx vite build
来源：http://fwl.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://qov.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://rdr.zhijiandao.cn

================================================================================
来源：http://nih.fengsongda.top

统计汇总
来源：http://omn.yonumen.top

================================================================================
来源：http://npt.gaohongyu789.top

按语言统计（条）：
来源：http://vnz.uphjek.com

Python ......... 252
来源：http://lwp.zhiwuduotai.top

PHP ............ 252
来源：http://bot.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://wro.yj202588.top

TypeScript ..... 212
来源：http://cay.zhiwuduotai.top

Java ........... 212
来源：http://ppt.gogol.net.cn

Go ............. 212
来源：http://zii.yueranfly.top

Ruby ........... 212
来源：http://uqh.kuanghao11.cn

C# ............. 212
来源：http://ehe.kuanghao11.cn

C .............. 30
来源：http://noi.nwbrower.top

C++ ............ 30
来源：http://qdb.zhixingplan.top

SQL ............ 90
来源：http://btj.ehwqpu.com

Bash ........... 80
来源：http://nkt.nwbrower.top

Kotlin ......... 15
来源：http://ibo.quarkkingdee.top

Swift .......... 15
来源：http://rva.tarul.cn

Lua ............ 10
来源：http://qow.nanxinkj.top

Perl ........... 10
来源：http://xgz.redwolf501.top

Scala .......... 10
来源：http://heq.cqqwz.cn

------------------------------------
来源：http://mdz.hfpthk.cn

合计 ........... 2106 条
来源：http://ztq.birdmap.top

按章节统计：
来源：http://tls.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xiz.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hnl.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dyh.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://med.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lda.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eis.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wes.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tzq.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fln.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fpk.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pkl.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rzm.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aip.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://boo.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rqw.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://axv.feifeiyinyue.top

Q SQL 专题                              90
来源：http://uff.fehbvm.com

R Bash 专题                             80
来源：http://bbf.kuanghao11.cn

S C / C++ 专题                          60
来源：http://zsu.nwbrower.top

T 其他语言补充                          60
来源：http://zwo.mhx1999.top

U 高频实用片段                         120
来源：http://ync.jqgufenzy.top

------------------------------------
来源：http://gbp.yangfankeji.com

合计                                  2106 条
来源：http://lxm.shuidangran.top

--------------------------------------------------------------------------------
来源：http://bor.jqgfzy.top

使用提醒
来源：http://onb.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://umz.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cwk.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zji.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cja.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rrh.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://awu.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://rhr.ydjk.org.cn

================================================================================
来源：http://wwg.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://ycu.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://zft.xziqi.cn

================================================================================
来源：http://jmv.gotoacloud.top

【收录内容】
来源：http://gts.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vbr.yueranfly.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cwm.yanxiufei.cn

SQL · Bash · C · C++
来源：http://aly.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nea.daxiang520.top

【使用说明】
来源：http://nqu.aizwys.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://byj.xinyue.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bee.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ewp.hnqzz.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rkj.316326.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ovw.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hei.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pom.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rax.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vyl.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://crj.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://psp.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wik.sjlbkw.cn

【文件统计】
来源：http://pgs.ybcxt.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ajv.epnwcf.com

--------------------------------------------------------------------------------
来源：http://zyv.shangyingyoupin.top

目  录
来源：http://dpj.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://lnf.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zcd.chenzaomai.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aqe.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zir.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://swd.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vxu.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://unq.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vky.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fcu.xziqi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ztb.cheryme.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lvs.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://unr.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nll.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fgr.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iji.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pxo.ydjk.org.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://liv.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mkt.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nru.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://auo.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dfo.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fro.dianchejie.cn

================================================================================
来源：http://njf.jinqigfzy.top

A. 基础语法与类型
来源：http://gep.ydzc1.top

================================================================================
来源：http://zha.hywenlv.cn

[A01] Hello World
来源：http://ety.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://srh.dianchejie.cn

PHP:  echo "Hello, World!";
来源：http://rrg.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://aih.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://doa.hammf.cn

Java: System.out.println("Hello, World!");
来源：http://aud.andypj.xyz

Go:   fmt.Println("Hello, World!")
来源：http://fku.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://nmv.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://vcq.hammf.cn

[A02] 变量声明与赋值
来源：http://wfm.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mav.daria6918.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ngp.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://lod.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qtb.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://fan.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://cia.zhiwuduotai.top

Ruby: name = "Alex"; age = 20
来源：http://tdv.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://aio.jyoumei.cn

[A03] 常量定义
来源：http://zvq.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xtp.0kj1m.cn

PHP:  const PI = 3.14159;
来源：http://gir.sxryk.cn

JS:   const PI = 3.14159;
来源：http://lkj.sweek.top

TS:   const PI: number = 3.14159;
来源：http://fou.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://lvx.yongpay.top

Go:   const PI = 3.14159
来源：http://pww.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://cjc.xuetiantiany.cn

C#:   const double PI = 3.14159;
来源：http://cai.jqgfzy.top

[A04] 判断变量类型
来源：http://blg.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://beo.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zna.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://njm.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://cni.jinqigufen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ysv.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://npu.hammf.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ljw.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://ifu.iojbl.cn

[A05] 整数除法与取模
来源：http://lle.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zqs.fktsv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cvo.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sjk.tanke756.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hmc.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://pso.sjlbkw.cn

Go:   7 / 2; 7 % 2
来源：http://yfq.xingfuxueyuan.xyz

Ruby: 7 / 2; 7 % 2
来源：http://inw.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://tvv.xziqi.cn

[A06] 字符串转数字
来源：http://jmf.yj20258.top

Py:   int("42"); float("3.14")
来源：http://mra.zhengqikj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wjv.shzxlz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uug.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gsw.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gvb.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://upc.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fgo.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ull.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://lpk.cashguo.top

Py:   str(42)
来源：http://wix.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://bkf.yj20258.top

JS:   String(42); (42).toString()
来源：http://bsv.yj20258888.top

TS:   String(42)
来源：http://ytn.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://eqz.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://edg.xinyue.icu


<!-- 参考信息 -->