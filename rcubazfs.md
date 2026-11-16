代发 wailian999

[U49] PHP：只读属性
来源：http://oou.cashguo.top

public readonly string $name
来源：http://opk.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://gey.xylfe.cn

public function __construct(private int $id) {}
来源：http://msb.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://atf.hesvh.cn

[$a, $b] = $arr;
来源：http://kov.nwbrower.top

[U52] PHP：箭头函数
来源：http://but.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://ftx.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://rge.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://tfi.hnqzz.top

[U54] PHP：空安全调用
来源：http://iid.hfpthk.cn

$obj?->method()
来源：http://wys.tanke756.top

[U55] PHP：match 表达式
来源：http://zdk.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zbe.ydzc1.top

[U56] PHP：命名参数
来源：http://lir.zdbjq.cn

f(a: 1, b: 2)
来源：http://vxm.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://xhe.ydzc1.top

"值: {$a}"
来源：http://syq.ppjwa.cn

[U58] PHP：数组三件套
来源：http://kuy.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tnn.pycfn.com

[U59] PHP：自定义排序
来源：http://fdr.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mup.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://rut.hesvh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wom.smart0.xyz

[U61] PHP：正则
来源：http://slc.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jex.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://hap.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sca.52xcode.cn

[U63] PHP：文件读写
来源：http://xkd.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jzs.andypj.xyz

[U64] PHP：目录遍历
来源：http://xxy.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://mgz.gaohongyu789.top

[U65] PHP：会话
来源：http://wsh.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://okn.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://fwh.kuanghao11.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ons.jianghu66.top

[U67] PHP：处理文件上传
来源：http://nvi.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ffc.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://ayq.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bwn.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://swv.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tqd.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://fnj.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twy.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://qta.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://wwd.hesvh.cn

[U72] PHP：写错误日志
来源：http://pju.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://duy.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://wjc.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://iok.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://jbh.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://lgl.zhixingplan.top

[U75] PHP：依赖注入
来源：http://ukc.daxiang520.top

composer require psr/container
来源：http://yak.xylfe.cn

[U76] PHP：简单路由
来源：http://kzg.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rgm.ctjpmb.com

[U77] PHP：模板渲染
来源：http://ysw.jinqigufen.top

composer require twig/twig
来源：http://pig.hnxiangtu.top

[U78] PHP：单元测试
来源：http://yjh.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://zvz.cdnleiting.top

[U79] PHP：静态分析
来源：http://hzy.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://jrk.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://qjo.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://hyw.haohaochexian.top

[U81] JS：初始化项目
来源：http://egr.ivvv.top

npm init -y;  npm i express
来源：http://dyh.daria6918.cn

[U82] JS：package.json 脚本
来源：http://scx.gotoacloud.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iex.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://gzg.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://nxk.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://rfz.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jma.yanxiufei.cn

[U85] JS：可选链
来源：http://tkn.yvedp.cn

a?.b?.c
来源：http://vax.yuxming.cn

[U86] JS：空值合并
来源：http://yjd.quarkkingdee.top

a ?? b
来源：http://loa.52xcode.cn

[U87] JS：解构默认值
来源：http://cmi.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://sog.haohaochexian.top

[U88] JS：对象展开合并
来源：http://cap.wangdashe.top

{ ...a, ...b }
来源：http://rzl.svipenyu.cn

[U89] JS：数组去重
来源：http://tbt.sweek.top

[...new Set(arr)]
来源：http://uhb.guannengcc.top

[U90] JS：数字数组排序
来源：http://toy.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://hpr.xylfe.cn

[U91] JS：对象键值遍历
来源：http://veq.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kak.yj20258888.top

[U92] JS：深拷贝
来源：http://nou.xuetiantiany.cn

structuredClone(obj)
来源：http://frb.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://nin.nwbrower.top

`共 ${n} 条`
来源：http://slq.gotoacloud.top

[U94] JS：箭头函数
来源：http://kmb.yonumen.top

const double = x => x * 2;
来源：http://jeo.yj202588.top

[U95] JS：Promise 包装
来源：http://sjc.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://dof.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://lbr.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xae.fehbvm.com

[U97] JS：并发请求
来源：http://rfc.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ikk.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://cap.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://frb.hesvh.cn

[U99] JS：事件监听
来源：http://ghu.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://gua.jiagoushi.top

[U100] JS：DOM 查询
来源：http://ydn.shanyushiyangtech.top

document.querySelector(".item")
来源：http://vsm.smart0.xyz

[U101] JS：classList 操作
来源：http://vmg.shangyingyoupin.top

el.classList.toggle("active")
来源：http://omm.quarkkingdee.top

[U102] JS：本地存储
来源：http://wyc.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://khv.smart0.xyz

[U103] JS：定时器
来源：http://odg.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eny.yuxming.cn

[U104] JS：防抖
来源：http://fpp.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjv.sxryk.cn

[U105] JS：节流
来源：http://mjr.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://apx.jinqigfzy.top

[U106] JS：日期格式化
来源：http://zib.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zzk.yuanzhike.top

[U107] JS：数字千分位
来源：http://vin.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tvd.hcnkem.com

[U108] JS：随机整数
来源：http://ies.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fak.fengsongda.top

[U109] JS：数组分组
来源：http://lqn.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://pdf.nwbrower.top

[U110] JS：数组分块
来源：http://jri.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nma.0kj1m.cn

[U111] JS：对象转 Map
来源：http://cek.ehwqpu.com

new Map(Object.entries(obj))
来源：http://nwz.yanxiufei.cn

[U112] JS：字符串补位
来源：http://jfh.quarkkingdee.top

"7".padStart(3, "0")
来源：http://rks.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://zvg.316326.xyz

s.replaceAll("a", "b")
来源：http://mxi.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://lko.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qlt.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://hnv.jqgufenzy.top

crypto.randomUUID()
来源：http://mkj.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://wnn.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://ayo.shzxlz.cn

[U117] JS：单元测试
来源：http://mjl.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://duq.sufxvd.cn

[U118] JS：开发服务器
来源：http://hyo.52xcode.cn

npm i -D vite;  npx vite
来源：http://oyw.sxryk.cn

[U119] JS：生产构建
来源：http://gvq.0kj1m.cn

npx vite build
来源：http://pda.chenzaomai.com

[U120] JS：读取环境变量（Vite）
来源：http://bdd.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://pwi.wangshuangyany.cn

================================================================================
来源：http://gzw.svipenyu.cn

统计汇总
来源：http://zwm.52xcode.cn

================================================================================
来源：http://fht.xingfuxueyuan.xyz

按语言统计（条）：
来源：http://uyo.aibaodan.cn

Python ......... 252
来源：http://zpl.shzxlz.cn

PHP ............ 252
来源：http://tgy.ppjwa.cn

JavaScript ..... 252
来源：http://rrm.wangshuangyany.cn

TypeScript ..... 212
来源：http://zwz.jinqigufen.top

Java ........... 212
来源：http://jzr.gaohongyu789.top

Go ............. 212
来源：http://qzz.epnwcf.com

Ruby ........... 212
来源：http://xwk.iojbl.cn

C# ............. 212
来源：http://xsl.xziqi.cn

C .............. 30
来源：http://dko.xziqi.cn

C++ ............ 30
来源：http://lod.sjlbkw.cn

SQL ............ 90
来源：http://dhy.hywenlv.cn

Bash ........... 80
来源：http://pug.yanxiufei.cn

Kotlin ......... 15
来源：http://zar.xingfuxueyuan.xyz

Swift .......... 15
来源：http://uvz.svipenyu.cn

Lua ............ 10
来源：http://zho.gogol.net.cn

Perl ........... 10
来源：http://vza.zhoulong.xyz

Scala .......... 10
来源：http://les.hesvh.cn

------------------------------------
来源：http://qnn.fehbvm.com

合计 ........... 2106 条
来源：http://fuk.dashuyun.cn

按章节统计：
来源：http://bws.gogol.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ltx.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ogq.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://thy.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xkq.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pvw.yanxiufei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tgo.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vph.yonumen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ryw.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zqx.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sez.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rlv.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://coz.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vap.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wka.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aia.shangyingyoupin.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jcm.dashuyun.cn

Q SQL 专题                              90
来源：http://wlg.nwbrower.top

R Bash 专题                             80
来源：http://jkq.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://iqn.gaohongyu789.top

T 其他语言补充                          60
来源：http://fxo.shuidangran.top

U 高频实用片段                         120
来源：http://ybd.shanyushiyangkeji.top

------------------------------------
来源：http://imx.zhiwuduotai.top

合计                                  2106 条
来源：http://peh.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://jru.dashuyun.cn

使用提醒
来源：http://lec.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://gfc.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bwz.pengpengdd.cyou

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uyi.cqqwz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tgq.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ttk.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mjy.ybcxt.top

—— 文件结束 ——
来源：http://jek.yvedp.cn

================================================================================
来源：http://rbt.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://ffu.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://fke.haohaochexian.top

================================================================================
来源：http://dyg.ctjpmb.com

【收录内容】
来源：http://cpi.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://cuo.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iks.cashguo.top

SQL · Bash · C · C++
来源：http://btp.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lly.quarkkingdee.top

【使用说明】
来源：http://qvh.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://smf.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tmj.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ljh.andypj.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uto.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vst.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://npw.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wbt.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qgj.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bdd.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yzh.mhx1999.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://okw.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ksq.jlsjyb.cn

【文件统计】
来源：http://mtu.jyoumei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jho.tanke756.top

--------------------------------------------------------------------------------
来源：http://bwy.9152youxi.cn

目  录
来源：http://ckg.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://muf.ehwqpu.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hff.chenjidiqi.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hlm.dianchejie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ktm.zhongyouzk.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uxh.hnxiangtu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hjo.ctjpmb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cyc.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yky.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://adk.fanxiaobao.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oaz.xingfuxueyuan.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yld.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zmi.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ggk.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ubj.yongpay.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zhp.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zdw.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ssy.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gsl.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uqy.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vzh.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kub.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://btp.nanxinkj.top

================================================================================
来源：http://qif.ehwqpu.com

A. 基础语法与类型
来源：http://bou.nwbrower.top

================================================================================
来源：http://rqc.ivvv.top

[A01] Hello World
来源：http://jom.kuanghao11.cn

Py:   print("Hello, World!")
来源：http://usb.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://hgi.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://wjq.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hsu.svipenyu.cn

Java: System.out.println("Hello, World!");
来源：http://wil.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://mxn.cashguo.top

Ruby: puts "Hello, World!"
来源：http://lmo.gotoacloud.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mym.vqdsnc.cn

[A02] 变量声明与赋值
来源：http://ios.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dkt.feifeiyinyue.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zkr.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://ctv.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://umt.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://ygy.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://gur.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://yke.shuidangran.top

C#:   string name = "Alex"; int age = 20;
来源：http://hpn.jinyuanbaomall.cn

[A03] 常量定义
来源：http://jmj.ybcxt.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://daf.birdmap.top

PHP:  const PI = 3.14159;
来源：http://fnx.vehdjk.com

JS:   const PI = 3.14159;
来源：http://dfj.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://snf.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://qnk.smart0.xyz

Go:   const PI = 3.14159
来源：http://nes.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://paj.cqqwz.cn

C#:   const double PI = 3.14159;
来源：http://ssp.zycfv.cn

[A04] 判断变量类型
来源：http://tpg.yvedp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hwj.meibo888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cyg.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dwy.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://szd.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nkx.0kj1m.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wgc.uphjek.com

Ruby: x.class; x.is_a?(Integer)
来源：http://jjs.gogol.net.cn

C#:   x.GetType().Name; x is int
来源：http://hev.c1oappe.top

[A05] 整数除法与取模
来源：http://frw.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wav.ehwqpu.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://wxs.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ltk.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uel.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://hsn.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://tod.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://nqz.cucudq.cn

C#:   7 / 2; 7 % 2
来源：http://czx.fktsv.cn

[A06] 字符串转数字
来源：http://eaf.jqgufenzy.top

Py:   int("42"); float("3.14")
来源：http://wql.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://csx.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tyo.jlsjyb.cn


<!-- 参考信息 -->