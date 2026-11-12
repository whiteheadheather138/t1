代发 wailian999

[U49] PHP：只读属性
来源：http://zsw.bbcook.cn

public readonly string $name
来源：http://dcy.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://bjq.epnwcf.com

public function __construct(private int $id) {}
来源：http://ogj.cdnleiting.top

[U51] PHP：数组解构
来源：http://reb.bjfxy.top

[$a, $b] = $arr;
来源：http://cvm.fanxiaobao.xyz

[U52] PHP：箭头函数
来源：http://urr.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://syy.pycfn.com

[U53] PHP：空合并运算符
来源：http://sls.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://cbw.zhixingplan.top

[U54] PHP：空安全调用
来源：http://cbp.c1oappe.top

$obj?->method()
来源：http://avd.0kj1m.cn

[U55] PHP：match 表达式
来源：http://pop.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nqu.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://gzw.yuanzhike.top

f(a: 1, b: 2)
来源：http://ahv.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://vkv.yuanzhike.top

"值: {$a}"
来源：http://syo.dashuyun.cn

[U58] PHP：数组三件套
来源：http://aig.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rau.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://dcy.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fec.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://nvo.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jhm.dianchejie.cn

[U61] PHP：正则
来源：http://sxw.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ytu.chenlongwang.top

[U62] PHP：日期对象
来源：http://hrs.pengpengdd.cyou

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lbg.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://dqd.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pmg.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://qvh.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://kae.hcnkem.com

[U65] PHP：会话
来源：http://vtm.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ary.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://svk.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://joh.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://xcw.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jqp.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://enr.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fcy.fengsongda.top

[U69] PHP：PDO 预处理
来源：http://agv.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://exj.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://dfn.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xym.jyoumei.cn

[U71] PHP：抛出异常
来源：http://efz.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://dvx.jqgfzy.top

[U72] PHP：写错误日志
来源：http://tlb.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://vcm.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://yus.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://puk.yueranfly.top

[U74] PHP：读取环境变量
来源：http://nsp.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://kkq.havefunace.top

[U75] PHP：依赖注入
来源：http://uyl.pycfn.com

composer require psr/container
来源：http://rky.svipenyu.cn

[U76] PHP：简单路由
来源：http://pyh.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lxq.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://uyv.316326.xyz

composer require twig/twig
来源：http://xbf.ctjpmb.com

[U78] PHP：单元测试
来源：http://kmv.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://yit.yuxming.cn

[U79] PHP：静态分析
来源：http://whk.316326.xyz

composer require --dev phpstan/phpstan
来源：http://xhn.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://idr.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yzq.gogol.net.cn

[U81] JS：初始化项目
来源：http://itd.jinqigfzy.top

npm init -y;  npm i express
来源：http://xbc.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://srx.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://han.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://car.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nml.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://soo.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://cfl.fanxiaobao.xyz

[U85] JS：可选链
来源：http://tqf.haohaochexian.top

a?.b?.c
来源：http://jhw.birdmap.top

[U86] JS：空值合并
来源：http://ecl.pycfn.com

a ?? b
来源：http://bwh.gogol.net.cn

[U87] JS：解构默认值
来源：http://mep.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://xkl.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://zlh.yueranfly.top

{ ...a, ...b }
来源：http://tfs.quarkkingdee.top

[U89] JS：数组去重
来源：http://aup.jqgfzy.top

[...new Set(arr)]
来源：http://boe.tanke756.top

[U90] JS：数字数组排序
来源：http://jwd.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://ewk.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://saw.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dng.bbcook.cn

[U92] JS：深拷贝
来源：http://ypy.hongshengwenyu.top

structuredClone(obj)
来源：http://tzx.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://nyl.shangyingyoupin.top

`共 ${n} 条`
来源：http://lye.jqgufenzy.top

[U94] JS：箭头函数
来源：http://qsm.fehbvm.com

const double = x => x * 2;
来源：http://iyn.zhengqikj.top

[U95] JS：Promise 包装
来源：http://ikn.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://jpf.yuxming.cn

[U96] JS：async/await 与异常
来源：http://hhz.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sij.dianchejie.cn

[U97] JS：并发请求
来源：http://niz.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cvr.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://yym.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rtr.iojbl.cn

[U99] JS：事件监听
来源：http://lsz.hesvh.cn

el.addEventListener("click", e => {})
来源：http://qap.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://knl.yueranfly.top

document.querySelector(".item")
来源：http://vcb.fktsv.cn

[U101] JS：classList 操作
来源：http://red.tian-w.cn

el.classList.toggle("active")
来源：http://xnx.shzxlz.cn

[U102] JS：本地存储
来源：http://ocd.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vts.gotoacloud.top

[U103] JS：定时器
来源：http://fgy.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://psa.jiagoushi.top

[U104] JS：防抖
来源：http://upz.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onw.andypj.xyz

[U105] JS：节流
来源：http://crh.guannengcc.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ksx.hywenlv.cn

[U106] JS：日期格式化
来源：http://sfl.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pzd.yvedp.cn

[U107] JS：数字千分位
来源：http://mqz.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://byl.gzhubu.top

[U108] JS：随机整数
来源：http://znq.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pau.yueranfly.top

[U109] JS：数组分组
来源：http://hhe.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://ihc.yuxming.cn

[U110] JS：数组分块
来源：http://xno.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jhq.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://fqf.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://czm.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://qzd.yonumen.top

"7".padStart(3, "0")
来源：http://wqc.yangfankeji.com

[U113] JS：正则替换全部
来源：http://fsf.aibaodan.cn

s.replaceAll("a", "b")
来源：http://ygq.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://zkd.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ikh.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://zmz.smart0.xyz

crypto.randomUUID()
来源：http://qrd.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://elx.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://tqb.nanxuanxn.top

[U117] JS：单元测试
来源：http://ilx.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://ytq.bbcook.cn

[U118] JS：开发服务器
来源：http://unp.yfazqb.com

npm i -D vite;  npx vite
来源：http://wlf.snrcjt.cn

[U119] JS：生产构建
来源：http://skv.9152youxi.cn

npx vite build
来源：http://glf.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://epv.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://uub.ppjwa.cn

================================================================================
来源：http://anc.haohaochexian.top

统计汇总
来源：http://htj.zhijiandao.cn

================================================================================
来源：http://bnk.meibo888.top

按语言统计（条）：
来源：http://rfj.jqgfzy.top

Python ......... 252
来源：http://qnu.xingfuxueyuan.xyz

PHP ............ 252
来源：http://eeb.cdnleiting.top

JavaScript ..... 252
来源：http://ldq.shuidangran.top

TypeScript ..... 212
来源：http://xqi.jinghuilouyu.cn

Java ........... 212
来源：http://xpe.yueranfly.top

Go ............. 212
来源：http://rzo.zhaomingkeji.xyz

Ruby ........... 212
来源：http://vcb.fktsv.cn

C# ............. 212
来源：http://pwr.shangyingyoupin.top

C .............. 30
来源：http://igf.ppjwa.cn

C++ ............ 30
来源：http://lwd.ydjk.org.cn

SQL ............ 90
来源：http://vbc.cashguo.top

Bash ........... 80
来源：http://thy.chenjidiqi.icu

Kotlin ......... 15
来源：http://vhf.c1oappe.top

Swift .......... 15
来源：http://dcm.yfazqb.com

Lua ............ 10
来源：http://tpm.xingfuxueyuan.xyz

Perl ........... 10
来源：http://oqg.wangshuangyany.cn

Scala .......... 10
来源：http://dvq.ehwqpu.com

------------------------------------
来源：http://dtw.yj20258.top

合计 ........... 2106 条
来源：http://cnn.pycfn.com

按章节统计：
来源：http://wut.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://szf.daxiang520.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://awh.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://guv.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ekc.tanke756.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://msf.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yha.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tsw.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ysh.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://icf.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://znr.nanxuanxn.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dnq.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ebm.tanke756.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nzq.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://imb.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vfz.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rvh.hywenlv.cn

Q SQL 专题                              90
来源：http://yqc.hcnkem.com

R Bash 专题                             80
来源：http://lop.xylfe.cn

S C / C++ 专题                          60
来源：http://lbx.yuxming.cn

T 其他语言补充                          60
来源：http://yiz.hesvh.cn

U 高频实用片段                         120
来源：http://gjg.yvedp.cn

------------------------------------
来源：http://zle.ctjpmb.com

合计                                  2106 条
来源：http://rws.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://twc.fengsongda.top

使用提醒
来源：http://spu.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://vxh.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cda.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rxf.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gsn.zdqjudy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zms.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://obo.chenzaomai.com

—— 文件结束 ——
来源：http://oim.guowangkeji.top

================================================================================
来源：http://idc.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://rrz.smart0.xyz

Common Programming Examples Cheat Book
来源：http://bik.shanyushiyangkeji.top

================================================================================
来源：http://stz.andypj.xyz

【收录内容】
来源：http://coq.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rhi.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bry.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://jqw.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rsg.yangfankeji.com

【使用说明】
来源：http://pis.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xzd.aibaodan.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qun.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://inx.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ljz.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://zww.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pkr.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xfl.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kkp.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dsm.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://azz.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://afq.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lkx.birdmap.top

【文件统计】
来源：http://rbc.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vxm.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://qyt.zdbjq.cn

目  录
来源：http://bxc.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://taq.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rxc.zhengqikj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://prx.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bad.sysykeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oow.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aab.aizwys.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hym.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://drm.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aob.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jyj.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bad.epnwcf.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zpl.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xla.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kze.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mzw.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tii.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://adv.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ged.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tus.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mju.feifeiyinyue.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eim.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://psy.52xcode.cn

================================================================================
来源：http://ahz.ydzc1.top

A. 基础语法与类型
来源：http://yxl.zhiwuduotai.top

================================================================================
来源：http://fde.zhaomingkeji.xyz

[A01] Hello World
来源：http://vmw.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://xmy.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://vin.wangshuangyany.cn

JS:   console.log("Hello, World!");
来源：http://wkh.bbcook.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rfz.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://vbg.0kj1m.cn

Go:   fmt.Println("Hello, World!")
来源：http://wtz.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://bzm.ydjk.org.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qtr.shuidangran.top

[A02] 变量声明与赋值
来源：http://emb.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rti.guannengcc.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ehy.sufxvd.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yfq.fengsongda.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rct.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://gcn.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://ddu.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://qoq.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://txn.hongshengwenyu.top

[A03] 常量定义
来源：http://ehk.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bfk.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://pog.wangshuangyany.cn

JS:   const PI = 3.14159;
来源：http://dsf.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://xan.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://ohz.0kj1m.cn

Go:   const PI = 3.14159
来源：http://iuy.pengpengdd.cyou

Ruby: PI = 3.14159
来源：http://nyq.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://aye.yongpay.top

[A04] 判断变量类型
来源：http://zjz.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yyk.52xcode.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ohi.jqgfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qmo.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://css.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dvb.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://dxe.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tbq.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://ffg.zhixingplan.top

[A05] 整数除法与取模
来源：http://lns.wangshuangyany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://stg.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://sev.yj202588.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qeb.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qgy.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://lbq.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://wfn.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://gex.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://mld.cdnleiting.top

[A06] 字符串转数字
来源：http://fxu.jqgufenzy.top

Py:   int("42"); float("3.14")
来源：http://uqb.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fme.jinqigfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ndx.gogol.net.cn


<!-- 参考信息 -->