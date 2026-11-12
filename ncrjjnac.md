代发 wailian999

[U49] PHP：只读属性
来源：http://ypz.fanxiaobao.xyz

public readonly string $name
来源：http://ewj.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://hts.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://ezn.gogol.net.cn

[U51] PHP：数组解构
来源：http://jjc.gzhubu.top

[$a, $b] = $arr;
来源：http://cel.gzhubu.top

[U52] PHP：箭头函数
来源：http://xfd.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://zqm.hcnkem.com

[U53] PHP：空合并运算符
来源：http://kwg.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://ymt.9152youxi.cn

[U54] PHP：空安全调用
来源：http://yhu.hesvh.cn

$obj?->method()
来源：http://jks.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://gjt.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pup.andypj.xyz

[U56] PHP：命名参数
来源：http://kju.9152youxi.cn

f(a: 1, b: 2)
来源：http://wwy.jinqigufen.top

[U57] PHP：字符串插值
来源：http://vbo.shuidangran.top

"值: {$a}"
来源：http://sxi.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://nwn.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://leg.xuanzx.com

[U59] PHP：自定义排序
来源：http://xrq.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oje.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://fif.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://asb.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://slj.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vci.vehdjk.com

[U62] PHP：日期对象
来源：http://lcw.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qjt.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://byj.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://web.tarul.cn

[U64] PHP：目录遍历
来源：http://wpx.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://fty.xingfuxueyuan.xyz

[U65] PHP：会话
来源：http://aqc.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://glx.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://kjc.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pdr.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://peg.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dck.birdmap.top

[U68] PHP：PDO 连接
来源：http://tsh.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://urb.cheryme.top

[U69] PHP：PDO 预处理
来源：http://fwe.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kuj.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://icy.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jgw.sweek.top

[U71] PHP：抛出异常
来源：http://cde.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://frc.fengsongda.top

[U72] PHP：写错误日志
来源：http://tai.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://dzt.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://lfs.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://cuz.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://xcr.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://xrm.meibo888.top

[U75] PHP：依赖注入
来源：http://kmf.redwolf501.top

composer require psr/container
来源：http://jpu.cqqwz.cn

[U76] PHP：简单路由
来源：http://gxx.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ace.bjfxy.top

[U77] PHP：模板渲染
来源：http://pyb.9152youxi.cn

composer require twig/twig
来源：http://xwa.kuanghao11.cn

[U78] PHP：单元测试
来源：http://nyl.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://nsl.fzhhl.top

[U79] PHP：静态分析
来源：http://ost.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://rwy.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://jdw.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xvd.ppjwa.cn

[U81] JS：初始化项目
来源：http://vil.cucudq.cn

npm init -y;  npm i express
来源：http://mff.ivvv.top

[U82] JS：package.json 脚本
来源：http://dmo.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ats.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://ncx.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://kvy.ydzc1.top

[U84] JS：CommonJS 写法
来源：http://zvi.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://xqr.fktsv.cn

[U85] JS：可选链
来源：http://vny.zhengqikj.top

a?.b?.c
来源：http://ozb.xuanzx.com

[U86] JS：空值合并
来源：http://irj.uphjek.com

a ?? b
来源：http://gat.sweek.top

[U87] JS：解构默认值
来源：http://pno.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://hly.yj202588.top

[U88] JS：对象展开合并
来源：http://dxa.cashguo.top

{ ...a, ...b }
来源：http://rcn.tianlin.xyz

[U89] JS：数组去重
来源：http://xfz.jqgufenzy.top

[...new Set(arr)]
来源：http://scv.yangfankeji.com

[U90] JS：数字数组排序
来源：http://elo.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://obi.yfazqb.com

[U91] JS：对象键值遍历
来源：http://cfn.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oyx.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://san.ppjwa.cn

structuredClone(obj)
来源：http://wmv.yuanzhike.top

[U93] JS：模板字符串
来源：http://vcf.zhixingplan.top

`共 ${n} 条`
来源：http://cmu.yj202588.top

[U94] JS：箭头函数
来源：http://dvk.jiagoushi.top

const double = x => x * 2;
来源：http://mmu.9152youxi.cn

[U95] JS：Promise 包装
来源：http://whh.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://ozc.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://aew.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zac.xinyue.icu

[U97] JS：并发请求
来源：http://ioe.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://unk.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://qfi.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eyv.yanxiufei.cn

[U99] JS：事件监听
来源：http://qea.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://neb.jiagoushi.top

[U100] JS：DOM 查询
来源：http://qyz.hfpthk.cn

document.querySelector(".item")
来源：http://aid.daria6918.cn

[U101] JS：classList 操作
来源：http://jpw.bjfxy.top

el.classList.toggle("active")
来源：http://quf.cashguo.top

[U102] JS：本地存储
来源：http://pwt.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uqr.feifeiyinyue.top

[U103] JS：定时器
来源：http://rdg.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nms.sjlbkw.cn

[U104] JS：防抖
来源：http://hdq.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezc.hywenlv.cn

[U105] JS：节流
来源：http://bsg.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gbo.havefunace.top

[U106] JS：日期格式化
来源：http://ife.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cym.quarkkingdee.top

[U107] JS：数字千分位
来源：http://qev.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jtc.ctjpmb.com

[U108] JS：随机整数
来源：http://zkj.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mnf.nwbrower.top

[U109] JS：数组分组
来源：http://ycb.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://eir.tanke756.top

[U110] JS：数组分块
来源：http://pxi.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://znm.guannengcc.top

[U111] JS：对象转 Map
来源：http://wno.ctjpmb.com

new Map(Object.entries(obj))
来源：http://nrc.xingfuxueyuan.xyz

[U112] JS：字符串补位
来源：http://myh.aibaodan.cn

"7".padStart(3, "0")
来源：http://ekt.yfazqb.com

[U113] JS：正则替换全部
来源：http://vko.yongpay.top

s.replaceAll("a", "b")
来源：http://ner.tanke756.top

[U114] JS：JSON 深比较
来源：http://bec.zdbjq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nzu.zdbjq.cn

[U115] JS：生成 UUID
来源：http://obw.zhengqikj.top

crypto.randomUUID()
来源：http://dab.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://zmo.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://ixl.guannengcc.top

[U117] JS：单元测试
来源：http://zol.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://nda.hnqzz.top

[U118] JS：开发服务器
来源：http://ytk.cashguo.top

npm i -D vite;  npx vite
来源：http://dza.feifeiyinyue.top

[U119] JS：生产构建
来源：http://sil.52xcode.cn

npx vite build
来源：http://poq.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://jkp.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://acx.daria6918.cn

================================================================================
来源：http://vld.tanke756.top

统计汇总
来源：http://pxp.jianghu66.top

================================================================================
来源：http://wpt.jiagoushi.top

按语言统计（条）：
来源：http://zmq.zhengqikj.top

Python ......... 252
来源：http://uzg.ctjpmb.com

PHP ............ 252
来源：http://gvr.gogol.net.cn

JavaScript ..... 252
来源：http://zau.yvedp.cn

TypeScript ..... 212
来源：http://cva.tian-w.cn

Java ........... 212
来源：http://bmp.hnqzz.top

Go ............. 212
来源：http://wud.andypj.xyz

Ruby ........... 212
来源：http://btf.9152youxi.cn

C# ............. 212
来源：http://hhy.chenlongwang.top

C .............. 30
来源：http://wai.0kj1m.cn

C++ ............ 30
来源：http://buy.svipenyu.cn

SQL ............ 90
来源：http://euw.pengpengdd.cyou

Bash ........... 80
来源：http://pqt.cashguo.top

Kotlin ......... 15
来源：http://zfp.gogol.net.cn

Swift .......... 15
来源：http://rqq.hammf.cn

Lua ............ 10
来源：http://tpi.shzxlz.cn

Perl ........... 10
来源：http://sov.zhengqikj.top

Scala .......... 10
来源：http://icu.aibaodan.cn

------------------------------------
来源：http://gra.aizwys.cn

合计 ........... 2106 条
来源：http://bya.zdbjq.cn

按章节统计：
来源：http://ayh.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rbp.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mha.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fey.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://btt.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kqs.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qpo.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fes.jqgufenzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://snr.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pri.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qff.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kbi.guannengcc.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rvl.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://eba.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ijv.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jqk.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mjl.52xcode.cn

Q SQL 专题                              90
来源：http://nfi.316326.xyz

R Bash 专题                             80
来源：http://tmi.yuxming.cn

S C / C++ 专题                          60
来源：http://srm.iojbl.cn

T 其他语言补充                          60
来源：http://cpb.9152youxi.cn

U 高频实用片段                         120
来源：http://fdf.xinyue.icu

------------------------------------
来源：http://eqd.jqgfzy.top

合计                                  2106 条
来源：http://nsu.fehbvm.com

--------------------------------------------------------------------------------
来源：http://cqi.guannengcc.top

使用提醒
来源：http://dfe.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://huy.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pfu.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wrh.cucudq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hrl.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://zwb.cashguo.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nby.havefunace.top

—— 文件结束 ——
来源：http://jls.yanxiufei.cn

================================================================================
来源：http://wrj.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://usj.gzhubu.top

Common Programming Examples Cheat Book
来源：http://vss.fehbvm.com

================================================================================
来源：http://utx.xuanzx.com

【收录内容】
来源：http://owv.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ovj.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cwu.haohaochexian.top

SQL · Bash · C · C++
来源：http://jub.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uho.hfpthk.cn

【使用说明】
来源：http://tcc.jianghu66.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qdx.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vnk.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eej.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bpj.jianghu66.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tvx.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uhc.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zqh.zhongyouzk.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ixf.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://omg.fengsongda.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qyc.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rsh.yuanzhike.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nvm.smart0.xyz

【文件统计】
来源：http://jdl.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vwp.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://rka.hongshengwenyu.top

目  录
来源：http://zfv.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://lhb.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pdf.bbcook.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iqd.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cyx.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ayu.0kj1m.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bqn.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://acq.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zku.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lyt.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rnu.fanxiaobao.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zsg.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oru.ivvv.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lpr.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kyj.sufxvd.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://afk.xinyue.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qvu.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://unm.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pjb.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qld.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zwd.quarkkingdee.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://upb.yuxming.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dpm.ppjwa.cn

================================================================================
来源：http://jrt.xingfuxueyuan.xyz

A. 基础语法与类型
来源：http://sci.ehwqpu.com

================================================================================
来源：http://uxe.ywan-chungtsiang.top

[A01] Hello World
来源：http://ktx.redwolf501.top

Py:   print("Hello, World!")
来源：http://bsh.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://wwz.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://hak.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://auc.zhengqikj.top

Java: System.out.println("Hello, World!");
来源：http://fer.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://mxm.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://gqv.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lws.bbcook.cn

[A02] 变量声明与赋值
来源：http://beb.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ned.zycfv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tht.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://jfc.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nnn.zhijiandao.cn

Java: String name = "Alex"; int age = 20;
来源：http://urp.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://cpn.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://mde.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://yds.sufxvd.cn

[A03] 常量定义
来源：http://mhq.ehwqpu.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mez.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://owb.epnwcf.com

JS:   const PI = 3.14159;
来源：http://ttl.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://fim.pycfn.com

Java: static final double PI = 3.14159;
来源：http://vst.yangfankeji.com

Go:   const PI = 3.14159
来源：http://xbh.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://ghr.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://geh.feifeiyinyue.top

[A04] 判断变量类型
来源：http://lru.aibaodan.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cia.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://klf.dianchejie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nte.tarul.cn

TS:   typeof x; x instanceof Date
来源：http://zdq.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://esf.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://ehg.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jwo.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://uom.shzxlz.cn

[A05] 整数除法与取模
来源：http://myu.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gsi.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bsl.jiagoushi.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yms.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mon.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://wsb.ivvv.top

Go:   7 / 2; 7 % 2
来源：http://tnl.yangfankeji.com

Ruby: 7 / 2; 7 % 2
来源：http://wkk.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://pmb.xuetiantiany.cn

[A06] 字符串转数字
来源：http://pmx.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://vwz.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xbz.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tts.jqgfzy.top


<!-- 参考信息 -->